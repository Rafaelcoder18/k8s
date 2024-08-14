### Container engine

O container engine é responsável por realizar a criação do container, realizar helthcheck, montagem de volume, rede, ou seja, realiza o gerenciamento de todos os recursos necessários para o container. Porém não conversa com o kernel, isso é responsabilidade do container runtime. O container runtime faz a comunicação entre o container engine e o kernel.

### Container runtime

É responsável por criar o container, e realizar a comunicação entre o kernel. É responsável pela execução do container. O Containerd é container runtime utilizado pelo kubernetes.

#### 3 tipos de container runtime

Low-level: Se comunica diretamente com o kernel. É responsável por criar os namespaces e cgroups que serão utilizados pelos containers.

High-level: São executados pelo container engine. Containerd é um container runtime de alto-nivel. A sua responsabilidade é conversar com o kubernetes para gerenciar ciclo de vida do container, organizar a criação, etc.



