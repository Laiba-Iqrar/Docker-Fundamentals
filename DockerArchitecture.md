# **Docker architecture**
Based on a client-server model.
![image](https://github.com/user-attachments/assets/d81cba20-d358-44da-8367-b0f3891df8b4)


### **Docker Client**: 
Allows users to communicate with Docker and send commands to the Docker daemon.

### **Docker Host**: 
The system where Docker runs containers and applications, consisting of the Docker daemon, images, containers, networks, and storage.

### **Docker Daemon**: 
Executes commands from the Docker client and manages container behavior.

### **Docker Images**: 
Templates used to create containers, containing metadata about functionality and requirements.

### **Docker Registry**: 
A repository for storing Docker images, which can be private (for internal use) or public (like Docker Hub).

### **Containers**: 
Encapsulated environments for applications, with access to defined resources.

### **Networking**: 
Containers can connect through various network drivers, such as Bridge, Host, Overlay, None, and Macvlan.

### **Storage Options**: 
Data can be stored using techniques like data volumes, volume containers, directory mounts, and storage plugins.

-----------------------------------------------
## **Basic Docker Commands**
 
### Docker Pull: 
This command is used to download a Docker image from a registry (like Docker Hub) to your local machine.
Example: docker pull ubuntu downloads the latest Ubuntu image.

### Docker Push: 
This command uploads a local Docker image to a registry.
Example: docker push myusername/myimage uploads your image to your Docker Hub account.

### Docker Run:
This command creates and starts a container from a specified image.
Example: docker run -d -p 80:80 nginx runs an Nginx container in detached mode and maps port 80 of the container to port 80 on the host.

-----------------------------------------------
## Storage Options

### Data Volumes: 
Persistent storage that exists outside of the container's writable layer. They are efficient and can be shared among containers.
Example: docker volume create myvolume (creates a new volume)

### Volume Containers: 
A dedicated container that hosts a volume, which can be mounted to other containers.
Example: You can create a container that manages a volume and share it with other containers.

-----------------------------------------------
## Network Drivers
![image](https://github.com/user-attachments/assets/1b607f14-e143-46bf-9756-42f52fe453d5)


### Bridge: 
The default network driver. It creates a private internal network on your host, allowing containers to communicate with each other.
Example: Containers on the same bridge network can reach each other using their container names.
### Host: 
Eliminates the network barrier between Docker containers and the Docker host. Containers share the host's network stack.
Example: docker run --network host myimage allows the container to use the host's IP address.
### Overlay: 
Used for multi-host networking, allowing containers on different Docker hosts to communicate. Useful for swarm services.
Example: Used in Docker Swarm to connect services across different nodes.
### None: 
Disables all networking for the container. The container will not have any network interfaces.
Example: docker run --network none myimage runs the container without any network access.
### Macvlan:
Assigns a MAC address to a container, making it appear as a physical device on the network.
Example: Useful for legacy applications that require a physical network interface.

-----------------------------------------------
## Docker Registry:

Repository for storing Docker images.

**Private Registry:** For internal sharing within organizations.
**Public Registry:** Like Docker Hub, for sharing with the community.


