# Sublime Grunt

A [Grunt](https://github.com/gruntjs/grunt) task runner for Sublime Text.

![Screencast of Sublime Grunt](screencast.gif)

## Installation

### Package Control

The easiest way to install is using Sublime's [Package Control](https://packagecontrol.io/packages/Grunt). It's
listed as `Grunt`.

1. Open `Command Palette` using menu item `Tools → Command Palette...`
2. Choose `Package Control: Install Package`
3. Find `Grunt` and hit `Enter`

### Manually

1. [Download the tarball](https://github.com/sptndc/sublime-grunt/releases)
2. Extract and rename folder to `Grunt`
3. Copy folder into `Packages` directory, which you can find using
   the menu item `Preferences → Browse Packages...`

## Usage

Open the Command Palette:

* macOS: <kbd>cmd+shift+P</kbd>
* Linux/Windows: <kbd>ctrl+shift+P</kbd>

Now choose the "Grunt" command.

The plugin expects to find a Gruntfile (`Gruntfile.js` or
`Gruntfile.coffee`) in an open folder. It displays a sorted list of
available Grunt tasks out of this Grunt file. If it finds more than
one Gruntfile, it first provides a list for selection.

As of version 0.2, there is also a command to kill running tasks, for
example `watch` tasks.

## Settings

The file `SublimeGrunt.sublime-settings` is used for configuration.

You may override your `PATH` environment variable as follows:

```
{
    "exec_args": {
        "path": "/bin:/usr/bin:/usr/local/bin"
    }
}
```

If your GruntFile is not in the base path of the project, then you
can add the path(s) to check as follows:

```
{
    "gruntfile_paths": [
        "/path",
        "/another/path",
        "/one/final/path"
    ]
}
```

Alternatively this could be set per-project in your .sublime-project
settings object.

## Maintenance

sublime-grunt was created by [Tim von Oldenburg](https://github.com/tvooo) and is
currently maintained by [Septian Dwic.](https://github.com/sptndc).

## License

This project was released under the [MIT](LICENSE) License.
