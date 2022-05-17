# Template Select plugin for Craft CMS 4.x [WORK IN PROGRESS]

A fieldtype that allows you to select a template from the site templates folder.

![Screenshot](resources/img/field-screenshot@2x.png)

## Requirements

This plugin requires Craft CMS 4 or later.

## Installation

To install the plugin, follow these instructions.

1. Open your terminal and go to your Craft project:

        cd /path/to/project

2. Then tell Composer to load the plugin:

        composer require breizhwave/craft4-templateselect:@dev


3. In the Control Panel, go to Settings → Plugins and click the “Install” button for Template Select.

## Configuring Template Select

You may limit the template list to a subfolder of the site template folder.

The path is relative, i.e. _subfolder/subfolder2/_.

![Subfolder](resources/img/field-config@2x.png)

## Using Template Select

If you want to include a template, you may do it like this in your entry template:

```twig
{% include entry.fieldHandle %}
```
or if you have limited to a subfolder :
```twig
 {% include "_subfolder/subfolder2/" ~  entry.wavetemplate    %}

```

Brought to you by [Superbig](https://superbig.co) and [wave.bzh](https://wave.bzh)
