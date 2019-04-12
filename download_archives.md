---
layout: download_archives
title: Загрузить архивы
permalink: /downloads/archives/
---

<div>
<div class="span-8 border" markdown="1">

## Версии установщика Ruby+Devkit

<ul>
  {% assign dls = site.data.downloads | where: "filetype", "ridkexe" %}
  {% include downloadlinks.html dls=dls %}
</ul>

## Версии установщика Ruby

<ul>
  {% assign dls = site.data.downloads | where: "filetype", "rubyinstallerexe" %}
  {% include downloadlinks.html dls=dls %}
</ul>

[« Назад]({{ "/downloads" | relative_url }})
</div>
<div class="span-8 border" markdown="1">

## Архивы
<ul>
  {% assign dls = site.data.downloads | where: "filetype", "rubyinstaller7z" %}
  {% include downloadlinks.html dls=dls %}
</ul>
</div>


<div class="span-8 last" markdown="1">
## Документация
<ul>
  {% assign dls = site.data.downloads | where: "filetype", "rubychm7z" %}
  {% include downloadlinks.html dls=dls %}
</ul>

## Версии DevKit
<ul>
  {% assign dls = site.data.downloads | where: "filetype", "devkitsfx" %}
  {% include downloadlinks.html dls=dls %}
</ul>
</div>
</div>
