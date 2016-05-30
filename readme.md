#Tag-ST2

This is my repo of the last version of [Tag](https://github.com/titoBouzout/Tag) to be released for Sublime Text 2. I strongly urge you to upgrade to [ST3](https://sublimetext.com/3 "Sublime Text 3") if at all possible and use [this version](https://packagecontrol.io/packages/Tag) of the plugin. However, if you still need to stay with ST2 for whatever reason, this repo is here for you.

## Important Note

I do not plan on maintaining this package. If you absolutely *must* file an issue or a PR, go right ahead (I'm not disabling them), but don't feel bad if I ignore you.

## Installation

For now the only way to install it is manually. There are two ways to do this: by downloading an archive, or via git. Both methods require you know where your `Packages` folder is:

* Windows Regular Install: `%APPDATA%\Sublime Text 2\Packages`
* Windows Portable Install: `InstallationFolder\Sublime Text 2\Data\Packages`
* OS X: `~/Library/Application Support/Sublime Text 2/Packages`
* Linux: `~/.config/sublime-text-2/Packages`

The menu item **`Preferences → Browse Packages…`** will open the `Packages` folder in your operating system's file manager application (Windows Explorer, Finder, Nautilus, etc.).

### Archive

Download the [`zip` file](https://github.com/MattDMo/Tag-ST2/archive/master.zip) or [`tar.gz` file](https://github.com/MattDMo/Tag-ST2/archive/master.tar.gz). Go the the `Packages` folder and unzip/untar.gz the archive there. It'll create a `Tag-ST2` folder. Rename it to `Tag`. Completely restart Sublime and you're all set.

### Git

Go to the `Packages` folder in the command line and run

    git clone https://github.com/MattDMo/Tag-ST2.git Tag

to create a `Tag` folder. Completely restart Sublime and you're all set.

# Original README

Description
------------------

"Tag" plugin is a collection of packages about tags, mixed together in an effort to provide a single package with utilities to work with tags.

Currently provides: "Close tag on slash", "Tag indent or AutoFormat Tags",  "Tag Remove", "Insert as Tag", "Tag Remove Attributes", "Tag Close", "Tag Lint"

Improvements and more features about tags are welcome on this package. Please submit these.

Source / Installation
------------------

Convenient way to install this plugin is to use "Package Control" via http://wbond.net/sublime_packages/package_control

Upgrade
------------------

If you already installed "Close tag on slash" or "Tag indent", please remove these packages first and the associated settings. "Close tag on slash" already provides keymap for "/", then if you already installed that keymap you may want to remove it.

Close tag on slash
------------------

A command that is meant to be bound to the slash ("/") key in order to semi auto close open HTML tags (in part inspired by the discussion at http://www.sublimetext.com/forum/viewtopic.php?f=5&t=1358).
Requires build 2111 or later of Sublime Text 2.

*Usage*

Runs automatically when inserting an Slash "/" into an HTML document.

Tag Indent
------------------

Apply and/or add beauty indentation to HTML/XML/RDF/XUL tags found on selection(s).

*Aims*

Aims to add and/or apply correct indentation to little portions of HTML or XML, not to complete documents.

*Usage*

There is context menuitems called "Indent Tags on Selection", "Indent Tags on Document"

There is also Main menuitems: Edit -> Tag -> "Indent Tags on Selection", "Indent Tags on Document"

There is also commands "Indent Tags on Selection", "Indent Tags on Document"

*Information*

It takes the starting "indentation level" from the first line of each selection and sums tabs as needed.

On empty tags, and on tags with less than 60 characters, it writes the tag in one line.

Short-cut is "ctrl+alt+f"

Tag Remove
------------------

Provides the ability to remove all tags or some selected tags in a document or in selection(s).

*Usage*

The main menu "Edit" -> "Tag" provide access to the commands

Insert As Tag
------------------

Converts the current word to an html-tag. If there is no current word, a default tag is inserted.

*Usage*

The short-cut is "ctrl+shift+,"

Tag Remove Attributes
------------------

Allows to remove attributes from tags for selection or document.

*Usage*

The main menu "Edit" -> "Tag" provide access to the commands

Tag Close
------------------

Overwrite the built-in funtionallity by a custom one provided by this package which fix some bugs.

*Usage*

Windows, Linux : ALT+.
OSX : SUPER+ALT+.

Tag Lint
------------------

Experimental feature which aims to check correctness of opened and closed tags.

*Usage*

The main menu "Edit" -> "Tag" -> "Tag Lint"

---

Just in case it's not clear: ***I didn't write any of this. This is all Tito Bouzout's work, and all credit goes to him. This repo is simply a mirror of his code provided for the public good.***
