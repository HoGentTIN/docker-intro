# Introduction to Docker

---

## In the old days

![](./img/traditional-deployment.png)

<!-- https://kubernetes.io/docs/concepts/overview/ -->

---

A lot of drawbacks:

-   TODO

---

## Solution: virtual machines

![](./img/virtualized-deployment.png)

<!-- https://kubernetes.io/docs/concepts/overview/ -->

---

## What is a hypervisor?

---

### 2 types

![](https://miro.medium.com/v2/resize:fit:4800/format:webp/0*uOG3TpWM2BlBYkbg)

<!-- https://medium.com/teamresellerclub/type-1-and-type-2-hypervisors-what-makes-them-different-6a1755d6ae2c -->

---

![](https://img.vembu.com/wp-content/uploads/2022/08/type-1-and-type-2-hypervisors-01.png) ![](https://img.vembu.com/wp-content/uploads/2022/08/type-1-and-type-2-hypervisors-02.png)

---

We still have a lot of drawbacks:

-   TODO

---

## Next solution: containers

![](./img/container-deployment.png)

<!-- https://kubernetes.io/docs/concepts/overview/ -->

---

## Recap

![](https://kubernetes.io/images/docs/Container_Evolution.svg)

<!-- https://kubernetes.io/docs/concepts/overview/ -->

---

## When do we use what?

---

## Docker

---

### What are images?

-   A template containing everything needed to run an application
-   Defined by a `Dockerfile`

---

### What are containers?

-   An isolated environment for your code.
    -   Has no knowlegde about your system.
-

---

### How are images and containers linked together?

E.g. compiled program

```mermaid
flowchart LR
    sourcecode["source code\n(e.g. notepad.cpp)"]
    executable["executable\n(e.g. notepad.exe)"]
    sourcecode --> executable
    executable --> program1["notepad running (1)"]
    executable --> program2["notepad running (2)"]
    executable --> program3["notepad running (3)"]
```

---

![](./img/notepads.png)

---

```mermaid
flowchart LR
    dockerfile["docker file (e.g. `Dockerfile`)"]
    image["image\n(e.g. nginx)"]
    dockerfile --> image
    image --> container1["nginx running (1)"]
    image --> container2["nginx running (2)"]
    image --> container3["nginx running (3)"]
```

---

### DockerHub

![](./img/dockerhub.png)

---

### How it all fits together

![](https://blog.octo.com/docker-registry-first-steps/docker-stages.webp)

<!-- https://blog.octo.com/docker-registry-first-steps -->

---

### What are port bindings?

---

### What are volumes?

---

### What are tags?

---

## Docker Compose

---

Notes:

-   https://www.backblaze.com/blog/vm-vs-containers/
-   https://www.atlassian.com/microservices/cloud-computing/containers-vs-vms
-   https://ubuntu.com/blog/containerization-vs-virtualization
-   https://learn.microsoft.com/en-us/virtualization/windowscontainers/about/containers-vs-vm
-   https://www.docker.com/blog/how-to-use-the-official-nginx-docker-image/
