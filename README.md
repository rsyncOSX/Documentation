# RsyncOSX

## The RsyncOSX code

The [code](https://github.com/rsyncOSX/RsyncOSX) is **not** example of neither writing _decent Swift code_, _OO-development_ or _applying the MVC-pattern_. It all started as a project to learn the _basics_ about Swift and Xcode. And I am still learning, every day. I am not a professional developer, this is for fun only.

**May 2017**: What is my experience after about a year into my Swift project? Writing code is fun and addicting. But I experience that parts of the code I am writing is a kind of "brute force". From time to time I am reading blogs and other resources about coding in Swift. Some ideas I do pick up, some I don´t understand and others again are like this is how I should have done it. But I am not a professional programmer, my project is for fun only.

But, I need a backup tool based upon rsync. I will continue to refactor code whenever I have got some ideas reading other code, and I will continue adding minor enhancements to RsyncOSX (at least for some time). That is it...

### Installing and important info

Before installing and using RsyncOSX there are some important information to read and understand. The _first_ document is how to get and install RsyncOSX. The _second_ document is some information what RsyncOSX is and how to use the application. Please read the _second_ document before using the application.

> - Getting and installing (#1) [RsyncOSX](docs/RsyncOSX.md).
> - Important (#2) [information](docs/HowtoUseRsyncOSX.md) about what RsyncOSX is.

### Using RsyncOSX

The following are documents about using RsyncOSX.

> - Short [intro](docs/Intro.md) to RsyncOSX
> - Adding [configurations](docs/AddConfigurations.md) (backup and restore).
> - Executing of [single tasks](docs/SingleTask.md) (configurations).
> - Executing of [batch tasks](docs/BatchTask.md).
> - Scheduling of [tasks](docs/ScheduleTasks.md).
> - Restore of [single files or catalogs](docs/CopySingleFiles.md).
> - [Logging](docs/Logging.md) execution of tasks.
> 	- There is a minor issue regarding logging, see [Logging](docs/Logging.md) for details
> - Some info about [user configuration](docs/UserConfiguration.md).

### Passwordless logins

Using RsyncOSX for backup to remote servers requiere to setup ssh passwordless login. What is ssh passwordless login? By using ssh private and public keypair, login to remote servers without password is enabled.

> - How to enable [passwordless logins](docs/PasswordlessLogin.md).
> - Or use RsyncOSX to assist setting up [passwordless](docs/ssh.md) logins.

### Parameters to rsync

There are a couple of other important information about using RsyncOSX (and rsync):

> - Parameters to [rsync](docs/Parameters.md).
> - Some more info about standard [parameters to rsync](docs/RsyncParameters.md).

### My NAS setup

I have setup up my own [NAS](docs/DIYNAS.md). My NAS SW is now FreeNAS Corral. I am doing backups by using RsyncOSX and sharing out disk by AFP and SMB.


## Changelog

The RsyncOSX [changelog](docs/Changelog.md).

## Rsync

The default version of `rsync` in macOS is old (version 2.6.9, [protocol](https://rsync.samba.org/how-rsync-works.html) version 29). Version [2.6.9](https://download.samba.org/pub/rsync/src/rsync-2.6.9-NEWS) was released in nov 2006. The current release of rsync is version [3.1.2](https://download.samba.org/pub/rsync/src/rsync-3.1.2-NEWS) protocol 31 released 21 Dec 2015. There are at least two options to get and install the current version of rsync for use in RsyncOSX:

- install Xcode and download the rsync [source](https://rsync.samba.org/) from rsync.samba.org
	- required tools are `gcc` and `make` which are part of Xcode command line tool (you might be able to install Xcode command line tool only by downloading the tools from [Apple Developer page](https://developer.apple.com/))
	- untar the source archive and use `make` to compile and install, rsync compiles without any issues on macOS
- install [homebrew](https://en.wikipedia.org/wiki/Homebrew_(package_management_software)) and then install rsync as part of homebrew

In RsyncOSX select [RsyncOSX configuration](docs/UserConfiguration.md) and set path for optional version of rsync.

## YouTube

I have uploaded a short (about 5 minutes) [YouTube demo of RsyncOSX](https://www.youtube.com/watch?v=ty1r7yvgExo) : "Downloading RsyncOSX, installing, first time configuration and using RsyncOSX for the first time. Backup (as demo) of about 120 MB of data and 4000 files to a VirtualBox FreeBSD machine."

## MacUpdate and Softpedia

RsyncOSX is also released on [MacUpdate](https://www.macupdate.com/app/mac/56516/rsyncosx) and linked for download on [Softpedia](http://mac.softpedia.com/get/Internet-Utilities/RsyncOSX.shtml) as well. The application is downloaded about 8300 times from MacUpdate and 2000 times from Softpedia (all versions, May 2017). RsyncOSX does also inform users about new releases and link to download new version.

To be honest, I have **no idea** how many users of RsyncOSX there are. And I am very happy that some users find it useful.

## Other documents

There are a few other documents in context of RsyncOSX. To enable remote storage of backups please read how to [enable passwordless logins](docs/PasswordlessLogin.md). Rsync utilises parameters. RsyncOSX can send extra (set by user) parameters to rsync.


> - My [DIY NAS](docs/DIYNAS.md).
> - The [idea](docs/Idea.md) behind RsyncOSX.
