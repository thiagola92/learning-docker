# Remove container
O container criado no capítulo anterior é inútil e deve ser deletado.  
É bom desapegar da idéia que container é algo complicado e difícil de criar, delete e crie quantas vezes quiser.  

```shell
$sudo docker ps -a
$sudo docker rm container_name
```

ou

```shell
$sudo docker container ls -a
$sudo docker rm container_name
```

ou

```shell
$sudo docker container ls -a
$sudo docker container rm container_name
```

Todos estes iram fazer a mesma tarefa, exibir a lista de containers para que você consiga ver o nome do container e mandar remover ele pelo nome (também é possível utilizar o id em vez do nome).  

# Remove image
Ainda vamos utilizar a imagem mas podemos também deletar e baixar a vontade.  

```shell
$sudo docker images
$sudo docker rmi image_name
```

ou

```shell
$sudo docker image ls
$sudo docker rmi image_name
```

ou

```shell
$sudo docker image ls
$sudo docker image rm image_name
```