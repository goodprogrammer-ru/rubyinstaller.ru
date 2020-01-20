---
layout: downloads
title: Скачать
permalink: /downloads/
---
### Какую версию загружать?

Если вы не знаете, какую версию RubyInstaller установить и только начинаете работать с Ruby, то используйте
установщик <b>Ruby+DevKit 2.6.x (x64)</b>. Он содержит наибольшее количество совместимых гемов и устанавливает
MSYS2-DevKit вместе с Ruby, потому гемы с расширением C скомпилируются сразу же. 32-битную (x86) версию советуем,
только если приходится работать с пользовательскими 32-битными встроенными DLL- или COM-объектами.

### Как обновлять?

Обновите Ruby до свежего патча (например, с версии 2.5.1 до 2.5.4), запустив соответствующую версию установщика.
Существующие гемы не перезапишутся и будут стабильно работать с новыми версиями. Используйте RubyInstaller
(без DevKit), чтобы обновить установки. Сам DevKit обновляйте отдельно с помощью команды `ridk install`.

Если вы загружаете версию Ruby из другой стабильной ветки (2.6.x, например), используйте новую директорию для этого.
То есть не следует обновлять RubyInstaller-2.5.x до версии 2.6.x, так как гемы с расширением C несовместимы между
Ruby 2.5 и 2.6. Больше информации об этом в разделе [FAQ](https://github.com/oneclick/rubyinstaller2/wiki/FAQ#user-content-update-install).

### RubyInstaller-head

RubyInstaller-head – это ежедневно обновляемая версия [Ruby development branch](https://github.com/ruby/ruby/).
Ее можно использовать для тестов непрерывной интеграции (CI) ваших гемов или приложений, чтобы вы были готовы к ближайшим изменениям ядра руби. 
Сборки доступны на URI стабильной загрузки в [разделе github release](https://github.com/oneclick/rubyinstaller2/releases/tag/rubyinstaller-head).
Их можно с легкостью [интегрировать в Appveyor](https://github.com/oneclick/rubyinstaller2/wiki/For-gem-developers#user-content-appveyor).

### Какую версию Development Kit выбрать?

Для Ruby 2.4.0 и новее в качестве комплекта разработки используется [пакет MSYS2](http://www.msys2.org). Он входит в
состав <b>Ruby+DevKit</b> как компонент по выбору, чтобы не было нужды скачивать/устанавливать MSYS2 дополнительно.
Если используете Ruby без DevKit, то MSYS2 DevKit устанавливайте отдельно командой `ridk install`

### RubyInstaller-head

RubyInstaller-head is a daily updated version of the [Ruby development branch](https://github.com/ruby/ruby/).
It can be used for continuous integration tests (CI) on your gems or applications, so that you’re prepared for upcoming changes to the ruby core.
Builds are available on stable download URIs in the [github release section](https://github.com/oneclick/rubyinstaller2/releases/tag/rubyinstaller-head).
They can be easily [integrated into Appveyor](https://github.com/oneclick/rubyinstaller2/wiki/For-gem-developers#user-content-appveyor).

### With Development Kit?

RubyInstaller uses the [MSYS2 toolchain](http://www.msys2.org) as development kit.
It is bundled into the <b>Ruby+Devkit</b> installer version as a selectable component, so that no additional downloads/installs are required.
It's possible to [share one Devkit](https://github.com/oneclick/rubyinstaller2/wiki/FAQ#user-content-shared-devkit) for multiple Ruby versions.

MSYS2 требуется, чтобы компилировать дополнения на C/C++ для Ruby. Он необходим также для [Ruby on Rails](http://rubyonrails.org/). 
Более того, MSYS2 позволяет загружать и использовать [сотни Open Source библиотек](https://github.com/Alexpux/MINGW-packages), 
от которых могут зависеть некоторые гемы.

Среду разработки MSYS2 запускайте в консоли с помощью `ridk enable`. Она добавляет команды `make`, `gcc`, `pacman` 
или `sh` к пути поиска. Больше информации в [вики](https://github.com/oneclick/rubyinstaller2/wiki/The-ridk-tool).

### Скорость и  удобство

RubyInstaller компилируется с помощью GCC в дату выхода. Установленный Ruby — это нативное Windows-приложение,
которое работает вкупе с функциональным дистрибутивом [MSYS2](http://www.msys2.org) и
[MINGW-библиотеками](https://github.com/Alexpux/MINGW-packages).

Ищите больше о RubyInstaller и его альтернативах [здесь]({{ "/about/comparison" | relative_url }}).

### Документация

Основы и документация стандартной библиотеки Ruby входит в установочный пакет. Мы рекомендуем почитать ещё и
[online-вариант](https://ruby-doc.org/) или HTML-версию, которую можно скачать на [ruby-doc.org](https://ruby-doc.org/downloads/).

### Поддержка

Делитесь вашим мнением о RubyInstaller или предлагайте улучшения в нашей дружелюбной и полезной 
[Google Группе](http://groups.google.com/group/rubyinstaller). Счастливого программирования на Ruby!
