# Install
`sudo snap install docker`  

# Running
Por padrão os comandos de docker requerem permissão do administrador, por isso utilizaremos sempre sudo, por exemplo:  

```shell
$sudo docker images ls
$sudo docker container ls
$sudo docker start xxx
$sudo docker stop xxx
```

# Image
A imagem de um container possui as instruções de como criar o container.  
Utilizando as instruções na imagem você pode criar vários containers.  

# Container
É uma instância em execução do container.  
Imagine como se fosse uma máquina em execução.  

## Example
Em programação uma classe pode gerar diversos objetos, cada um deles armazena seus próprios valores e podem ser deletados/alterados.  
Da mesma maneira uma imagem pode criar diversos containers e mandar cada um deles fazer uma tarefa ou armazenar uma informação.  

## Why
Por que utilizar containers?  
> Posso facilmente criar um container que executa apenas aquilo que me interessa.  
> Por exemplo, um container com apenas o banco de dados PostgreSQL  

Por que não utilizar uma máquina virtual?  
> Preparar uma máquina virtual envolve instalar muitas coisas desnecessárias.  
> Por exemplo, a parte gráfica de um sistema operacional.  

Por que não apenas instalo o que me interessa na minha máquina normalmente?  
> Um container é fácilmente substituivel e recriado.  
> Você pode querer ter vários bancos PostgreSQL e não querem que de conflito entre seus arquivos.  
> Não é preciso se preocupar com instalações diferentes em diversos sistemas operacionais.  
> ...  
