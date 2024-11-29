# Optimizing the placement of an industrial robot for the selective palletizing of packages.
# ONGOING PROJECT
It is required to create a system composed of a conveyor belt on which packages received by the courier arrive 
to be delivered. These packets have a certain address (read by an artificial vision system and
sent to the robot controller on the network interface). Depending on the specified address, there are 10 possible
destinations. Each destination is associated with a list with a container that is filled to the brim with
packets to that destination. The robot-VA-conveyor belt-container system works
continuously. Packages coming onto the lane are selectively palletized to the destination container and when a
container is filled it will be taken out of production for a period of time (20 seconds) to be
loaded into the car. Each container allows the storage of a maximum number of boxes. After it fills up it
is taken out of production and the boxes are disposed of, returning the empty container.
It is required to create a digital model of the above system that generates packets of 10 different types
by reading a message on the network interface. Depending on the package type, the robot executes the trajectory of
handling to the related container. The container has an external dimension of 400mm (width), 300mm (length),
270mm (depth). The packages are cubes of size 40X40X40mm. It will be calculatedthe maximum capacity 
of the container and the disposition of the boxes in the container. Coupling the digital model of
workstation to an application for ordering the creation of boxes and specifying their type. It will be implemented
a socket communication, in which the robot controller is a server and the client sends a command of
box creation and box type.
The project is composed only of the RobotStudio&Rapid program, with commented code so that
understand how the interaction protocol works (Robot-Hercules controller/Putty/client
TCP).

# STAGE 1 (COMPLETED): Realization of project infrastructure with the validation of reaching the points of interest
# STAGE 2 (COMPLETED): Realization of the trajectory of selective manipulation of packages.
(STAGE 2 DETAILS) Each packet type will be assigned a digital input signal that will be operated from the menu
Simulation; when the signal is actuated, a track of the respective type will be generated which will be
palletized in the related container (eg: when generating a type 2 packet it will be palletized in
container 2). A terminal effector (tool) defined by the user will be used. It must be designed as such
so that stacks can be made in containers without collisions.
# STAGE 3 (ONGOING): Integration of a packet generation system with an external application
