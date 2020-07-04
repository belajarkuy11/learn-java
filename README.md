# learn-java
1. download jdk file

from open-jdk ==> https://jdk.java.net/java-se-ri/8-MR3

from oracle ==> https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html



2. Open a terminal using Ctrl+Alt+T key combination

3. Change a current directory to ~/<dir>
cd ~/<dir> ex:cd "/opt/latihan-java/open-jdk/"

4. Unpack the tarball
tar zxvf <name-of-jdk>.tar.gz


5. Inform Ubuntu to use this JDK

from open-jdk
sudo update-alternatives --install "/usr/bin/java" "java" "/opt/latihan-java/open-jdk/java-se-8u41-ri/bin/java" 1
sudo update-alternatives --install "/usr/bin/javac" "javac" "/opt/latihan-java/open-jdk/java-se-8u41-ri/bin/javac" 1

6. setting PTH JDK
vi ~/.bashrc

JAVA_HOME="/opt/latihan-jdk/open-jdk/java-se-8u41-ri"
export JAVA_HOME
export PATH=$PATH:$JAVA_HOME/bin
