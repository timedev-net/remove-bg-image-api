# Api para remover o fundo de fotografias

Para uso deve ser enviado um PUT para a rota "/remove_bg" com o anexo da foto através do "Multipart Form" incluindo o caminho do arquivo no atributo "image".

O retorno é a imagem com o fundo removido.


## Comandos para executar o projeto com Docker

1. Cria a imagem docker da aplicação
```
docker build -t bgremover .
```

2. Sobe o container docker que executa a aplicação
```
docker run --rm --name bg-remover -p 5000:5000 bgremover
```
