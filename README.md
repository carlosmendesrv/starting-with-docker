<p align="center">
  <a href="#" target="blank"><img src="http://maratona.fullcycle.com.br/public/img/logo-maratona.png"/></a>
</p>

## 👊🏼 Desafio
1 - Configurar um ambiente Laravel utilizando o docker-compose com: <br>
Nginx <br>
PHP-FPM <br>
Redis <br>
MySQL <br>

Lembrando que o volume do código fonte deve ser compartilhado com a App.

2 - Gere o build da imagem desse container e faça a publicação em sua conta no Hub do Docker.
Lembre-se: Ao gerar o build da imagem, TODO o conteúdo incluindo arquivos como vendor, .env, etc deverão ser incluídos.
Adicione o endereço da imagem do seu dockerhub no README.md e faça o commit do projeto contendo todos os arquivos (laravel + docker) para um repositório público do Github.

## ⚙️ Executar a Aplicação

Subindo os container
```bash
$ docker-compose up -d
$ docker exec -it laravel-default_app bash
```

```bash
 composer install
```

Crie o arquivo .env baseado no .env.example
```
php artisan key:generate 
php artisan migrate
```

Acessando a Aplicação
```
http://127.0.0.1:8000
```
