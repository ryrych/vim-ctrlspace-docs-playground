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

### I want to group files in a separate tab

[![asciicast](https://asciinema.org/a/30059.png)](https://asciinema.org/a/30059)

```shell
$ vim

# Open Ember project
[CTRL]+[SPACE]
[B]
>ember<
[Enter]

# Search for `README.md` and open it in the current tab without closing the plugin window
[O]
>readme<
[enter][space]

# Open 3 files in a separate tab (note the `+3` indicator)
[/]
[CTRL]+[U]
>computed<

# Select each file with:
[SHIFT]+[T]

# Clear search term
[/]
[CTRL]+[U]
[/]

# Open list of tabs
[l]

# Give second tab custom label
[j]
[=]
>Computed feature + spec<
[Enter]
[ESC]
[qa]
```

[Link to gist](https://gist.github.com/ryrych/e95ba23a5f71c93cfda4)

#### Notes

<kbd>[CTRL]+[U]</kbd> is a normal shell command to clear backward from point to
the beginning of line. You can use any valid command like <kbd>[CTRL]+[H]</kbd>.
See this [Bash CheatSheet for UNIX Systems](https://gist.github.com/LeCoupa/122b12050f5fb267e75f) for more.

##### Clear search term improved

Instead of:

```shell
[/]
[CTRL]+[U]
[/]
```

you can just press <kbd>[Backspace]</kbd>.
