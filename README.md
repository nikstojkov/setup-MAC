# setup-MAC

## Software requirements
### 1. Java (java version "1.8.0_92" or higher)
### 2. MariaDB (10.5)
### 3. Maven (lastest)
### 4. Eclipse IDE (latest) / Intellij IDEA (latest)
### 5. Python 3 (MUST BE 3)

---

### Homebrew package manager

run in termnial
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

allows commands such as `brew install wget' 

---

### Java (java version "1.8.0_92" or higher)

`brew install java`

create hello.java on desktop

```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

run `javac hello.java`

if you get an error, visit [Oracle downloads](https://www.oracle.com/uk/java/technologies/downloads/#java21) and download appropriate JDK Dev kit and try again.

---

### MariaDB

`brew install mariadb@10.5`

---

### Maven

`brew install maven`

---

### Eclipse 

visit [Eclipse](https://www.eclipse.org/downloads/packages/installer) and download appropirate installer. 

---

### Python 3

`brew install pyenv`
pyenv allows you to switch between any version of python once installed

`pyenv install 3.9.2 `
note: '3.9.2' can be substituted for any version as per requirements

