<ol>
  <li>
    <strong>What is a container image in Docker?</strong>
    <ul>
      <li>A container image is a package that includes all the dependencies and information needed to create a container. It comprises multiple base images layered to form the container's filesystem and is immutable once created.</li>
    </ul>
  </li>
  <li>
    <strong>What is a Dockerfile and what is its purpose?</strong>
    <ul>
      <li>A Dockerfile is a text file containing instructions for building a Docker image. It specifies the base image and the steps to install required programs, copy files, and configure the environment needed to create the final container image.</li>
    </ul>
  </li>
  <li>
    <strong>What does the 'build' process in Docker entail?</strong>
    <ul>
      <li>The build process involves creating a container image based on the instructions in a Dockerfile and the additional files in the build context. This is done using the docker build command.</li>
    </ul>
  </li>
  <li>
    <strong>Define a Docker container.</strong>
    <ul>
      <li>A Docker container is an instance of a Docker image. It represents the execution of a single application, process, or service, containing the Docker image's contents, an execution environment, and a standard set of instructions.</li>
    </ul>
  </li>
  <li>
    <strong>What are volumes in Docker, and why are they used?</strong>
    <ul>
      <li>Volumes in Docker provide a writable filesystem layer for containers, as images are read-only. They allow programs within the container to write to the filesystem and persist data, managed by Docker and residing on the host system.</li>
    </ul>
  </li>
  <li>
    <strong>What is a tag in Docker, and what is its use?</strong>
    <ul>
      <li>A tag is a label applied to Docker images to identify different images or versions of the same image. Tags help in distinguishing between various builds, versions, or environment-specific images.</li>
    </ul>
  </li>
  <li>
    <strong>Explain the concept of a multi-stage build in Docker.</strong>
    <ul>
      <li>Multi-stage builds in Docker allow the use of multiple base images within a single Dockerfile to optimize the final image size. For instance, one stage can compile code using a large image with an SDK, and another stage can create a smaller runtime image to host the application.</li>
    </ul>
  </li>
  <li>
    <strong>What is a Docker repository (repo)?</strong>
    <ul>
      <li>A Docker repository is a collection of related Docker images, labeled with tags to indicate different versions or variants. A repo can contain multiple images for different environments or platforms.</li>
    </ul>
  </li>
  <li>
    <strong>Describe a Docker registry.</strong>
    <ul>
      <li>A Docker registry is a service that provides access to repositories of Docker images. It can be public, like Docker Hub, or private, such as Azure Container Registry or Docker Trusted Registry</li>
    </ul>
  </li>
  <li>
    <strong>What is a multi-arch image in Docker?</strong>
    <ul>
      <li>A multi-arch image simplifies selecting the appropriate image based on the platform where Docker is running. It ensures the correct variant of an image is used, depending on the operating system and version.</li>
    </ul>
  </li>
  <li>
    <strong>What is Docker Hub?</strong>
    <ul>
      <li>Docker Hub is a public registry provided by Docker for hosting Docker images. It supports public and private registries, build triggers, webhooks, and integration with GitHub and Bitbucket.</li>
    </ul>
  </li>
  <li>
    <strong>What is Azure Container Registry?</strong>
    <ul>
      <li>Azure Container Registry is a public resource for managing Docker images in Azure, providing a registry close to Azure deployments and integrating with Azure Active Directory for access control.</li>
    </ul>
  </li>
  <li>
    <strong>Explain Docker Trusted Registry (DTR).</strong>
    <ul>
      <li>Docker Trusted Registry is an enterprise-grade Docker registry service that can be installed on-premises within an organization's datacenter. It is part of the Docker Datacenter product and is used for managing private images securely within the enterprise.</li>
    </ul>
  </li>
  <li>
    <strong>What is Docker Desktop, and what are its components?</strong>
    <ul>
      <li>Docker Desktop is a set of development tools for building, running, and testing containers on Windows and macOS. It includes a Docker host (Linux-based on Hyper-V for Windows and on the Apple Hypervisor framework for macOS) and development environments for both Linux and Windows containers.</li>
    </ul>
  </li>
  <li>
    <strong>What is Docker Compose?</strong>
    <ul>
      <li>Docker Compose is a command-line tool and YAML file format used to define and run multi-container applications. It allows defining an application with multiple services in a single file and deploying them with a single command (docker-compose up).</li>
    </ul>
  </li>
  <li>
    <strong>Define a Docker cluster.</strong>
    <ul>
      <li>A Docker cluster is a collection of Docker hosts that are exposed as a single virtual Docker host. This setup allows an application to scale across multiple hosts, distributing services for higher availability and performance.</li>
    </ul>
  </li>
  <li>
    <strong>What is an orchestrator in Docker?</strong>
    <ul>
      <li>An orchestrator is a tool that simplifies the management of Docker clusters and hosts. It handles container networking, configuration, load balancing, service discovery, high availability, and more. Examples include Kubernetes, Azure Service Fabric, and Docker Swarm.</li>
    </ul>
  </li>
  <li>
    <strong>Why are private image registries recommended, and when should they be used?</strong>
    <ul>
      <li>Private image registries are recommended for storing confidential images and minimizing network latency between the registry and the deployment environment. They are especially useful for enterprises needing secure, fast access to images within their local network or specific cloud environments.</li>
    </ul>
  </li>
  <li>
    <strong>How does Docker ensure consistent deployment across different environments?</strong>
    <ul>
      <li>Docker ensures consistent deployment by using container images that encapsulate the application and its dependencies. These images are versioned and stored in registries, allowing them to be reliably deployed across development, QA, staging, and production environments.
</li>
    </ul>
  </li>
  <li>
    <strong>What is the relationship between Docker images and registries?</strong>
    <ul>
      <li>Docker images are stored in registries, which act as libraries of images. Registries provide access to these images for building and running containers. Public registries like Docker Hub and private registries like Azure Container Registry or Docker Trusted Registry manage and distribute images for different environments and purposes.</li>
    </ul>
  </li>
</ol>
