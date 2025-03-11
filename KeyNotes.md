Why need Docker:
Different teams (development, testing, operations) work in separate environments, leading to inconsistencies in code behavior across these environments.
Solutions : Docker or virtualization

------------------------------------------------------

**Difference between Docker and virtualization:**
![image](https://github.com/user-attachments/assets/62804b5f-276f-4794-8f17-2409f9b619a5)

**Virtualization**: Creates virtual machines (VMs) that each run their own operating system on top of a hypervisor. This approach requires more resources (CPU, RAM, disk space) because each VM is a complete system.
Suitable for long-term use and resource-intensive applications.
Measured in gigabytes

**Docker**: Uses containers that share the host operating system, allowing multiple applications to run in isolated environments without the overhead of a full operating system for each. This makes Docker containers lightweight and faster to start.
Ideal for short-term activities and microservices, allowing for quick scaling.
Measured in megabytes

------------------------------------------------------

 **Docker's role in DevOps.** 

DevOps: It combines development (Dev) and operations (Ops)
DevOps aims to streamline the software release, configuration, and monitoring processes, making them the responsibility of developers.
It emphasizes continuous coding, building, testing, and deployment of application code.
Various tools are needed to support the DevOps process, with Docker being highlighted as a key tool that facilitates continuous application deployment.

------------------------------------------------------

**Microservices**:
MicroServices are a variation of Service-Oriented Architecture (SOA), allowing software development to be divided into smaller, manageable segments handled by different teams

------------------------------------------------------
**Monolithic VS Microservices Architecture**:

**Monolithic Services**:
Single Unit: The entire application is developed as one unit, with tightly coupled components.
Containerization: Packaged as a single Docker container, including all dependencies.
Deployment: Involves running one container, making it straightforward.
Scaling: Challenging, as scaling requires replicating the entire application.
Maintenance: Any updates require redeploying the whole application, which can be time-consuming.

**Microservices Architecture**:
Independent Services: Decomposes the application into smaller, loosely coupled services.
Containerization: Each service is packaged in its own Docker container, allowing for flexibility.
Deployment: Involves multiple containers, enabling independent scaling.
Scaling: Allows for fine-grained scaling of individual services based on demand.
Maintenance: Updates to one service do not affect the entire application, making it easier to manage.

------------------------------------------------------

