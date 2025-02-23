# i2c-gpio-custom

DKMS Module

## Setup

Install environment

```shell
sudo apt install build-essential git linux-headers-$(uname -r)
```

Clone the repository

```shell
git clone git@github.com:LeoWare/i2c-gpio-custom.git
```

Copy the source into the correct directory

```shell
sudo cp -r i2c-gpio-custom /usr/src/i2c-gpio-custom-0.1.1
```

Add the module to DKMS
```shell
sudo dkms add -m i2c-gpio-custom/0.1.1
```

Build the module
```shell
sudo dkms build -m i2c-gpio-custom/0.1.1
```

Install the module
```shell
sudo dkms install -m i2c-gpio-custom/0.1.1
```

