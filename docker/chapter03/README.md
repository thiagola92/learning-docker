# Create container
```shell
$ sudo docker run ubuntu
$ sudo docker ps --all
```

ou

```shell
$ sudo docker container run ubuntu
$ sudo docker ps --all
```

ou

```shell
$ sudo docker pull ubuntu
$ sudo docker create ubuntu
$ sudo docker ps --all
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker create ubuntu
$ sudo docker ps --all
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker container create ubuntu
$ sudo docker ps --all
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker container create ubuntu
$ sudo docker container ls --all
```

Todos estes iram fazer a mesma tarefa, criar um container com um nome aleatório e exibir os containers existentes.  
Como este container não possue nenhum programa que fica rodando em loop, ele inicia e finaliza ao mesmo tempo.  

| Comando                  | Comando original                                                           |
| ------------------------ | -------------------------------------------------------------------------- |
| `sudo docker run ubuntu` | `sudo docker image pull ubuntu` <br> `sudo docker container create ubuntu` |
| `sudo docker ps --all`      | `sudo docker container ls --all`                                              |
  