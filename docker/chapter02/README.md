# Download image
A imagem que será utilizado durante o aprendizado é a do [Ubuntu](https://hub.docker.com/_/ubuntu)  

```shell
$ sudo docker pull ubuntu
$ sudo docker images
```

ou

```shell
$ sudo docker pull ubuntu
$ sudo docker image ls
```

ou

```shell
$ sudo docker image pull ubuntu
$ sudo docker image ls
```

Todas essas sequências de comandos iram fazer a mesma tarefa, baixa a imagem e mostrar as imagens na máquina.  

| Comando                   | Comando original                |
| ------------------------- | ------------------------------- |
| `sudo docker pull ubuntu` | `sudo docker image pull ubuntu` |
| `sudo docker images`      | `sudo docker image ls`          |

> No docker você verá vários comandos possuem um comando atalho