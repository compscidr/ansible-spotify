# Changelog

## 0.0.5
* Updated expired Spotify GPG signing key from C85668DF69375001 to 5384CE82BA52C83A
* Added automatic detection and removal of the old expired key on existing installations

## 0.0.4
* Fixed the apt source to remove the signed-by

## 0.0.3
* Switched back to .list format because otherwise Spotify will update and create a .list file which leads to duplicate sources when we have a .sources file present.

## 0.0.2
* Updated to use DEB822 format with deb822_repository module.

## 0.0.1
* First version.