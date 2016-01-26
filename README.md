# idev-basebox-jessie64

This repository hosts the build for https://atlas.hashicorp.com/kiesel/boxes/idev-basebox-jessie64

It is based on the *official* Debian build whose sources can be acquired here: https://wiki.debian.org/Teams/Cloud/VagrantBaseBoxes, but it is in no way related to the Debian project.

The primary feature this box has over the official one is that the root partition is 100GB instead of just 10. Resizing **after** a box has been built is a PITA, so we try to do it before the build:)

## Building it

### Manually

```shell
$ packer build idev-basebox-jessie64.json
[... now wait a looong time ...]
```

Use the Virtualbox GUI to be sure your build actually does something.

### Via GitHub

Supposedly, pushes to this repo should initiate automated builds at [HashiCorp Atlas](https://atlas.hashicorp.com/kiesel/build-configurations/idev-basebox-jessie64)

## Direct Download

	vagrant init kiesel/idev-basebox-jessie64

## Credits

  Many thanks to [Mitchell Hashimoto](https://github.com/mitchellh/) for his awesome work on [Packer](https://github.com/mitchellh/packer) and [Vagrant](https://github.com/mitchellh/vagrant), [![Tech-Angels](http://media.tumblr.com/tumblr_m5ay3bQiER1qa44ov.png)](http://www.tech-angels.com), the Debian Team