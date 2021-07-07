# Autonomous-vehicles-using-IoT-enabled-AI-technologies
# Introduction 
In this project, we aspire to develop a city that relies on artificial intelligence (AI) technologies to deal with self-driving vehicles and their importance to humans and provide the best solutions with easy effort and reduce the financial cost through the development of sensors. And linking them with self-driving vehicles to facilitate transportation, choose the best roads, and avoid congestion and dangerous problems.

# Problem Definition
Various methodological techniques have been developed to discover and predict the best paths for autonomous vehicles through advanced sensor processing, machine learning, and artificial intelligence algorithms. The purpose of this project is to first investigate basic smart algorithms that are being applied to discover the best approaches for autonomous and autonomous vehicles. Then, using advanced technologies to accurately detect traffic congestion, choose the appropriate road, and have less time while driving. Although many survey articles have been written to address this issue, according to our limited knowledge, none of them have built a hybrid system with cameras and sensors to study the road and provide the best solutions. There is a recent investigative article to detect and predict accidents before they happen, but that study indicated that there are still many improvements required in this area. Accordingly, in this project, we will also develop an integrated e-sharing technology for predicting best methods and incidents before they happen that supports AI and the Internet of Things. 


# carla 
is Open-source simulator for autonomous driving research [https://carla.org/]. CARLA has been developed from the ground up to support development, training, and validation of autonomous driving systems. In addition to open-source code and protocols, CARLA provides open digital assets (urban layouts, buildings, vehicles) that were created for this purpose and can be used freely. The simulation platform supports flexible specification of sensor suites, environmental conditions, full control of all static and dynamic actors, maps generation and much more.For this project we used the release CARLA 0.9.11 [https://carla.org/2020/12/22/release-0.9.11/] . 

# Tools and Technologies
* Carla simulation tool
The Carla Simulator was developed to support developers to design and verify autonomous driving systems. The Carla platform provides some open-source protocols to support the development and improvement of systems for autonomous driving and also provides a set of sensors and environmental conditions and fully controls them freely.
* Unreal Engine (UE4)
is a complete suite of creation tools for game development, architectural and automotive
visualization, live event production, training and simulation, and other real-time applications.

# Sensors 

 * # Robot Operating System (ROS)
The simulator uses the ROS sensor it detects vehicles and calculates the distance between vehicles

<img width="659" alt="Screen Shot 2021-07-06 at 7 39 02 AM" src="https://user-images.githubusercontent.com/86910279/124543114-5243c600-de2d-11eb-85ba-2c4b6383879f.png">

* # Responsibility sensitive safety (RSS) 
The simulator uses the RSS sensor, when the vehicle approaches another vehicle, the sensor sends a signal to the system and the system reduces the speed

<img width="715" alt="Screen Shot 2021-07-06 at 7 41 55 AM" src="https://user-images.githubusercontent.com/86910279/124543403-db5afd00-de2d-11eb-8035-35cabd18d83e.png">

# Modular Decomposition 
The following figure depicts different modules of CARLA simulator architecture that help to understand the working of the overall system. Each module is assigned a different task. These modules are set to predefined inputs according to which they perform their function and are interconnected through ROS interfaces. These allows the user to understand and interchange the modules with same function, input and output. On the other hand this modular approach allows to test and verify different settings and solutions of test environment.

![Picture2](https://user-images.githubusercontent.com/86910279/124544100-232e5400-de2f-11eb-9f91-cfa1d05173de.png)

According to above shown layout data flows from sensors and processor to different modules. These modules then control the vehicle in terms of steering, accelerating and braking. User can communicate with vehicle through Graphical User Interface, through which aimed destination can be achieved. Additionally, V2X module helps to communicate with other entities of the model.



# Graphical User Interface Description
In this part, we will show some pictures of when the CARLA simulator is running and explain the details about it.

* View of the map from the top

 ![Picture1](https://user-images.githubusercontent.com/86910279/124514950-ec345000-dde6-11eb-97b9-59e5d504b00b.png)
 
 * After adding the vehicles and walkers on the map

 ![Picture1](https://user-images.githubusercontent.com/86910279/124770749-434f3780-df43-11eb-8d54-535b4940b291.png)

* Run's manual control to drive 

![Picture2](https://user-images.githubusercontent.com/86910279/124771182-9a550c80-df43-11eb-93cf-cde1e965d345.png)

* A list of details to help with driving on the CARLA simulation

![Picture1](https://user-images.githubusercontent.com/86910279/124771379-c1134300-df43-11eb-9c43-73b7401ec051.png)

* Change weather on the map

![3](https://user-images.githubusercontent.com/86910279/124771514-db4d2100-df43-11eb-91bf-fd0dd59274ff.png)

* When the vehicle off the lane, details appear at the bottom of the screen

![4](https://user-images.githubusercontent.com/86910279/124771760-12bbcd80-df44-11eb-8efc-5bec6551fb05.png)

* Upon collision, collision details appear at the bottom of the screen 

![5](https://user-images.githubusercontent.com/86910279/124771976-43036c00-df44-11eb-8c82-1322baf74308.png)

![6](https://user-images.githubusercontent.com/86910279/124772124-67f7df00-df44-11eb-9ca8-52f2243ceee2.png)

* run's the "Autopilot ", it is means drive by use the sensors 'RSS' on the road 

![7](https://user-images.githubusercontent.com/86910279/124772345-9e355e80-df44-11eb-97cb-e2d00e4647d9.png) 

* Stand completely on paths, pedestrians, and intersections and make sure of them before setting off, after run's '' autopilot " mode 

![8](https://user-images.githubusercontent.com/86910279/124772526-c91fb280-df44-11eb-862d-2009ae24b6eb.png) 

* Maintaining the path and not leaving it after operating the "autopilot" 

![9](https://user-images.githubusercontent.com/86910279/124772791-fff5c880-df44-11eb-82c7-d5e6e67ba8ec.png)

* Client bounding boxes to alert him to vehicles moving around him 

![10](https://user-images.githubusercontent.com/86910279/124772942-27e52c00-df45-11eb-9338-ddbd40c9ffa7.png)


 # Future work 
 In this project, we presented a model for the development of autonomous vehicles through the Carla simulator, and the development of conditions similar to reality to overcome the problems faced by autonomous vehicles on the roads by developing sensors and linking them to the vehicles for experiment and drawing plans to develop them in the future more precisely. This experience with the Kala simulator had a clear effect on the study and development of autonomous vehicles. Many people strive to be the first to develop a self-driving car that can drive in all driving conditions. Big automakers and tech giants are looking for a way to get to the front of the race. They run a bunch of experiments on the road with their self-driving cars, and the data gathered from these experiments help cars navigate a world where unexpected things happen all the time. In the future of autonomous driving, cars will not only take on many of our tasks, but our societies will undergo a massive redesign. The cars will drive you to the destination and continue to serve the next customer. Then there would be no need for sprawling parking and underground parking, and self-driving cars could provide people with disabilities with the basic freedom to come and go as they like.
