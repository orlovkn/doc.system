### Установка
```
composer create-project symfony/website-skeleton mysite.local
```

[install](htps://www.youtube.com/watch?v=ABdeoIm6e74)

[дока](https://symfony.ru/doc/current/doctrine.html)

### создать сущность
```
php bin/console make:entity
```

### создать новую миграцию
```
php bin/console make:migration
```

### опросить на предмет изменений в сущностях
```
php bin/console doctrine:migrations:diff
```

### выполнить существующие миграции
```
php bin/console doctrine:migrations:migrate
```

```
To run just this migration for testing purposes, you can use migrations:execute --up 'DoctrineMigrations\\Version20201027035620'

To revert the migration you can use migrations:execute --down 'DoctrineMigrations\\Version20201027035620'
```

### очистить кэш
```
bin/console cache:clear
```

### создать пользователя
```
bin/console make:user
```
### сделать аутентификацию
```
bin/console make:auth
```

### хз
```
php bin/console messenger:consume async
```



https://websiteforstudents.com/how-to-install-symfony-5-on-ubuntu-18-04-16-04-with-nginx/



### создать контроллер
php bin/console make:controller


### создать базу
php bin/console doctrine:database:create

### роутинг
php bin/console debug:router

### создать форму
bin/console make:form
https://symfony.com/doc/current/forms.html

### админки
https://symfony.com/doc/current/bundles/EasyAdminBundle/index.html
https://symfony.com/doc/current/cmf/tutorial/sonata-admin.html

### поля
update_at — datetime
is_published — boolean
ManyToOne — relationship

Main types
  * string
  * text
  * boolean
  * integer (or smallint, bigint)
  * float

Relationships / Associations
  * relation (a wizard 🧙 will help you build the relation)
  * ManyToOne
  * OneToMany
  * ManyToMany
  * OneToOne

Array/Object Types
  * array (or simple_array)
  * json
  * object
  * binary
  * blob

Date/Time Types
  * datetime (or datetime_immutable)
  * datetimetz (or datetimetz_immutable)
  * date (or date_immutable)
  * time (or time_immutable)
  * dateinterval

Other Types
  * ascii_string
  * decimal
  * guid
  * json_array



```
$patchList = $this->patchRepository->findBy([], ['id' => 'DESC'], 5, 0);

$repository = $this->getDoctrine()
                   ->getManager()
                   ->getRepository('GeneralRegistrationBundle:Service');

$service = $repository->findOneBy(array('name' => 'Registration'),array('name' => 'ASC'));

$comment = $service->getComment();
$name = $service->getName();

return new Response('le service is '. $name . ', content is ' . $comment);
```

```
$service = $repository->findBy(array('name' => 'Registration'),array('name' => 'ASC'),1 ,0);
$repository->findBy(array('name' => 'Registration'),array('name' => 'ASC'),1 ,0)[0];
```

https://folkprog.net/doctrine-symfony-framework/


### сервисы
выполняют только логику

### Ссылки
