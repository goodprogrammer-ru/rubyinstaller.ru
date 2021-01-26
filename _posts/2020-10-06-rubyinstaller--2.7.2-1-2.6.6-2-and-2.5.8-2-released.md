---
layout: post
title:  "Вышли версии установщика Ruby 2.7.2-1, 2.6.6-2 и 2.5.8-2"
author: Lars Kanis
---
Вышли версии установщика Ruby 2.7.2-1, 2.6.6-2 и 2.5.8-2. Это служебные обновления с исправлениями ошибок и проблем безопасности.

Эта серия обновлений исправляет [найденные недавно проблемы](https://github.com/oneclick/rubyinstaller2/issues/184) с установкой пакета MSYS2 и обновлением MSYS2.
Как необязательный компонент при установке также добавлена RI документация, которая теперь интегрирована в `irb` на Ruby-2.7 и улучшает использование команды [`ridk use`](https://github.com/oneclick/rubyinstaller2/wiki/The-ridk-tool).
Также, в этих релизах содержатся несколько обновлений к встроенным библиотекам и обновление списка сертификатов TLS.

Если нунжы подробности, смотрите [анонс релиза ruby-2.7.2](https://www.ruby-lang.org/en/news/2020/10/02/ruby-2-7-2-released/) и список изменений установщика Ruby (CHANGELOG) для версий [RubyInstaller-2.5.8-2](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.5.md#rubyinstaller-258-2---2020-10-06), [RubyInstaller-2.6.6-2](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.6.md#rubyinstaller-266-2---2020-10-06) и [RubyInstaller-2.7.2-1](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.7.md#rubyinstaller-272-1---2020-10-06).

К сожалению, на момент написания этого поста, основной сервер пакета MSYS2 [https://repo.msys2.org](https://repo.msys2.org) недоступен.
`pacman` сам выберет альтернативные адреса, правда с довольно большой задержкой.
Если хотите её избежать, можно закомментировать основной сервер, используя первую команду и изучить оставшиеся сервера второй командой:
```
ridk exec sh -c "sed -e '/repo.msys2.org/ s/Serv/#Serv/' -i /etc/pacman.d/mirrorlist.*"
ridk exec sh -c "cat /etc/pacman.d/mirrorlist.*"
```

Как всегда, бинарники доступны в разделе [Скачать]({{ "/downloads/" | relative_url }})!
