This a sub-repo of [Neard project](https://github.com/crazy-max/neard) involving PHPUnit tool bundles.

## Installation

* Download and install [Neard](https://github.com/crazy-max/neard).
* If you already have installed Neard, stop it.
* Download [a PHPUnit bundle](#download) (check [compatibility table](#compatibility-table) first).
* Extract archive in `neard\tools\phpunit\`. Directory structure example :

```
[-] neard
 | [-] tools
 |  | [-] phpunit 
 |  |  | [-] phpunit4.8.24
 |  |     | neard.conf
 |  |  | [-] phpunit5.3.2
 |  |     | neard.conf
```

* Edit the `neard.conf` file and replace the key `phpunitVersion` with the correct version.
* Start Neard.

## Download

![](https://raw.github.com/crazy-max/neard-tool-phpunit/master/img/star-20160403.png) : Default bundle on Neard.

### 4.8

|                    | PHPUnit release date | Neard release | Neard compatibility | Download |
| -------------------|:--------------------:|:-------------:|:-------------------:|:--------:|
| **PHPUnit 4.8.24** ![](https://raw.github.com/crazy-max/neard-tool-phpunit/master/img/star-20160403.png) | 2016/03/14 | [r1](https://github.com/crazy-max/neard-tool-phpunit/releases/tag/r1) | >= 1.0.19 | [neard-phpunit-4.8.24-r1.7z](https://github.com/crazy-max/neard-tool-phpunit/releases/download/r1/neard-phpunit-4.8.24-r1.7z) |

### 5.3

|                    | PHPUnit release date | Neard release | Neard compatibility | Download |
| -------------------|:--------------------:|:-------------:|:-------------------:|:--------:|
| **PHPUnit 5.3.2**  | 2016/04/12 | [r1](https://github.com/crazy-max/neard-tool-phpunit/releases/tag/r1) | >= 1.0.19 | [neard-phpunit-5.3.2-r1.7z](https://github.com/crazy-max/neard-tool-phpunit/releases/download/r1/neard-phpunit-5.3.2-r1.7z) |

## Compatibility table

|               | PHPUnit 4.8.x  | PHPUnit 5.3.x |
| ------------- |:--------------:|:-------------:|
| **PHP 5.2.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ko-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ko-20151214.png) |
| **PHP 5.3.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) |
| **PHP 5.4.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) |
| **PHP 5.5.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) |
| **PHP 5.6.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) |
| **PHP 7.0.x** | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ko-20151214.png) | ![](https://raw.github.com/crazy-max/neard-bin-apache/master/img/ok-20151214.png) |

## Sources

* https://phpunit.de/

## Contribute

If you want to contribute to this bundle and create new bundles, you have to download [neard-dev](https://github.com/crazy-max/neard-dev) in the parent folder of the bundle.
Directory structure example :

```
[-] neard-dev
 | [-] build
 |  |  | build-commons.xml 
[-] neard-tool-phpunit
 |  | build.xml
```

To create a new bundle :
* Do not forget to increment the `build.release` in the `build.properties` file.
* If you want you can change the `build.path` (default `C:\neard-build`).
* Open a command prompt in your bundle folder and call the Ant target `release` : `ant release`.
* Upload your release on a file hosting system like [Sendspace](https://www.sendspace.com/).
* Create an [issue on Neard repository](https://github.com/crazy-max/neard/issues) to integrate your release.

## Issues

Issues must be reported on [Neard repository](https://github.com/crazy-max/neard/issues).<br />
Please read [Found a bug?](https://github.com/crazy-max/neard#found-a-bug) section before reporting an issue.
