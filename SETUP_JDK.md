
## JDK

### Setup OpenJDK 11

```sh
sudo apt install -y \
    software-properties-common \ 
    default-jdk
```

### Managing multiple Java Versions

```sh
sudo update-alternatives --config java
# also
sudo update-alternatives --config javac
```

### Setting the JAVA_HOME Environment Variable

#### OpenJDK 11 (AMD64)

```sh
echo 'JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"' >> /etc/environment
```