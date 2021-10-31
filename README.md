# black-mypyc-index

A PEP 503 compliant index hosted on GitHub Pages designed to serve the
mypyc compiled psf/black wheels for testing.

To use this index, please pass
`--extra-index-url https://ichard26.github.io/black-mypyc-index/simple/`
to your pip install.

**Note:** I don't really know how this will interact with normal installs
of Black given the files from this index will end up cached by pip. From
what I know and have observed the cache for this index won't be used if
you don't specify it (via `--index-url` / `--extra-index-url`) so normal
installs should work, hopefully. Although if you do run into problems
try running the `cache purge` pip subcommand.[^1]

~ Richard (ichard26)

[^1]: yes there's no way to remove a specific package from pip's cache
      fully AFAIK
