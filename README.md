# MARRtino-autonomous-navigation

MARRtino Autonomous Navigation

Navigazione autonoma del robot MARRtino in tre diversi ambienti complessi attraverso Gazebo e RViz

Installazione pacchetti:


Per l'algoritmo di GMapping con la versione ROS Noetic:
sudo apt-get install ros-noetic-gmapping

Per l'algoritmo AMCL
sudo apt-get install ros-noetic-map-server
sudo apt-get install ros-noetic-navigation

Per la guida teleoperata:
git clone https //github.com/robotis-git/turtlebot3_msgs.git
git clone https //github.com/robotis-git/turtlebot3_simulation.git
git clone https //github.com/robotis-git/turtlebot3.git 



Esecuzione Algoritmo:


Eseguire in un terminale il comando:
roscore

Per la navigazione autonoma nel primo ambiente eseguiamo i seguenti comandi:

In un primo terminale:
roslaunch marrtino2 maze.launch
In un secondo terminale:
roslaunch marrtino2 amcl_maze.launch
In un terzo terminale:
roslaunch marrtino2 marrtino_rviz.amcl.launch

Per la navigazione autonoma nel secondo mondo eseguiamo i seguenti comandi:
In un primo terminale:
roslaunch marrtino2 maze2.launch
In un secondo terminale:
roslaunch marrtino2 amcl_maze2.launch
In un terzo terminale:
roslaunch marrtino2 marrtino_rviz.amcl.launch


Per la navigazione autonoma nel terzo ambiente eseguiamo i seguenti comandi:
In un primo terminale:
roslaunch marrtino2 stanza.launch
In un secondo terminale:
roslaunch marrtino2 amcl_stanza.launch
In un terzo terminale:
roslaunch marrtino2 marrtino_rviz.amcl.launch
