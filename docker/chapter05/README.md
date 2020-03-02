# Create interactive container
Supondo que você deletou sua imagem e container igual no último capítulo, vamos baixar, criar ele e acessa-lo.  

```shell
$ sudo docker run -it ubuntu bash
```

ou

```shell
$ sudo docker container run -it ubuntu bash
```

ou

```shell
$ sudo docker pull ubuntu
$ sudo docker create -i ubuntu
$ sudo docker start container_name
$ sudo docker exec -it container_name bash
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker create -i ubuntu
$ sudo docker start container_name
$ sudo docker exec -it container_name bash
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker container create -i ubuntu
$ sudo docker start container_name
$ sudo docker exec -it container_name bash
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker container create -i ubuntu
$ sudo docker container start container_name
$ sudo docker exec -it container_name bash
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker container create -i ubuntu
$ sudo docker container start container_name
$ sudo docker container exec -it container_name bash
```

Todos estes iram fazer a mesma tarefa, baixar a imagem, criar o container interativo, inicializar ele e executar o bash dentro dele.  
Na criação do container passamos um `-i` para criar um loop interno naquele container, garantindo que ele não finalize assim que começar a executar.  
Na execução do comando bash passamos `-it` garante interatividade ao mesmo tempo que as informações passadas são jogadas para um pseudo-terminal.  