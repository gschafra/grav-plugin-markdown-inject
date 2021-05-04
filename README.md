# Grav Markdown Inject Plugin

`Markdonws Inject` is a  [Grav][grav] Plugin that lets you inject markdown files from an external source into other pages using simple markdown syntax

# Installation

Installing the Markdown Inject plugin can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the plugin with a simple terminal command, while the manual method enables you to do so via a zip file.

## GPM Installation (Preferred)

The simplest way to install this plugin is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install markdown-inject

This will install the Markdown Inject plugin into your `/user/plugins` directory within Grav. Its files can be found under `/your/site/grav/user/plugins/markdown-inject`.

## Manual Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `markdown-inject`. You can find these files either on [GitHub](https://github.com/cron-ix/grav-plugin-markdown-inject) or via [GetGrav.org](http://getgrav.org/downloads/plugins#extras).

You should now have all the plugin files under

    /your/site/grav/user/plugins/markdown-inject

# Config Defaults

```
enabled: true
```

If you need to change any value, then the best process is to copy the [markdown-inject.yaml](markdown-inject.yaml) file into your `users/config/plugins/` folder (create it if it doesn't exist), and then modify there.  This will override the default settings.


### Page Config

(not yet implemented)

# Usage

```
[plugin:markdown-inject](https://your.doma.in/path/to/file.md)
```

This approach load the content of external markdown file into the page rendered with the associated template.  This works best for modular page content or content that uses a specific template that provides appropriate styling that is intended to be part of other pages.
