Easy Dotfiles
=============

The `easy_setup` script was created as a solution to [Dotbot's 
issue #22][origin-issue]. The problem: Everybody and their grandma has a way to
manage an existing dotfiles repository. However, there isn't an existing 
mechanism to easily setup a dotfiles repository to start with. Even if someone
uses a dotfile manager, they still need to move files themselves, go through 
the manager install and configuration process, and setup a repository so the 
version control system can function.

This script aims to do everything for you. All you need to do is run it, and 
give it permission to do everything it does.

Currently, the script is designed for use with the [DotBot dotfiles
manager][dotbot-repo] and git.

Command Line Options
--------------------

Every command line option can have ``no-`` prepended to turn off the option.
You can pass options in any order, but the last time an option is passed will 
be the final state of that flag.

Note that the script uses ``stderr`` whenever possible, only sending the DotBot 
configuration file to ``stdout``. The reasons were not well thought out, but 
hey, it's a feature.

``./easy_setup.sh test no-test test no-test test`` will end up in test mode.

- ``test`` - Test mode. Nothing will actually be done. Best if you are wary 
  about the whole thing. Default: No.

- ``verbose-config`` - The DotBot configuration will have every option explicitly set. Default: No.

- ``dump-config`` - The configuration will be sent to ``stdout``, perfect for 
  redirecting into a file. Default: No.

- ``preview`` - Commands will be printed to the console before being executed. 
  There won't be newlines between them, but you can see what they are. Default: 
  Yes.


Contributing
------------

If you want to help out, there are two ways to do that. Either you can open an 
issue, or you can fork and pull request. Either way, your feature will likely 
be added. If you wanted a file added to your dotfiles that isn't looked for in 
the script, open an issue.

[origin-issue]: https://github.com/anishathalye/dotbot/issues/22
[dotbot-repo]: https://github.com/anishathalye/dotbot
