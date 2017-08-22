<h1 align="center">
    <img src="images/squash-small-vs.png" alt="squash" width="100" height="118">
  <br>
  Squash debugger for microservices
</h1>


<h4 align="center">Debug your microservices application running on container orchestration from IDE.</h4>
<BR>


Debugging microservices applications is a difficult task. The state of the application is spread across multi microservices and it is hard to get the holistic view of the state of the application. Currently debugging of microservices is assisted by openTracing, which helps in tracing of a transaction or workflow for post-mortem analysis, and linkerd and itsio which monitor the network to identify latency problems. These tools however, do not allow to monitor and interfere with the application during run time. 

In contrast, "traditional" debuggers of monolitic application provide devs with powerful features like setting breakpoints in their codes, following values of variables on the fly, stepping through the code, and changing these variables during run time. 

Squash brings the power of modern popular debuggers to developers of microservices apps that run on container orchestration platforms. Squash bridges between the orchestration platform (without changing it) and IDE. Users are free to choose which containers, pods, services or images they are interested in debugging, and are allowed to set breakpoints in their codes, follow values of their variables on the fly, step through the code while jumping between microservices, and change these values during run time. 

Squash is built to be easily extensible, allowing – and encouraging – adding support for more platforms, debuggers and IDEs.

To learn more about the motivation behind project squash, read our blog [post](https://www.solo.io/single-post/2017/05/14/Squash-Microservices-Debugger) or watch a [recorded demo](). We also encourage you to read squash technical overview [blog]().

To stay up-to-date with Squash, follow us [@GetSoloIO](https://twitter.com/GetSoloIO) and join us on our [slack channel](http://slack.solo.io).


## Supported features:
* Live debugging cross multi microservices
* Debug container in a pod
* Debug a service
* Set breakpoints
* Step through the code
* View and modify values of variables
* and more ...

## demo

<iframe class="imgur-embed" width="100%" height="808" frameborder="0" src="http://i.imgur.com/YDeaHYD.gifv#embed"></iframe>

## Documentation
- **Installation**
  - [install squash](docs/install)
- **Getting Started**
  - [debug your microservice](docs/getting-started.md)
- **User Documenation**
  - using [IDEs to debug](docs/IDEs.md)
  - using the [command line interface](docs/cli.md)
- **Developer Documentation**
  - how to [build squash](docs/build) from source
  - [technical overview](docs/techincal-overview.md)
  - adding [debbuger](docs/debuggers.md) support
  - adding [platform](docs/platforms.md) support
  - squash's [REST API](http://squash.solo.io)

---

## Supported debuggers:
 - [gdb](docs/debuggers/gdb.md)
 - [dlv](https://github.com/derekparker/delve)

## Supported platforms:
 - [Kubernetes](docs/platforms/kubernetes.md)
 
## Supported IDEs:
 - [VS Code](https://github.com/solo-io/squash-vscode)

*We are looking for community help to add support for more debuggers, platforms and IDEs.*

## Roadmap:
  
**debuggers**:
  - [Nodejs](https://nodejs.org/api/debugger.html)
  - [Java](http://docs.oracle.com/javase/7/docs/technotes/guides/jpda/jdwp-spec.html)

**platforms**:
  - [Mesos](http://mesos.apache.org)
  - [Docker Swam](https://github.com/docker/swarm)
  - [Cloud Foundry](https://www.cloudfoundry.org)
  
**IDEs**
  - [Eclipse](https://eclipse.org/ide/)


Squash is still experimental! APIs and compatibility are subject to change. We are looking for community support to help identify potential bugs and compatibility issues. Please open a Github issue for any problems you may experience, and join us on our [slack channel](http://slack.solo.io)

---

## Thanks

**Squash** would not be possible without the valuable open-source work of projects in the community. We would like to extend a special thank-you to [Kubernetes](https://kubernetes.io), [gdb](https://www.gnu.org/software/gdb/) and [dlv](https://github.com/derekparker/delve).
