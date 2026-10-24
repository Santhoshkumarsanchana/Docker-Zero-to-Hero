# Multi Stage Docker Build

The main purpose of choosing a golang based applciation to demostrate this example is golang is a statically-typed programming language that does not require a runtime in the traditional sense. Unlike dynamically-typed languages like Python, Ruby, and JavaScript, which rely on a runtime environment to execute their code, Go compiles directly to machine code, which can then be executed directly by the operating system.

So the real advantage of multi stage docker build and distro less images can be understand with a drastic decrease in the Image size.

### 1. Multi-stage Dockerfile
![Multi-stage Dockerfile](images/1-Dockerfile.png)

### 2. Fixing the docker.sock permission error
![Permission denied error](images/2-permission-error.png)
### 3. Single-stage build (1.01GB image)
![Single-stage build](images/3-single-stage-build.png)
### 4. Multi-stage build result (3.94MB image)
![Multi-stage build and size comparison](images/4-Multi-stage-build-and-size.png)
