# Android Environment Setup

About

This repository is intended to share the way I like to configure my development environment to work with Android applications.

For this, I performed the steps on a computer with the Mac OS X system, however the available links will possibly have instructions to perform the steps on other platforms as well!

## Summary

1. [Install Android Studio](#install-android-studio)
2. [Install Java](#install-java)
3. [Install Homebrew](#install-homebrew)
4. [Install iTerm2](#install-iterm2)
5. [Install zsh](#install-zsh)
6. [Install oh-my-zsh](#install-oh-my-zsh)
7. [Configure your .zshrc file](#configure-your-zshrc-file)
8. [Install NVM](#install-nvm)
8. [Configure GitHub credentials](#configure-github-credentials)
9. [Clone a test project](#clone-a-test-project)
10. [Open and run the test project](#open-and-run-the-test-project)
10. [References](#references)


## Install Android Studio
1. [Download android studio]
2. Install android studio

## Install Java
1. Go to the [Previous Java releases] page and select the java versions you will need in your context. In my case, I'm going to download versions [Java SE Development Kit 8u251] and [Java SE Development Kit 11.0.2].

## Install Homebrew
1. Open the terminal
2. Paste the following command and [ENTER]
```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
## Install iTerm2
1. Open the terminal
2. Paste the following command and [ENTER]
```sh
brew install iterm2
```

## Install zsh
1. Open the terminal
2. Paste the following command and [ENTER]
```sh
brew install zsh
```

## Install oh-my-zsh
1. Open the terminal
2. Paste the following command and [ENTER]
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Configure your .zshrc file
1. Open the terminal
2. Copy the commands below respectively and [ENTER] after each of them

```sh
cd
```

```sh
open .
```
3. Now download this [.zshrc file] and copy it to the open folder.
4. Fill in the following fields in the [.zshrc file] file with your github data
```sh
alias gitUserName="git config user.name \"Your Name\""
alias gitUserEmail="git config user.email \"@gmail.com\""
```

## Install NVM
1. Open the iterm
2. Copy the commands below respectively and [ENTER] after each of them
```sh
brew update
```
```sh
 brew install nvm 
```
```sh
 mkdir ~/.nvm 
```

## Configure GitHub credentials

Now that your [Iterm] is configured, we can start using it instead of the standard terminal.

1. Open the iterm
2. Copy the commands below respectively and [ENTER] after each of them
```sh
 git config --global user.name "Your Name"
```
```sh
 git config --global user.email "your_email@example.com"
```

3. Now you will need to follow the documentation available on github for [Generating a new SSH key and adding it to the ssh-agent] and [Adding a new SSH key to your GitHub account].

## Clone a test project 

After setting up your ssh keys, you should be able to clone a test repository to build an Android project. To do this, run the following command in your iterm:
```sh
 git clone git@github.com:knludi/DiceRoller.git
```
If there is an error at this stage, you can search for an answer on Google, or contact me by sending the error message, and I can try to help you in some way!

## Open and run the test project

Now that the initial configurations are done, let's test them by building a pre-existing project, which was downloaded from git in the previous step.

1. Open Android Studio, and you should see a screen like this:

<div align="center">
<img align="center" alt="Tip time app running" height="500" src="https://github.com/knludi/android-environment-setup/blob/master/README/home-android-studio.png">
</div>

2. Open the project you downloaded earlier: 

<div align="center">
<img align="center" alt="Tip time app running" height="500" src="https://github.com/knludi/android-environment-setup/blob/master/README/open-project.png">
</div>

3. [Create a virtual device] following the guideline;

4. Once you have a device created, use the play icon to build and view the app in the emulator:

<div align="center">
<img align="center" alt="Tip time app running" height="50" src="https://github.com/knludi/android-environment-setup/blob/master/README/play-app.png">
</div>

5. Wait for the app to build, this may take a few minutes. At the end you should see a screen similar to this:

<div align="center">
<img align="center" alt="Tip time app running" height="500" src="https://github.com/knludi/android-environment-setup/blob/master/README/environment-working.png">
</div>

6. Congratulations!! you have a completely configured android environment, and now you can start building your apps!🥳 


## References
- [Dillinger | The Last Markdown Editor, Ever](https://dillinger.io/)
- [Androidfor Developers](https://developer.android.com/)
- [Text to kebab-case (dash-case) Online Conterter](https://textedit.tools/kebabcase)



   [download android studio]: <https://developer.android.com/studio>
   [.zshrc file]: <https://github.com/knludi/android-environment-setup/blob/master/.zshrc>
   [Previous Java releases]: <https://www.oracle.com/java/technologies/downloads/archive/>
   [Create a virtual device]: <https://developer.android.com/studio/run/managing-avds>
   [Java SE Development Kit 11.0.2]: <https://download.oracle.com/otn/java/jdk/11.0.2+9/f51449fcd52f4d52b93a989c5c56ed3c/jdk-11.0.2_osx-x64_bin.dmg>
   [Java SE Development Kit 8u251]: <https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html#license-lightbox>
   [Iterm]: <https://iterm2.com/>
   [Generating a new SSH key and adding it to the ssh-agent]: <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>
   [Adding a new SSH key to your GitHub account]: <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>
 

