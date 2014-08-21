---
layout: main
title: 'Changelog'
description: 'Changelog for all versions of Dash to Dock'
section: 'development'
order: 2
---

<a name="changelog"></a>
## Change log

The version numbering follows the uploads to the extension website. Releases divided by GNOME Shell version supports are listed in the [release page](.{{ site.release_page_url }}) with links to the zip archives.

{% for release in site.data.releases %}
<a name="v{{ release.version }}"></a>
<p><strong>Version {{ release.version }} ({{ release.date }})</strong></p>
<p>Compatible with GNOME Shell: {{ release.shell_version | join: ', ' }} </p>
<ul>
{% for rn in release.notes %}
<li>{{ rn }}</li>
{% endfor %}
</ul>
{% endfor %}
