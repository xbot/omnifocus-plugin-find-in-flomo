# omnifocus-plugin-find-in-flomo
Find the current project in flomo.

Search in Flomo according to the selected project or the containing project of the selected task.

## Quick Start Guide

### Installation

Clone the repo and link it in the Automation Configuration dialog in OmniFocus, or add it as a git submodule to the default plugin folder of OmniFocus. I recommend the latter for an easier synchronization with other devices.

```shell
cd ~/Library/Mobile Documents/iCloud~com~omnigroup~OmniFocus/Documents/Plug-Ins

git init

git submodule add https://github.com/xbot/omnifocus-plugin-find-in-flomo.git find-in-flomo

# For updating:
git submodule update --remote --recursive
```

### Configuration

You must set settings in the preferences dialog before this plugin works.

In macOS, hold the CTRL key and click the menu item `Automation` → `Find in Flomo` to open the preferences dialog.

In iOS, tap the console icon in the home perspective, then tap the corresponding menu item.

`Pattern` is a regular expression which will be used to match the selected project name.

`Keyword template` is a string template, the matched results will be used to fill this template and then be used to search in flomo as a keyword.

`Tag` is the name of a tag in Flomo, this option is optional, if set, it will be appended to the query URL to filter the results as an additional dimension.

