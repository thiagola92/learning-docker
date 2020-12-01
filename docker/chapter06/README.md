# Build image
Uma imagem é construida lendo um arquivo **Dockerfile**, normalmente esse arquivo recebe o nome de "Dockerfile" e ele possui uma sintaxe própria.  

## Dockerfile
Boa parte das imagens são montadas possuindo outras imagens como base.  
Neste caso iremos usar a imagem do Ubuntu base.  

```Dockerfile
FROM ubuntu
```

## Build image
O comando seguinte procura o arquivo Dockerfile dentro do diretório atual.  

```shell
$sudo docker build .
```

ou

```shell
$sudo docker image build .
```

A imagem vai receber exatamente o mesmo nome da imagem usada como base ao menos que passe um nome diferente para o argumento `--tag`.  
`sudo docker build --tag image_name .`  

Para passar variáveis de ambiente durante a criação da imagem, utilize `--build-arg`  
`sudo docker build --build-arg PASSWORD=123 .`  
Agora a variável de ambiente PASSWORD estará com o valor "123" durante a criação da imagem. Multiplos argumentos são passados da seguinte forma:  
`sudo docker build --build-arg USERNAME=thiagola92 --build-arg PASSWORD=123 .`  