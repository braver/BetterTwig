# Twig

A Sublime Text package that offers enhanced syntax highlighting, snippets, completions and much more for PHP [Twig](https://twig.symfony.com/) templates. 

## Features

- Indentation for code blocks.
- Snippets for common code blocks.
- Key bindings to make your life easier.
- Enhanced syntax highlighting for Twig templates.
- Autocompletions for built in tags, filters, functions, tests & loop variables.

## Installation

#### Package Control

The easiest way to install is using [Package Control](https://packagecontrol.io). It's listed as `Twig`.

1. Open `Command Palette` using <kbd>ctrl+shift+P</kbd> or menu item `Tools → Command Palette...`
2. Choose `Package Control: Install Package`
3. Find `Twig` and hit <kbd>Enter</kbd>

## Documentation

### How to use this package ?

By default, this package supports Twig in these file extensions:

1. `.twig`
2. `.htm.twig`
3. `.html.twig`

Since a user can have more than one templating language package installed, this package doesn't support `.html` directly. To get highlighting for `.html` files with Twig code and all the other features this package provides, you can follow any of the two approaches given below 

1. Go to the bottom right status bar item that displays information on current syntax and click on that when the currently open file is any `.html` file. From there go to `Open all with current extensions as ...` and scroll to select `HTML (Twig)`. You should now be good to go.

2. When the currently open file is a `.twig` file, from the main menu, go to `Preferences -> Settings -- Syntax Specific`. This should open a 2 column new window, with the default settings on the right and a user settings on the left. In the user settings, add the following, save & close.

```json
{
    "extensions": [
        ".html"
    ]
}
```

### Snippets

This package adds basic snippets for common code blocks. If you want more snippets, then please follow the official documentation on
[snippets](https://www.sublimetext.com/docs/completions.html#snippets) and create your own. Or use [SnippetMaker](https://packagecontrol.io/packages/SnippetMaker) for convenience.

- apply
- autoescape
- block
- dump
- embed
- extends
- for
- if
- if else
- include
- macro
- sandbox
- set
- verbatim
- with

If you want to ignore the snippets that are provided by default, you can use the `ignored_snippets` setting.

`"ignored_snippets": ["Twig/*"]`

## Reporting issues.

There is always scope for improvements, so please do report any bug(s) that you encounter.

Use the [Twig playground](https://twigfiddle.com/) if you want to share a particular snippet of template while creating a specific issue.
