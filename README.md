# Solus-moriel5-Repo
Here I shall upload package.ymls of several packages I use, though there is no guarantee of me being active.

## Adding the Repository

TBD

## Disclaimer :notebook:
 
**These packages are not official**, they are neither supported nor endorsed by the official *Solus* devs. Do not ask for help in *Solus's* help forum, instead create an [issue](https://github.com/moriel5/Solus-moriel5-repo/issues/new).

If something here gets accepted into the official *Solus* repository, it will eventually be removed from here.

## Install

You will need to set up an enviroment for packaging software for Solus (please use it to help the main repository).
Instructions can be found over at the Solus Help Center, under *Package Management*: https://getsol.us/help-center/home/

In your preferred location, follow the following steps (replace "<package-name>" with the name of the software):
```bash
mkdir <package-name>
cd <package-name>
echo "include ../Makefile.common" > Makefile
```
Then move the downloaded package.yml (or alternatively, just copy it's content from the repository into a new text file named "package.yml") over to <package-name> and finally:
```bash
make
sudo eopkg install *.eopkg
(optional, to remove the installation file:) rm *.eopkg
```

## Packages List

| Package Name | Version | Last Updated | Notes |
|-|-|-|-|
| gnome-sound-recorder | 40.0 | 5/8/2022 | Renamed to `gnome-sound-recorder-fix` since this is a dropped package |
| skypeforlinux | 8.83.0.408 | 5/9/2022 | Duplicate dependencies, not influental, however I would like feedback on how to clean this|
| skypeforlinux-preview | 8.84.76.301 | 5/9/2022 | Duplicate dependencies, not influental, however I would like feedback on how to clean this|
