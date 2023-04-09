
---
title: 2022-12-26 SiriKali works on Linux, macOS and Microsoft Windows Operating Systems
---



[[- InternetScrap]]
[[- ReadItLater]] [[- Article]]

# [SiriKali works on Linux, macOS and Microsoft Windows Operating Systems](https://mhogomchungu.github.io/sirikali/)

SiriKali is a Qt/C++ GUI application that manages ecryptfs, cryfs, encfs, gocryptfs, fscrypt and securefs based encrypted folders. These projects are compared [here.](https://nuetzlich.net/gocryptfs/comparison/) SiriKali can also connect to ssh servers using sshfs.

#### Supported Backends on Linux:

[Fscrypt](https://github.com/google/fscrypt), [Securefs](https://github.com/netheril96/securefs), [Ecryptfs](https://github.com/mhogomchungu/ecryptfs-simple), [Cryfs](https://www.cryfs.org/), [Encfs,](https://github.com/vgough/encfs) [Gocryptfs](https://nuetzlich.net/gocryptfs), [Sshfs](https://github.com/libfuse/sshfs) and [Cryptomator,](https://github.com/mhogomchungu/cli)

#### Supported Backends on Microsoft Windows:

[Cryfs](https://www.cryfs.org/), [Securefs](https://github.com/netheril96/securefs), [Encfs](https://github.com/mhogomchungu/encfs), [Sshfs](https://github.com/billziss-gh/sshfs-win) and [Cppcryptfs](https://github.com/bailey27/cppcryptfs)

Users of Securefs and Cppcryptfs should inform SiriKali of where Securefs and Cppcryptfs binaries are located on the system by setting the path at: `Menu->Settings->External Commands->Set Executables Search Path.`

If you are using the portable version, then a better place to put external executables is in the “local/bin” subfolder of the portable application folder.

#### Supported Backends on macOS:

[Securefs,](https://github.com/netheril96/securefs) [Cryfs,](https://www.cryfs.org/) [Encfs](https://github.com/vgough/encfs) and [Gocryptfs.](https://nuetzlich.net/gocryptfs)

Building SiriKali on macOS is currently a bit involving process and [the steps are documented here](https://github.com/mhogomchungu/sirikali/blob/master/MACOS_BUILD_INSTRUCTIONS).

#### Using SiriKali to connect to ssh server using sshfs:

Steps to setup SiriKali to connect to an ssh server are documented [here.](https://github.com/mhogomchungu/sirikali/wiki/Frequently-Asked-Questions#90-how-do-i-add-options-to-connect-to-an-ssh-server)

Encrypted container `folders` have an advantage over encrypted container `files` like the ones that are created by [zuluCrypt](http://mhogomchungu.github.io/zuluCrypt/),TrueCrypt,VeraCrypt among other projects that use file based encrypted containers.

SiriKali now has an extension system and it can support pretty much any fuse based backend and a small list of custom backends is [here.](https://github.com/mhogomchungu/sirikali/tree/master/custom%20backends)

#### Advantages are:

The encrypted container folder can freely grow and shrink as files are added,removed,grow or shrink. File based encrypted containers are limited to the size of the container and the size is set when the container is created and does not change to reflect the amount of data the container is hosting.

#### Disadvantages are:

The encrypted container folder does not hide the space usage of its contents and an adversary can derive meaning from space usage of the encrypted container folder. File based container hides the space utilization of the volume and the only thing an adversary can see is the fixed size of the container.

More advantages/disadvantages are discussed [here.](https://www.cryfs.org/comparison)

## FAQ

Most frequently asked questions are answered [here.](https://github.com/mhogomchungu/SiriKali/wiki/Frequently-Asked-Questions)

## DONATIONS

```
Donations are accepted through:
1. Bitcoin transfers.
2. Bank transfers.
3. Western Union.
4. Mobile money transfers through services like https://www.worldremit.com
   among others.

Send me an email through mhogomchungu at Gmail Dot coM for transfer details.
```

## Source download link.

Latest released version is 1.5.0 and its source code can be downloaded by clicking below link.

[SiriKali-1.5.0.tar.xz](https://github.com/mhogomchungu/sirikali/releases/download/1.5.0/SiriKali-1.5.0.tar.xz)

## Download links for Microsoft Windows Operating System.

The installer for Microsoft Windows operating system is [here](https://github.com/mhogomchungu/sirikali/releases/download/1.5.0/SiriKali-1.5.0.setup.exe).

The installer is not signed and expect to get a warning from windows saying the installer is from an unknown publisher. We recommend using the installer version.

A portable version is also found [here](https://github.com/mhogomchungu/sirikali/releases/download/1.5.0/SiriKali-1.5.0.exe.zip).

Packages are also available for [Winget](https://github.com/microsoft/winget-pkgs/tree/master/manifests/f/FrancisBanyikwa/SiriKali) and [Scoop](https://github.com/ScoopInstaller/Extras/blob/master/bucket/sirikali.json).

## Binary packages for Linux.

Check first if SiriKali is present in your distribution’s repositories and use that version if it is. `Fedora,opensuse,ubuntu and debian` users can install binary packages by following instructions on [this](http://software.opensuse.org//download.html?project=home%3Aobs_mhogomchungu&package=sirikali) link.

Gentoo users can get SiriKali from [holgersson overlay.](https://github.com/holgersson32644/holgersson-overlay)

Arch Linux users can get SiriKali from [AUR.](https://aur.archlinux.org/packages/sirikali/)

[![Mac Informer Editor's pick award](Mac%20Informer%20Editor's%20pick%20award.png)](http://macdownload.informer.com/sirikali/)

## Where did the name come from?

“SiriKali” name is a combination of two Swahili words, “siri” and “kali”.In Swahili, “Siri” means [“secret”](https://translate.google.com/#view=home&op=translate&sl=sw&tl=en&text=siri) and “kali” means [“severe”.](https://translate.google.com/#view=home&op=translate&sl=sw&tl=en&text=kali) “SiriKali” can therefore loosely be translated to “top secret”.

## Screenshots

[![](Screenshot_20190912_113741.png)](https://github.com/mhogomchungu/sirikali/raw/master/images/Screenshot_20190912_113741.png)

[![](Screenshot_20190912_113930.png)](https://github.com/mhogomchungu/sirikali/raw/master/images/Screenshot_20190912_113930.png)

[![](Screenshot_20190912_114512.png)](https://github.com/mhogomchungu/sirikali/raw/master/images/Screenshot_20190912_114512.png)

[![](Screenshot_20190912_114700.png)](https://github.com/mhogomchungu/sirikali/raw/master/images/Screenshot_20190912_114700.png)

```
Name: Francis Banyikwa
email: banyikwafb@gmail.com

gpg key finderpring: E3AF84691424AD00E099003502FC64E8DEBF43A8

The key can be retrieved with command: gpg --recv-keys 0x02FC64E8DEBF43A8

The key is below:

-----BEGIN PGP PUBLIC KEY BLOCK-----

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
9azeqex9
=L6yQ
-----END PGP PUBLIC KEY BLOCK-----
```

last update: Tue Mar 1 06:23:57 PM EAT 2022