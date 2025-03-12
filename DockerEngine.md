
---

#### **Docker Engine**
**Client-Server Model**:
 **Docker Engine Components**:
  **Docker CLI**: Command-line interface (client).
  
  **Docker Daemon**: Server that executes commands.
  
  **REST API**:ommunication between CLI and daemon.

  - Admins can configure Docker Engine to maintain a desired state.
  - Configuration files/tools manage settings.
  - Linux (e.g., CentOS via RPM).
  - Windows (via EXE/MSI).
  - Mac.

---

#### **2. Docker Plugins**
Extend Docker Engine functionality.
- **Types**:
  **Volume Plugins**: Enable data persistence across hosts.
  
  **Network Plugins**: Provide network configurations.
  
  **Authorization Plugins**: Manage access control.
  
  **Cloud Plugins**: Integrate with AWS, Google Cloud, Azure.
  
  **CI/CD Plugins**: Extend Docker to CI/CD (Jenkins).
  

   Admins can install plugins from Docker Hub.
  Users can create custom plugins.

---

#### **3. Docker Swarm**
 Docker’s built-in clustering/orchestration tool.
**Cluster**: A group of servers providing similar services.
**Swarm Kit**: Foundation of Docker Swarm.

---

#### **4. Data Volumes**
- **Purpose**: Persistent storage for Docker containers.

  Shareable across containers.
  Backup and migration-friendly.
  Cross-platform (Linux & Windows).
Managed via Docker CLI.

---


1. **Docker Engine** = CLI (client) + Daemon (server) + REST API.
2. **Plugins** extend functionality (e.g., volumes, networks, cloud).
3. **Docker Swarm** = Clustering/orchestration.
4. **Data Volumes** = Persistent, shareable, cross-platform storage.
