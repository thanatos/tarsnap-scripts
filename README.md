# `tarsnap` scripts

This is a small set of scripts to drive `tarsnap`.

It takes one argument, a directory name to use for configuration and logging.
E.g., `my-home.tarsnap`. That directory should have the following files:

* `archive-name`; the name of the archive, no trailing newline.
  `printf 'my-archive' >archive-name`
* `target`: the directory to back up, no trailing newline.
  `printf '/home/me' >target
* `extra.conf`: extra configuration to give to `tarsnap`.
