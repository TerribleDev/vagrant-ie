This is a folder structure which includes vagrant files for IE9+ on every platform it is offered..

## How to use?

Install vagrant and virtual box if you do not already have it. (note: hyper-v does not like virtualbox disable the hyper-v service if you want both installed).

```
choco install virtualbox -y
choco install vagrant -y

```

cd to `	virtualbox/$ieVersion/win$Version`

and then run `vagrant up` the box image will be downloaded from the cloud (if its not already) and then the vm will be booted in virtualbox. Username and password both vagrant

for example if you want IE10 on windows 7 you would cd to virtualbox/ie10/win7 and then run vagrant init

```
cd virtualbox/ie10/win7
vagrant init

```