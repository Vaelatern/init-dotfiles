Easy Dotfiles
=============

**The problem:** Everybody and their grandma has a way to manage an existing
dotfiles repository. However, there is no easy way create a dotfiles repository
to start with. Even if someone uses a dotfile manager, they still need to move
files themselves, go through the manager install and configuration process, and
setup a repository under version control.

We aim to do all of this for you. All you need to do is run it, and
give it permission to do everything it does.

Currently, the script is designed for use with [Dotbot][dotbot-repo] dotfile manager and git.

Get Running in 5 Minutes
------------------------

```bash
  wget https://raw.githubusercontent.com/Aviator45003/easy-dotfiles/master/easy_setup.sh
  ./eash_setup.sh
```

Usage
--------------------

- `test` - Test mode. Nothing will actually be done. Best if you are wary
  about the whole thing. Default: No.

- `verbose-config` - The DotBot configuration will have every option
  explicitly set. Default: No.

- `dump-config` - The configuration will be sent to `stdout`, perfect for
  redirecting into a file. Default: No.

- `preview` - Commands will be printed to the console before being executed.
  There won't be newlines between them, but you can see what they are. Default:
  Yes.

Every command line option can have `no-` prepended to turn off the option.

For example:

```bash
  ./easy_setup.sh test no-preview
```

Will enable the `test` option and disable the `preview` option.

Contributing
------------

If you want to help out, there are two ways to do that. Either you can open an
issue, or you can fork and pull request. If you wanted a file added to your
dotfiles that isn't looked for in the script, open an issue.

[dotbot-repo]: https://github.com/anishathalye/dotbot
