# Setup instructions

The following instructions will help you to get ready for [Imbue](http://www.imbue.es) fullstack path:

- Grab a text editor, ideally VSCode
- Install a package manager
- Pimp your Terminal
- Setup git and GitHub
- Install Node


## GitHub account

Have you signed up to GitHub? If not, [do it right away](https://github.com/join).

:point_right: **[Upload a picture](https://github.com/settings/profile)** and put your name correctly on your GitHub account. This is important as we'll use an internal dashboard with your avatars. Please do it **now**.


## Git

To install `git`, first open a terminal. To open a terminal, you can click on the Ubuntu Start button in the sidebar and type `Terminal`. Then click on the terminal icon.

Then copy this line with `Ctrl` + `C`:

```bash
sudo apt install -y git
```

:bulb: To **paste it in the terminal**, you need to use `Ctrl` + `Shift` + `V`.


## VS Code - Your text editor

A text editor is one of the most important tools of a developer.

The easiest way to install Visual Studio Code for Debian/Ubuntu based distributions is to download and install the .deb package (64-bit), either through the graphical software center if it's available, or through the command line with:

```bash
sudo apt install ./<file>.deb
```
To download the file you can go to the [VS Code downloads page](https://code.visualstudio.com/Download)

:point_up: This command will ask for your password with: `[sudo] password for <username>:`. Don't panick! Calmy type your password key by key. You won't have a visual feedback (like little `*`), that's **perfectly normal**, keep on typing. When you're done, hit `Enter` :muscle:.

```bash
sudo apt-get install apt-transport-https
sudo apt-get update
sudo apt-get install code # or code-insiders
```


## Oh-my-zsh - Fancy your Terminal

We will use the shell named `zsh` instead of `bash`, the default one.

```bash
sudo apt install -y zsh curl vim nodejs imagemagick jq
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
# it will ask for your session password
```

Be careful, those commands will ask you to type your password twice. At the end
your prompt should look like this:

<img src='https://imbueprogram.github.io/imbue-program-docs/images/ubuntu_oh_my_zsh.png'></img>

If it doesn't, **ask a mentor**.

To make this change stick, restart your laptop (or virtual machine):

```bash
sudo reboot
```


## GitHub

We need to generate SSH keys which are going to be used by GitHub and Heroku
to authenticate you. Think of it as a way to log in, but different from the
well known username/password couple. If you already generated keys
that you already use with other services, you can skip this step.

Open a terminal and type this, replacing the email with **yours** (the
same one you used to create your GitHub account). It will prompt
for information. Just press enter until it asks for a **passphrase**.

```bash
mkdir -p ~/.ssh && ssh-keygen -t ed25519 -o -a 100 -f ~/.ssh/id_ed25519 -C "TYPE_YOUR_EMAIL@HERE.com"
```

**NB:** when asked for a passphrase, put something you want (and that you'll remember),
it's a password to protect your private key stored on your hard drive. You'll type,
nothing will show up on the screen, **that's normal**. Just type the passphrase,
and when you're done, press `Enter`.

Then you need to give your **public** key to GitHub. Run:

```bash
cat ~/.ssh/id_ed25519.pub
```

It will prompt on the screen the content of the `id_ed25519.pub` file. Copy that text,
then go to [github.com/settings/ssh](https://github.com/settings/ssh). Click on
**Add SSH key**, fill in the Title with your computer name, and paste the **Key**.
Finish by clicking on the **Add key** green button.

To check that this step is completed, in the terminal run this. You will be
prompted a warning, type `yes` then `Enter`.

```bash
ssh -T git@github.com
```

If you see something like this, you're done!

```bash
# Hi --------! You've successfully authenticated, but GitHub does not provide shell access
```

If it does not work, try running this before trying again the `ssh -T` command:

```bash
ssh-add ~/.ssh/id_ed25519
```

Don't be in a rush, take time to [read this article](http://sebastien.saunier.me/blog/2015/05/10/github-public-key-authentication.html) to get a better
understanding of what those keys are used for.



## Installing Node 

Node.js package is available in the LTS release and the current release. It’s your choice to select which version you want to install on the system as per your requirements. Let’s add the PPA to your system to install Nodejs on Ubuntu.

Use Current Release: At te last update of this tutorial, Node.js 13 is the current Node.js release available.
```bash
curl -sL https://deb.nodesource.com/setup_13.x | sudo -E bash -
```

You can successfully add Node.js PPA to the Ubuntu system. Now execute the below command install Node on and Ubuntu using apt-get. This will also install NPM with node.js. This command also installs many other dependent packages on your system.


```bash
sudo apt-get install nodejs
```


After installing node.js verify and check the installed version. You can find more details about current version on node.js official website.

```bash
node -v 
````

v13.3.0

## Installing Docker

If you have any problem, please refer to the [docker ubuntu installation page](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

First we are going to clear up the old versions
```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```

Update the apt package index.


```bash
 sudo apt-get update
```

Install the latest version of Docker Engine - Community and containerd, or go to the next step to install a specific version:

To install a specific version of Docker Engine - Community, list the available versions in the repo, then select and install:

a. List the versions available in your repo:

```bash
 apt-cache madison docker-ce
```

b. Install a specific version using the version string from the second column, for example, 5:18.09.1~3-0~ubuntu-xenial.

```bash
sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING> containerd.io
```

Verify that Docker Engine - Community is installed correctly by running the hello-world image.


```bash
sudo docker run hello-world
```


## Mongo Docker Image

In a few weeks, we'll talk about SQL and Databases and you'll need something called MongoDB,
an open-source robust and production-ready database. Let's download it now.

The simplest solution to download our image is to execute the following:

```bash
docker pull mongo
```
With the image available to us, we need to deploy it. In its simplest form, and what is outlined in the Docker Hub documentation, we can execute the following command:

```
docker run --name mongodb mongo:4.0.4
```

This command works, but there are potentially a few problems. What we’re doing is we are running a container and naming it mongodb. We aren’t running it in the background and if we wanted to connect to it, we’d have to do it from another container instance. In other words, we wouldn’t be able to connect to it from our host computer or server.

Instead, what we could do is the following:

```bash
docker run -d -p 27017-27019:27017-27019 --name mongodb mongo:4.0.4
```

## Ubuntu inotify

Ubuntu is always tracking changes in your folders, and to do this it uses inotify.
By default the Ubuntu limit is set to 8192 files monitored.

As programming involves a lot of files, we need to raise this limit.
In your terminal run:

```bash
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```

## Slack

[Install Slack for Linux (beta)](https://get.slack.help/hc/en-us/articles/212924728-Slack-for-Linux-beta-).

Launch the app and sign in to `imbueprogram` organization.

Make sure you upload a picture there.

You can also sign in to Slack on your iPhone or Android device!

The idea is that you'll have Slack open all day, so that you can share useful links / ask for help / decide where to go to lunch / etc.

Enjoy your ride with Imbue :)

