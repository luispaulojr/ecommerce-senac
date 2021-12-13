# Desafio e-commerce com Python com Django

# Sobre

- Projeto final do treinamento de desenvolvimento com Python.

# Como rodar o projeto

- Para buildar e subir o app
```
docker-compose build
docker-compose up -d
```

- Para rodar os comandos de dentro da VM:
```
docker-compose exec web bash
```

- Para rodar as migrations:
```
docker-compose exec web bash
python manage.py makemigrations
python manage.py migrate
```


- Para popular a base:
```
python manage.py loaddata products
```

- Para criar o usuário do admin:
```
python manage.py createsuperuser
```

- Para rodar os testes:
```
pytest

# teste com cobertura exportado em html:
pytest --cov=. --cov-report html:reports
```