# CakephpBakeTemplatesTrw plugin for CakePHP

This plugin help to have a better bake code generation for :
- Entity
- Fixtures
- Templates ( bootstrap needed ):
  - add
  - edit
  - index

This plugin work with bake 1.x

https://book.cakephp.org/bake/1/en/development.html#creating-a-bake-theme

If you need this plugin to work in bake 2.x you need to change the plugin structure :

https://book.cakephp.org/bake/2/en/development.html#creating-a-bake-theme

## Installation

```
composer require iteracode/cakephp-bake-templates-trw
```
Add into Application.php
```php
public function bootstrap()
{
    $this->addPlugin('CsvView');
    //Add here
    $this->addPlugin('CakephpBakeTemplatesTrw');

    parent::bootstrap();
}
```
## Use

To bake with this plugin just use 
```
bin/cake bake WHAT_TO_BAKE TABLE --theme CakephpBakeTemplatesTrw
```
If you to use this theme by default just add
```php
<?php
Configure::write('Bake.theme', 'CakephpBakeTemplatesTrw');
```
In config/bootstrap.php or config/bootstrap_cli.php