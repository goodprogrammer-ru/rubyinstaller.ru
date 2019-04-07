## RubyInstaller <a id="archive" href="{{ "/downloads/archives" | relative_url }}">Архивы</a>

Не знаете, какую версию выбрать? Тогда прочтите инструкцию справа.

###  С Devkit

<ul>
  {% assign dls = site.data.downloads | where: "filetype", "ridkexe" | where: "show", "true" %}
  {% include downloadlinks.html dls=dls %}
</ul>

### Без Devkit

<ul>
  {% assign dls = site.data.downloads | where: "filetype", "rubyinstallerexe" | where: "show", "true" %}
  {% include downloadlinks.html dls=dls %}
</ul>

## Другие полезные дополнения

### 7-Zip архивы

<ul>
  {% assign dls = site.data.downloads | where: "filetype", "rubyinstaller7z" | where: "show", "true" %}
  {% include downloadlinks.html dls=dls %}
</ul>
