# MARRtino-autonomous-navigation

MARRtino Autonomous Navigation

Navigazione autonoma del robot MARRtino in tre diversi ambienti complessi attraverso Gazebo e RViz

Installazione pacchetti:


Per l'algoritmo di GMapping con la versione ROS Noetic:<br>
sudo apt-get install ros-noetic-gmapping

Per l'algoritmo AMCL<br>
sudo apt-get install ros-noetic-map-server<br>
sudo apt-get install ros-noetic-navigation

Per la guida teleoperata:<br>
git clone https //github.com/robotis-git/turtlebot3_msgs.git<br>
git clone https //github.com/robotis-git/turtlebot3_simulation.git<br>
git clone https //github.com/robotis-git/turtlebot3.git <br>



Esecuzione Algoritmo:


Eseguire in un terminale il comando:<br>
roscore

Per la navigazione autonoma nel primo ambiente eseguiamo i seguenti comandi:<br>

In un primo terminale:<br>
roslaunch marrtino2 maze.launch<br>
In un secondo terminale:<br>
roslaunch marrtino2 amcl_maze.launch<br>
In un terzo terminale:<br>
roslaunch marrtino2 marrtino_rviz.amcl.launch<br>

Per la navigazione autonoma nel secondo mondo eseguiamo i seguenti comandi:<br>
In un primo terminale:<br>
roslaunch marrtino2 maze2.launch<br>
In un secondo terminale:<br>
roslaunch marrtino2 amcl_maze2.launch<br>
In un terzo terminale:<br>
roslaunch marrtino2 marrtino_rviz.amcl.launch<br>


Per la navigazione autonoma nel terzo ambiente eseguiamo i seguenti comandi:<br>
In un primo terminale:<br>
roslaunch marrtino2 stanza.launch<br>
In un secondo terminale:<br>
roslaunch marrtino2 amcl_stanza.launch<br>
In un terzo terminale:<br>
roslaunch marrtino2 marrtino_rviz.amcl.launch<br>
