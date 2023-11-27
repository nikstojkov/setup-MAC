# setup-MAC
---

### Homebrew package manager

run in termnial
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

allows commands such as `brew install wget`

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

