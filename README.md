TechStruck
================

Tech Struck is a discord server where developers, designers and just about everyone struck with curiosity on tech unite together as a community!

**Links**
 - [TechStruck Discord](https://discord.gg/6BxbAfedAP)
 - [TechStruck Invite](https://discord.com/api/oauth2/authorize?client_id=790474885804982293&permissions=0&scope=bot%20applications.commands)
 - [TechStruck Github repo](https://github.com/FalseDev/Tech-Struck)

### Running YAGPDB yourself

Running this bot may seem challenging, and that's because I don't have time to make it easy to run for everyone, for the most part, it should run fine after the initial work has been done. Please view [this page](https://docs.yagpdb.xyz/development/self-hosting-with-docker) for more information.

#### Updating
Updating after v1 should migrate schemas automatically, but you should always take backups beforehand if things go wrong.

I will put breaking changes in the breaking_changes.md file, which you should always read before updating.

#### There's 2 ways of running this bot

1. Using Docker
2. Standalone

**I will not help with basic problems or how to do unrelated things (how to run it on startup for example), use Google, if those well written tutorials and articles confuse you, how the hell is a guy with English as a second language gonna be any better?**

(There's still a lot of contributing you can do without this though, such as writing docs, fixing my horrible typos and so on)

#### General Discord bot setup

**Downloading:**
```
git clone https://github.com/FalseDev/Tech-Struck
cd Tech-Struck/
chmod +x bot.py
```


**Requirements:**

```
cd Tech-Struck/
sudo python3 -m pip install -r requirements.txt
```

OR

```
cd Tech-Struck/
sudo pip3 install -r requirements.txt
```

### Plugins

**Standard plugins:**

* Common
* Thank
* Github
* Stackexchange
* CodeExec
* RTFM
* And More!

**Planned plugins**

[See the Issues Tab for more](https://github.com/FalseDev/Tech-Struck/issues)

### Core packages:

- Web: The core web server package, in charge of authentication.
- Bot: Core bot package, delegates events to plugins.
- Common: Handles all the common stuff between web and bot (config, discord session, redis pool etc).
- Feeds: Handles all feeds, personally I like to run each feed as its own service, that way I can start and stop individual feeds without taking everything down.
- Commands: Handles all commands.

Currently, YAGPDB builds everything into one executable and you run the bot with the -bot switch, the web server with the -web switch and so on (see -h for help).

### Contributing new features

You can send a pull request or open an issue to contribute.

**If you need any help finding things in the source or have any other questions, don't be afraid of messaging me (FalseDev).**
