Homebrew
=====

What is [Homebrew](http://brew.sh/)?


## Install from a local archive

1. Download the archive manually `wget http://xxx.com/package.tar.gz`
2. Move the archive to cache directory `mv ~/Downloads/package.tar.gz$(brew --cache)`
3. Rerun `brew install package`

## Manage startups

Take `mongodb` as an example

```
$ brew services list | grep mongodb
$ brew services start mongodb
$ brew services stop mongodb
```