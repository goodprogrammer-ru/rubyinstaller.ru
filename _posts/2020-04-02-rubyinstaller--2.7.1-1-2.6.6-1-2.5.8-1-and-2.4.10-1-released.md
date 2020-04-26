---
layout: post
title:  "Новые версии RubyInstaller 2.7.1-1, 2.6.6-1, 2.5.8-1 и 2.4.10-1"
author: Lars Kanis
---
Вышли новые версии установщика RubyInstaller 2.7.1-1, 2.6.6-1, 2.5.8-1 и 2.4.10-1. В рамках поддержки исправлены ошибки и уязвимости.

Подробнее смотрите [ruby-2.4.10](https://www.ruby-lang.org/en/news/2020/03/31/ruby-2-4-10-released/), [ruby-2.5.8](https://www.ruby-lang.org/en/news/2020/03/31/ruby-2-5-8-released/), [ruby-2.6.6](https://www.ruby-lang.org/en/news/2020/03/31/ruby-2-6-6-released/) и [ruby-2.7.1 release notes](https://www.ruby-lang.org/en/news/2020/03/31/ruby-2-7-1-released/), а также в файлах в CHANGELOG для [RubyInstaller-2.4.10-1](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.4.md#rubyinstaller-2410-1---2020-04-02), [RubyInstaller-2.5.8-1](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.5.md#rubyinstaller-258-1---2020-04-02), [RubyInstaller-2.6.6-1](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.6.md#rubyinstaller-266-1---2020-04-02) и [RubyInstaller-2.7.1-1](https://github.com/oneclick/rubyinstaller2/blob/master/CHANGELOG-2.7.md#rubyinstaller-271-1---2020-04-02).
Объединенные с OpenSSL версии обновлены до 1.0.2u (Ruby-2.4.x) и 1.1.1f (Ruby-2.5+).

Все вышеперечисленные версии установщика RubyInstaller переключились на [Reline](https://github.com/ruby/reline) в качестве редактора строк для irb и дргуих приложений, использующих интерактивную консоль.

Также теперьвсе установщики по умолчанию используют UTF-8 в качетсве внешней кодировки символов.

Все эти изменения [уже были в RubyInstaller-2.7.1-1]({% post_url 2020-01-05-rubyinstaller-2.7.0-1-released %}), а теперь портированы в более ранние версии RubyInstaller-2.4, 2.5 and 2.6.

Обратите внимание, что RubyInstaller-2.4.10-1 будет последней версии установщика в линейке Ruby-2.4.

Причина — окончание поддержки Ruby-2.4 и OpenSSL-1.0.x.

Все бинарники лежат в секции [Скачать]({{ "/downloads/" | relative_url }})!
