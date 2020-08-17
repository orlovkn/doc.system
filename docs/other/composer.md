Основные команды
========

Инициализация проекта
```
composer init
```

Инициализация проекта
```
composer install
```

Обновление проекта
```
composer update
```

удаление пакета
```
composer remove vendor/package
```

## Примеры composer.json

```
{
	"extra": {
		"installer-paths": {
				"bitrix/modules/{$name}/": ["type:bitrix-module"]
			}
	},
	"require": {
		"andreyryabin/sprint.options": "dev-master",
		"arrilot/bitrix-migrations": "^2.3",
		"symfony/var-dumper": "^3.3"
	}
}
```

```
{
    "require": {
        "roave/security-advisories": "dev-master",
        "cjp2600/bim-core": "^1.1",
        "monolog/monolog": "^1.21",
        "symfony/config": "^3.1",
        "symfony/yaml": "^3.1",
        "symfony/dependency-injection": "^3.1",
        "mikehaertl/phpwkhtmltopdf": "^2.2",
        "mongodb/mongodb": "^1.1",
        "ocramius/proxy-manager": "^1.0",
        "symfony/proxy-manager-bridge": "^3.2",
        "symfony/expression-language": "^3.2",
        "symfony/validator": "^3.2",
        "php-amqplib/php-amqplib": "2.5.*",
        "symfony/symfony": "^3.2",
        "sensio/framework-extra-bundle": "^3.0",
        "sensio/distribution-bundle": "^5.0",
        "symfony/monolog-bundle": "^3.1",
        "box/spout": "^2.7",
        "phpoffice/phpspreadsheet": "1.0.0-beta"
    }
}
```

```
{
	"extra": {
		"installer-paths": {
				"bitrix/modules/{$name}/": ["type:bitrix-module"]
			}
	},
	"require": {
		"andreyryabin/sprint.options": "dev-master",
		"arrilot/bitrix-migrations": "^2.3",
		"symfony/var-dumper": "^3.3"
	}
}
```

```
{
  "require": {
    "roave/security-advisories": "dev-master",
    "cjp2600/bim-core": "^1.1",
    "monolog/monolog": "^1.21",
    "symfony/config": "^3.1",
    "symfony/yaml": "^3.1",
    "symfony/dependency-injection": "^3.1",
    "mikehaertl/phpwkhtmltopdf": "^2.2",
    "mongodb/mongodb": "^1.1",
    "adv/osago-rsa": "^1.7",
    "adv/osago-kbm": "^0.1",
    "ocramius/proxy-manager": "^1.0",
    "symfony/proxy-manager-bridge": "^3.2",
    "symfony/expression-language": "^3.2",
    "symfony/validator": "^3.2",
    "php-amqplib/php-amqplib": "2.5.*",
    "symfony/symfony": "^3.2",
    "sensio/framework-extra-bundle": "^3.0",
    "sensio/distribution-bundle": "^5.0",
    "symfony/monolog-bundle": "^3.1",
    "box/spout": "^2.7",
    "phpoffice/phpspreadsheet": "1.0.0-beta"
  },
  "autoload": {
    "psr-4": {
      "Adv\\": "local/php_interface/adv/lib"
    }
  },
  "repositories": [
    {
      "type": "vcs",
      "url": "git@scm.adv.ru:/sgz/osago-rsa.git"
    },
    {
      "type": "vcs",
      "url": "git@scm.adv.ru:/sgz/osago-kbm.git"
    }
  ]
}
```

```
{
    "name": "orlov/mm",
    "description": "lesson",
    "type": "project",
    "license": "MIT",
    "authors": [
        {
            "name": "orlovkn",
            "email": "to@konstantin-orlov.ru"
        }
    ],
    "minimum-stability": "stable",
    "require": {},
  	"autoload": {
	  	"psr-4": {
		  	"liw\\": ""
		}
	}
}
```
### Ссылки
[Статья на Хабре](http://habrahabr.ru/post/145946/)
