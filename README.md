# Let the kernel only swap if it is absolutely necessary using /etc/sysctl.d #

Sets vm.swappiness to the lowest possible value, which is 0. Experience has
shown, that in virtual machines have better performance when using this
setting.
## How to install `swappiness-lowest` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org stretch main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `swappiness-lowest`.

```
sudo apt-get install swappiness-lowest
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `swappiness-lowest` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`swappiness-lowest` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
