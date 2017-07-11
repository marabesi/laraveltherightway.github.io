---
anchor: configuration
---

# Configurações {#configuration_title}

Sempre tenha certeza que a chave da sua aplicação está configurada. A chave é definida na constante `APP_KEY` no arquivo `.env`. Você pode gerar uma automaticamente com o comando:

```
php artisan key:generate
```


Sempre defina o nome da sua aplicação. Ou seja, em vez de utilizar o namespace padrão _App_, defina um namespace que faça sentido para a aplicação. Isso pode ser feito através do comando:

```
php artisan app:name NomeDaSuaAplicacao
```

Isso faz com que os controllers/models usem o namespace NomeDaSuaAplicacao\Controllers e NomeDaSuaAplicacao\Models.

Use o arquivo `.env` para armazenar qualquer informação importante e acesse esses valores através da função `getenv`. Não use os seus models/controllers para armazenar essas informações e commita-las no Git.