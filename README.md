# DevOps-AL_Assignment ![DevOps](https://www.capgemini.com/wp-content/uploads/2019/09/DEVOPS.gif)
_________________________________________________________________________________________________
"Demand for the development of dependable, functional apps has soared in recent years. In a volatile and highly competitive business environment, the systems created to support, and drive operations are crucial. Naturally, organizations will turn to their in-house development teams to deliver the programs, apps, and utilities on which the business counts to remain relevant."

"That's a lot to ask from DevOps. Fortunately, there are tools to help deliver custom, quality applications in a timely fashion. Jenkins is one of them. Conjuring images of the stereotypical English butler, the tool acts as a "faithful servant" of sorts, easing cumbersome development tasks."

Let us now begin this article to take a deep dive into what is DevOps, its features and architecture. Main Technology/Tools Used:
_______________________________________________________________________________________________________________
## <img src="https://miro.medium.com/max/1000/1*E8IgOSkMTpBRs0w0-Zsx2g.gif" width=200 height=100>Docker:

Docker is one of the tools that used the idea of the isolated resources to create a set of tools that allows applications to be packaged with all the dependencies installed and ran wherever wanted. Docker has two concepts that is almost the same with its VM containers as the idea, an image, and a container. An image is the definition of what is going to be executed, just like an operating system image, and a container is the running instance of a given image.

**Differences between Docker and VM:**

    Docker containers share the same system resources, they don’t have separate, dedicated hardware-level resources for them to behave like completely independent machines.
    They don’t need to have a full-blown OS inside.
    They allow running multiple workloads on the same OS, which allows efficient use of resources.
    Since they mostly include application-level dependencies, they are pretty lightweight and efficient. A machine where you can run 2 VMs, you can run tens of Docker containers without any trouble, which means fewer resources = less cost = less maintenance = happy people.

## <img src="https://www.edureka.co/blog/wp-content/uploads/2016/11/Jenkins-4.gif" width=300 height=200> Jenkins:

a. What is Jenkins and Continuous Integration?

'Jenkins to the rescue!'

As a Continuous Integration tool, Jenkins allows seamless, ongoing development, testing, and deployment of newly created code. Continuous Integration is a process wherein developers commit changes to source code from a shared repository, and all the changes to the source code are built continuously. This can occur multiple times daily. Each commit is continuously monitored by the CI Server, increasing the efficiency of code builds and verification. This removes the testers' burdens, permitting quicker integration and fewer wasted resources.

b. What are the Jenkins Features?

    Easy Installation:

Jenkins is a platform-agnostic, self-contained Java-based program, ready to run with packages for Windows, Mac OS, and Unix-like operating systems.

    Easy Configuration:

Jenkins is easily set up and configured using its web interface, featuring error checks and a built-in help function.

    Available Plugins:

There are hundreds of plugins available in the Update Center, integrating with every tool in the CI and CD toolchain.

    Extensible:

Jenkins can be extended by means of its plugin architecture, providing nearly endless possibilities for what it can do.

    Easy Distribution:

Jenkins can easily distribute work across multiple machines for faster builds, tests, and deployments across multiple platforms.

    Free Open Source:

Jenkins is an open source resource backed by heavy community support.
