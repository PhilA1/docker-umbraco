# docker-Umbraco

A collection of useful powershell scripts and dockerfiles for using when deploying the Umbraco CMS into a MSWindows container.

## Pre-Requisites

* [Docker][4] v1.13
* [PowerShell][5]
* Windows10 Anniversary Edition or Windows Server 2016

To use images from this repository you will need to switch Docker to using Windows Containers. If you are new to Docker or Windows Containers the [Build And Run Your First Docker Windows Server Container][3] will guide you through the process of getting setup with these pre-requisites. For Windows 10 users the [Windows Containers on Windows 10][7] quickstart covers the same material.


## Building the Umbraco Image

```
# Clean out any previous containers and images
PS> ./dockerclean.ps1

# Build and run a named container - umbraco.web
PS> ./dockerrun.ps1
```

You should now be able to connect to your running container using the IP address given on screen. 


## More Information

Take a look at my other [docker windows repo][9] for more useful powershell docker scripts.


 [1]: https://our.umbraco.org/contribute/releases/759
 [2]: https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-server
 [3]: https://blog.docker.com/2016/09/build-your-first-docker-windows-server-container/
 [4]: https://www.docker.com/
 [5]: https://msdn.microsoft.com/en-us/powershell/mt173057.aspx
 [7]: https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-10
 [9]: https://github.com/PhilA1/docker-aspmvc
