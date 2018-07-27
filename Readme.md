This is a folder structure which includes vagrant files for major versions of IE.

## How to use?

Install vagrant and virtual box if you do not already have it. (note: hyper-v does not like virtualbox disable the hyper-v service if you want both installed).

Windows:

```
choco install virtualbox -y
choco install vagrant -y

```

Macos:

```
brew cask install virtualbox
brew cask install vagrant
```

cd to the root of the git repo

you can then run `vagrant up IE10-Win7`

you can also launch multiple versions `vagrant up edge-Win10 IE10-Win7 IE10-Win8 IE9-Win7`

Avalible Machines:

* IE10-Win7
* IE10-Win8
* IE11-Win7
* IE11-Win8.1
* IE8-Win7
* IE9-Win7
* edge-Win10


Inspired by [another project](https://github.com/markhuber/modern-ie-vagrant) but uses boxes in the regular vagrant cloud.
