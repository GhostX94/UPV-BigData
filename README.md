# UPV-BigData
WorkShop


# COMMANDOS PARA INSTALAR SCALA

#  Requisitos
  1) Tener instalado java , preferentemente version 1.8.0
  2) Tener minimo 8 Ram
  3) Setear 2 Cores de CPU a la MVM
  4) Paciencia
  
  # INSTALAR JAVA
  sudo yum install java-1.8.0-openjdk.x86_64
  
  # SETEAR JAVA HOME Y JRE HOME
  
  sudo cp /etc/profile /etc/profile_backup      #Backup the profile file in order to prevent unintentional mistakes
echo 'export JAVA_HOME=/usr/lib/jvm/jre-1.8.0-openjdk' | sudo tee -a /etc/profile
echo 'export JRE_HOME=/usr/lib/jvm/jre' | sudo tee -a /etc/profile
source /etc/profile

# TESTING JAVA
echo $JAVA_HOME
echo $JRE_HOME

# DOWNLOAD AND INSTALL SCALA
wget http://downloads.lightbend.com/scala/2.11.8/scala-2.11.8.rpm
sudo yum install scala-2.11.8.rpm

Puedes verificar que se instaló exitosamente usando el comando : scala -version
viendo una salida similar a la siguiente:
# Output:
Scala code runner version 2.11.8 -- Copyright 2002-2016, LAMP/EPFL
