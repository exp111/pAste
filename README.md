## DETECTED

Since 06.06.2017 all Aimtux forks and Aimtux itself are detected. I wouldnt recommend using this as it brings some risks (untrusted bans).

## What is pAste?

pAste is a fork of Aimtux/Antario with more features added. 
Aimtux is a fully featured internal hack for *CounterStrike : Global Offensive* written in C++.

I will add my own features here and maybe add stuff from other forks as Antario was discontinued.

If you find a bug or want to add something just make a pull request.

### What is different?
**From AimTux:**
- New Aimbot Features (Closest Bone, Adaptive FOV, Hitscan (still WIP), Velocity Prediction)
- Legit mode Toggle
- Walkbot
- Knife/Zeus Bot
- Custom Watermark
- Bugfixes & Updates

**From Antario:**
- Really bad memes (Found in an **a e s t h e t i c** new menu in the main menu bar)
- Different 'Menu Themes'
- Fixed some bugs
- Slightly different menu (Can still change in the future)
- Still maintained
- New features when I have an idea

## Compiling

**Note:** _Do NOT download or compile as the root user_

#### Download the dependencies required to build pAste:

__Ubuntu-Based / Debian:__
```bash
sudo apt-get install cmake g++ gdb git libsdl2-dev zlib1g-dev
```

If you're having problems compiling make sure you've got the latest version of `g++`.

[How to update g++](https://github.com/AimTuxOfficial/AimTux/wiki/Updating-your-compiler)


__Arch:__
```bash
sudo pacman -S base-devel cmake gdb git sdl2
```
__Fedora:__
```bash
sudo dnf install cmake gcc-c++ gdb git libstdc++-static mesa-libGL-devel SDL2-devel zlib-devel
```

__Gentoo:__
```bash
sudo emerge cmake dev-vcs/git gdb libsdl2 mesa
```


#### Download Antario:

```bash
git clone --recursive https://github.com/exp111/pAste
```

```bash
cd pAste
```


#### Compile with build script
 
You can build easily with the included build script.

```bash
./build
```

## Injecting

First of all, make sure CSGO is open, it doesn't matter whether you're in game or not.

Navigate to the directory where pAste was built if you haven't ready.

```bash
cd pAste
```

Now, you can inject the hack with the `load` script

```bash
./load
```

You might be prompted to enter in your password, this is because the injection script requires root access.

You should see a lot of text being printed out, most of which is not important,

If the injection was successfull you'll see a message at the bottom saying `Successfully injected!`, however, if the message says `Injection failed`, then you've most likely done something wrong.

Now, go back into csgo, if you're in the main menu of the game you should see the pAste banner in the top left.

## Using the hack

Now that pAste has been injected into the game, press <kbd>Insert</kbd> on your keyboard to open the hack menu (<kbd>ALT</kbd>+<kbd>I</kbd> if you're using a laptop).

If you want to change skins, create and load configs or open the player list, you can find those buttons at the top of the screen.

## Unloading the hack

If you wish to unload the hack from the game, you can do so by entering the command:

```bash
./uload
```

## Updating pAste

We add and improve and fix things almost every day with pAste. We don't have a fixed release schedule, we just add things to it when they're ready. Because of this, pAste will need to update a lot.

If you don't update once a day then we recommend at LEAST update once a week, and ALWAYS update after a CSGO update, just to make sure we fix anything that's broken.

We provide a script included in the pAste folder that updates pAste for you. To use it, just run:

```bash
./update
```

And it will download and compile without any effort. Once it's done, happy hacking!


## Configs

Configs are stored in a hidden directory in your home folder. Specifically 

```bash
~/.config/pAste
```

Each `config.json` is stored in a seperately named folder (The name you see in-game, in the config window). 

To add a config, create a folder inside of the `~/.config/pAste` folder with a name of your choice, and paste the `config.json` inside of that folder.

To see hidden folders inside your home folder, press <kbd>CTRL</kbd>+<kbd>H</kbd> when using a file manager.

## Grenade Configs

```bash
~/.config/pAsteGH
```

Each `config.json` is stored in the folder named after them map name.

To add a config, copy the folder containing it to `~/.config/pAsteGH`
## Contributing to pAste

If you wish to contribute code to this opensource project, please keep some things mind before creating a *pull request*:
 - Make sure you're using the correct [code style](https://github.com/AimTuxOfficial/AimTux/wiki/Code-Style).
 - Make sure your commits are clean and straight forward ( no junk commits )
 - Explain what you've done in your pull request.


## Screenshots

![aimbot](http://i.imgur.com/MLaD9z9.jpg)
![menu](http://i.imgur.com/hHMJ8nH.jpg)
![esp](http://i.imgur.com/rLxmdFk.jpg)

## Credits
Special thanks to [@aixxe](http://www.github.com/aixxe/) ([aixxe.net](http://www.aixxe.net)) for the skin changer and with the initial project, as well as helping this project with source code (Available on [@aixxe's](http://www.github.com/aixxe/) github page.)

This project was also originally based upon Atex's [Linux Basehook](http://unknowncheats.me/forum/counterstrike-global-offensive/181878-linux-basehook.html).

Thanks to @McSwaggens(http://www.github.com/McSwaggens/) and @Wando1423(http://www.github.com/Wando1423/) for creating Aimtux/Antario and adding new features.
