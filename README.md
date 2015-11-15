# vim-ctrlspace-docs-playground

## HOW TO?

### I want to add my project to bookmarks

[![asciicast](https://asciinema.org/a/29529.png)](https://asciinema.org/a/29529)

```shell
$ vim
[CTRL]+[C]
[b]
[a]
⌗ Add directory to bookmarks: /Users/ryrych/projects/ember_awesome/[Enter]
⌗ New bookmark name: Ember is Awesome Bookmark[Enter]
```

After adding the project to bookmarks, you choose the project from the list
using <kbd>j</kbd> and <kbd>k</kbd> keys. Press <kbd>Enter</kbd> to confirm.

An unnamed tab should open. [todo: link how to rename tab]

```
> [1*No Name] ★
```

Press <kbd>o</kbd> to open project file list. Press <kbd>r</kbd> to index all files from the
project. After indexing you should get this message:

```
⌗  Collecting files... Done (399).
```

As before use <kbd>j</kbd> and <kbd>k</kbd> keys for navigation.

### I want to open a bookmarked project (in search mode)

[![asciicast](https://asciinema.org/a/30055.png)](https://asciinema.org/a/30055)

```shell
$ vim
[CTRL]+[C]
[B]
```

Alternatively you can open the list of projects with <kbd>b</kbd> and then
open the search mode with <kbd>/</kbd>.
