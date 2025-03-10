Why need Docker:
Different teams (development, testing, operations) work in separate environments, leading to inconsistencies in code behavior across these environments.
Solutions : Docker or virtualization

Difference between Docker and virtualization:

![image](https://github.com/user-attachments/assets/62804b5f-276f-4794-8f17-2409f9b619a5)![image](https://github.com/user-attachments/assets/02500745-92c9-4bf4-af06-a1daad6fdef8)

Virtualization: Creates virtual machines (VMs) that each run their own operating system on top of a hypervisor. This approach requires more resources (CPU, RAM, disk space) because each VM is a complete system.
Suitable for long-term use and resource-intensive applications.


Docker: Uses containers that share the host operating system, allowing multiple applications to run in isolated environments without the overhead of a full operating system for each. This makes Docker containers lightweight and faster to start.
Ideal for short-term activities and microservices, allowing for quick scaling.


