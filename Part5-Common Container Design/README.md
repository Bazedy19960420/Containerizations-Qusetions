<ol>
  <li>
    <strong>What does a container represent in the container model</strong>
    <ul>
      <li>
        In the container model, a container represents a single process. The container lifecycle is tied to the lifecycle of this process, which is defined by the ENTRYPOINT.
      </li>
    </ul>
  </li>
  <li>
    <strong>Can you explain the types of processes that can run in a Docker container?</strong>
    <ul>
      <li>
        Containers can run long-running processes, such as web servers, and short-lived processes, such as batch jobs. The orchestrator manages these processes and can replace them if they fail.
      </li>
    </ul>
  </li>
  <li>
    <strong>How does Docker handle process failures within a container?</strong>
    <ul>
      <li>
        If a process within a container fails, the container ends, and the orchestrator creates a new container to replace it, maintaining the desired number of instances.
      </li>
    </ul>
  </li>
  <li>
    <strong>Is it possible to run multiple processes within a single container?</strong>
    <ul>
      <li>
        While the common practice is to run a single process per container, it is possible to run multiple processes using a Supervisor pattern if necessary.
      </li>
    </ul>
  </li>
  <li>
    <strong>What is a monolithic application in the context of containerization?</strong>
    <ul>
      <li>
        A monolithic application is a single application or service deployed as one container. Internally, it may consist of several libraries, components, or layers, but externally it appears as a single container.
      </li>
    </ul>
  </li>
  <li>
    <strong> How is scaling handled for monolithic applications in containers?</strong>
    <ul>
      <li>
        To scale a monolithic application, additional copies of the container are deployed, typically managed by a load balancer.
      </li>
    </ul>
  </li>
  <li>
    <strong>What challenges are associated with scaling monolithic applications?</strong>
    <ul>
      <li>
         Scaling monolithic applications means replicating the entire codebase, which can be inefficient if only parts of the application need to scale. Additionally, changes to one component require testing and redeploying the entire application.
      </li>
    </ul>
  </li>
  <li>
    <strong>How do monolithic applications utilize server resources?</strong>
    <ul>
      <li>
         Monolithic applications running multiple instances can efficiently utilize server resources, as each server can run many applications within the same host.
      </li>
    </ul>
  </li>
  <li>
    <strong>What are some deployment options for containerized applications?</strong>
    <ul>
      <li>
         Deployment options include using Azure VMs, Azure App Services, and Azure Load Balancers. These services can manage scaling and deployment of containers efficiently.</li>
    </ul>
  </li>
  <li>
    <strong>What are the benefits of using containers for deployment?</strong>
    <ul>
      <li>
         Containers offer fast scaling and updates, immutability, and efficient resource utilization. They also allow for automated management of instances and their lifecycle through orchestrators.
      </li>
    </ul>
  </li>
  <li>
    <strong>How should persistent data be managed in Docker applications?</strong>
    <ul>
      <li>
        Persistent data should be managed using Docker Volumes or remote storage solutions like Azure Storage, Azure SQL Database, or Azure Cosmos DB. Local storage within containers is not recommended for persistent data.
      </li>
    </ul>
  </li>
  <li>
    <strong>What are Docker Volumes, and how are they used?</strong>
    <ul>
      <li>
         Docker Volumes are directories mapped from the host OS to directories in containers. They persist data independently of the container lifecycle and are managed by Docker, providing a secure and efficient way to handle local data.
      </li>
    </ul>
  </li>
  <li>
    <strong>What are the different types of storage options for Docker containers?</strong>
    <ul>
      <li>
        Storage options include Docker Volumes, bind mounts, and tmpfs mounts. Volumes are managed by Docker, bind mounts map host filesystem folders to containers, and tmpfs mounts are virtual folders in memory.
      </li>
    </ul>
  </li>
  <li>
    <strong>Why is it not recommended to use local container storage for business-critical data?</strong>
    <ul>
      <li>
        Local container storage is ephemeral, meaning data can be lost if the container is deleted. Business-critical data should be stored in persistent storage solutions like remote databases or cloud storage to ensure data durability and availability.
      </li>
    </ul>
  </li>
</ol>
