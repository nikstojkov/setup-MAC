# setup-MAC
---

### Homebrew



[Homebrew](http://brew.sh/) package manager.

Open terminal and run:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

This will ask for your confirmation (hit `Enter`) and your **macOS user account password** (the one you use to [log in](https://support.apple.com/en-gb/HT202860) when you reboot your Macbook).

:warning: When you type your password, nothing will show up on the screen, **that's normal**. This is a security feature to mask not only your password as a whole but also its length. Just type your password and when you're done, press `Enter`.

:warning: If you see this warning :point_down:, run the two commands in the `Next steps` section to add Homebrew to your PATH:

![macOS Homebrew installation warning](macos_homebrew_warning.png)

```bash
# Only execute these commands if you saw this warning
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

If you already have Homebrew, it will tell you so.

run:

```bash
brew update
```

If you get a `/usr/local must be writable` error, run:

```bash
sudo chown -R $USER:admin /usr/local
brew update
```

[Useful guide](https://nelson.cloud/how-to-install-older-versions-of-homebrew-packages/) on how to install older versions of homebrew packages.

---

## Software requirements

### 1. Java (java version "1.8.0_92" or higher)

`brew install java`



create hello.java on desktop

`cd ~/Desktop`

`touch hello.java` and open with textedit.app or your favorite note editor.



inside hello.java
```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
save the file.

run `javac hello.java`

if you get an error, visit [Oracle downloads](https://www.oracle.com/uk/java/technologies/downloads/#java21) and download appropriate JDK Dev kit and try to complie again.

run `java hello.java` and 'Hello, World!' should print in the termnial 

---

### 2. MariaDB (10.5)

if you have had mysql, run `sudo rm -rf /usr/local/var/mysql/` before running any installs as it will cause no end of errors (still researching why)

`brew install mariadb@10.5`

run `brew services start mariadb@10.5` to verify

run `brew services stop mariadb@10/5` to stop

---

### 3. Maven (lastest)

`brew install maven`
check version 
`mvn -v`

---

### 4. Eclipse IDE (latest) / Intellij IDEA (latest)

visit [Eclipse](https://www.eclipse.org/downloads/packages/installer) and download appropirate installer. 

---

### 5. Python 3 (MUST BE 3)


`brew install pyenv`
pyenv allows you to switch between any version of python once installed

`pyenv install 3.9.2 `
note: '3.9.2' can be substituted for any version as per requirements

check version
`pyenv versions`

run
`pyenv global 3.9.2`

