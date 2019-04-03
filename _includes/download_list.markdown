## RubyInstaller <a id="archive" href="{{ "/downloads/archives" | relative_url }}">Архивы</a>

Не знаете, какую версию выбрать? Тогда прочтите инструкцию справа.

###  С Devkit

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "ridkexe" | where: "show", "true") %}
  {% include downloadlinks.html dls=dls %}
</ul>

### Без Devkit

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "rubyinstallerexe" | where: "show", "true") %}
  {% include downloadlinks.html dls=dls %}
</ul>

## Другие полезные дополнения

### 7-Zip архиватор

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "rubyinstaller7z" | where: "show", "true") %}
  {% include downloadlinks.html dls=dls %}
</ul>


### Основы Ruby и документация стандартной библиотеки (старая)

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "rubychm7z" | where: "show", "true") %}
  {% include downloadlinks.html dls=dls %}
</ul>


### Development Kit (старая)

#### Для Ruby версий от 2.0 до 2.3 (для 32-битной версии):

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "devkitsfx" | where: "show", "32") %}
  {% include downloadlinks.html dls=dls %}
</ul>


#### Для Ruby версий от 2.0 до 2.3 (для 64-битной версии)

<ul>
  {% assign dls = (site.data.downloads | where: "filetype", "devkitsfx" | where: "show", "64") %}
  {% include downloadlinks.html dls=dls %}
</ul>
