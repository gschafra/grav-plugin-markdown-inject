# Grav Markdown Inject Plugin

`Markdown Inject` is a Grav Plugin that lets you inject markdown content from external sources into your page using simple markdown syntax

# Installation

Installing the Markdown Inject plugin can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the plugin with a simple terminal command, while the manual method enables you to do so via a zip file.

## GPM Installation (Preferred)

The simplest way to install this plugin is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install markdown-inject

This will install the Markdown Inject plugin into your `/user/plugins` directory within Grav. Its files can be found under `/your/site/grav/user/plugins/markdown-inject`.

## Clone GitHub repository

Use your system's Terminal (also called the command line).  From the root of your Grav install type:

```
$ cd user/plugins 
$ git clone https://github.com/cron-ix/grav-plugin-markdown-inject.git markdown-inject/
```


This will install the Markdown Inject plugin into your `user/plugins` directory within Grav. Its files can be found under `/your/site/grav/user/plugins/markdown-inject`.

To update the plugin go to the plugins root folder `/your/site/grav/user/plugins/markdown-inject/` and type:

    git pull
    
## Manual Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `markdown-inject`. You can find these files either on [GitHub](https://github.com/cron-ix/grav-plugin-markdown-inject) or via [GetGrav.org](http://getgrav.org/downloads/plugins#extras).

You should now have all the plugin files under

    /your/site/grav/user/plugins/markdown-inject

# Config Defaults

```
enabled: true
```

If you need to change any value, then the best process is to copy the [markdown-inject.yaml](markdown-inject.yaml) file into your `users/config/plugins/` folder (create it if it doesn't exist), and then modify there.  This will override the default settings.

# Usage

To load an external Markdown file:
```
[plugin:markdown-inject](https://your.domain.com/path/to/file.md)
```
To load the output from an external php script:
```
[plugin:markdown-inject](https://your.domain.com/path/to/file.php)
```
To load the content of an external nextcloud share:
```
[plugin:markdown-inject](https://cloud.domain.de/index.php/s/SomeRandomStuff42/download)
```

**Important:** only https URLs are allowed.

This approach load the content of external source into the page.
