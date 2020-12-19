# autnomousSysResearch

## Self-driving Cars in Browser Using Neuro.js
-	Must install Node.js to use npm (node packet manager) 
- npm is Node.js’ package ecosystem that includes many public software packages like [neuro.js](https://neuro.js.org/learn/#introduction) (machine learning framework), which can be used to create [autonomous vehicles in browser](https://github.com/janhuenermann/neurojs)
  - See examples folder to see actual code for self driving cars in browser project
-	Easy to [install and setup Node.js](https://nodejs.org/en/download/) and use its libraries (neuro.js)
-	Simplistic environment, more focus on machine learning
- Lightweight

## Open Source Simulators

### CARLA
**Description**
- Built on Unreal Engine (UE4)
- Features include
  - LIDAR
  - Multiple cameras
  - Depth sensors
  - Custom map generation
  - [ROS](https://www.ros.org/about-ros/) (Robot Operating System) integration
- Client/server architecture allows multiple clinets in the same or different nodes
  - Server = environment i.e. simulated world (Unreal Engine, C++)
  - Clients = agents/actors i.e. cars, sensors on cars, pedestrains (Python)
  - Blueprints = attributes of actors
- Simulator controlled by client application that collects data and sends driving instructions to server
- Realistic graphics, urban environments, pedestrians, weather


**Download**
- Download [CARLA] for Windows or Linux(https://carla.readthedocs.io/en/latest/download/)
  - Download [instructions](https://carla.readthedocs.io/en/latest/)
- Need to download Unreal Engine regardless of whether using Windows or Linux
- Need to download Visual Studio on Windows to use CARLA
- No immediate downloadable version of CARLA for OS but can install/build CARLA on Linux using a Mac ([a bit more complicated](https://github.com/carla-simulator/carla/issues/150))
- CARLA includes examples in PythonAPI folder that allows you to interact with environment
  - Need to [download Python](https://www.python.org/downloads/) to access PythonAPI via command line
  - Recommends installation of [numpy](https://numpy.org/install/) and [pygame](https://www.pygame.org/download.shtml) to run examples

**Summary**
- Has both standalone and server mode
  - Standalone mode doesn't connect to a client and the car is controlled manually by keyboard strokes (the default environment when you launch the application)
  - Server mode waits for a client to connect and control the vehicle 
  ([client/server connect instructions](https://carla.readthedocs.io/en/stable/connecting_the_client/))
- Has the most capabilities and features (of all simulators listed here)
- Has documentation and tutorials
  - More tutorials on Linux because CARLA originally built on Linux
- Slow to download because very large file (CARLA recommends 30GB disk space) and many other things to download (Unreal Engine, CARLA, Visual Studio + other minor installations)
- Slow to launch
- Difficult installation/setup 
  - Setup requires compiling all the dependencies and modules to be compatible with Unreal Engine (server) and Python (client)
  - Need to create client/server connection to spawn autonomous vehicles in environment
- More info on their [website](https://carla.org/)


### AirSim
**Description**
- Built on Unreal Engine (UE4) and developed by Microsoft
- Capable of both autonomous vehicle and drone testing

**Download**
- Download [AirSim] for Windows or Linux(https://github.com/Microsoft/AirSim/releases)
  - Download instructions for [Windows](https://microsoft.github.io/AirSim/build_windows/) or [Linux](https://microsoft.github.io/AirSim/build_linux/)
- Need to download Unreal Engine regardless of whether using Windows or Linux
- Need to download Visual Studio to use AirSim
- No immediate downloadable version of AirSim for OS but can build on Linux using Mac, AirSim only supports macOS Catalina([a bit more complicated](https://microsoft.github.io/AirSim/build_linux/))

**Summary**
- Realistic graphics, urban environments, pedestrians, weather
- More info on their [github](https://microsoft.github.io/AirSim/)
- Experimental Unity release in development


### Udacity Self Driving Simulator
**Description**
- Created in Unity environment, connect to Python client
- Built for Udacity Self Driving Car Engineer Nanodegree Course --> corresponding [tutorials/projects](https://github.com/ndrplz/self-driving-car)
- Client/server architecture

**Download**
- Very easy [download](https://github.com/udacity/self-driving-car-sim) available for Linux, Mac, Windows
- Need to [download Unity](https://unity3d.com/get-unity/download)

**Summary**
- Quick and easy startup
- Record training data in Training mode using keyboard controls and test in Autonomous mode
- Simpler environment but can modify track/map in Unity
