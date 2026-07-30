Introducing OS-Level Virtualization

What is OS-Level Virtualization?
OS-level virtualization is a method of running multiple isolated, containerized applications on a single operating system while sharing the host operating system’s kernel. Each application runs inside its own container, which packages the application together with the libraries and dependencies it needs to run. This helps ensure consistent behavior across development, testing, and production environments while simplifying application deployment and updates. As a result, system integrators can maintain applications more reliably across different computers and environments. Because containers are lightweight and portable, they have become an increasingly popular way to deploy and run applications for industrial control systems. Docker, an open-source platform, is the industry standard for building, deploying, and managing containerized applications. It provides the tools needed to build, distribute, and run containerized applications consistently across multiple systems.

Key Features
OS-level virtualization provides several benefits that make it well suited for industrial applications, including: 
•	Lower resource overhead than VMs
•	Fast startup times
•	Application isolation using containers
•	Portable container images
•	Shared host operating system kernel
•	Process-level isolation
•	High application density per host

 
OS-Level Virtualization vs. Virtual Machines
Unlike a traditional virtual machine (VM), OS-level virtualization does not create a complete virtual computer for each isolated environment. A virtual machine includes its own guest operating system, while multiple containers share the host operating system’s kernel. Although they share the same kernel, each container remains isolated and can access only its own files, resources, and assigned devices. Because containers do not require separate guest operating systems, they generally start much faster and consume fewer CPU, memory, and storage resources than virtual machines. This allows more applications to run on the same hardware while simplifying software deployment and maintenance. For applications where fast deployment, efficient resource utilization, and high application density are important, OS-level virtualization provides a lightweight alternative to traditional virtual machines.

OS-Level Virtualization:
Runs applications in isolated user-space	
Uses OS-level isolation instead of hardware virtualization	
Shares the host operating system’s kernel
Uses containers for application isolation	
Slices a single host filesystem into isolated view	
	
Virtual Machine:
Runs applications in isolated user-space	
Uses hardware virtualization for isolation		
Can run a different kernel than the host		
Uses a hypervisor to virtualize an entire computer		
Commonly creates entire system snapshots	

NOTE
Containers share the host operating system’s kernel and therefore must use the same operating system family as the host. Virtual machines (such as VMWare), however, can run different operating systems on the same physical hardware.

Sources
https://en.wikipedia.org/wiki/OS-level_virtualization 
https://en.wikipedia.org/wiki/Docker_(software) 
https://www.scalecomputing.com/resources/exploring-uses-benefits-and-types-of-virtual-machines 
https://unwiredlearning.com/blog/containers-os-virtualization 
https://www.ibm.com/think/topics/hypervisors 
https://learn.microsoft.com/en-us/virtualization/windowscontainers/about/containers-vs-vm