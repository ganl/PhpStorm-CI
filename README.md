#Code Completion for CodeIgniter3 & HMVC projects in PHPStorm

This repository contains helper files for code completion in phpStorm with CodeIgniter3 + HMVC.

CodeIgniter3: [https://github.com/bcit-ci/CodeIgniter.git]()

HMVC: [https://bitbucket.org/wiredesignz/codeigniter-modular-extensions-hmvc]()

## Installation

### Method 1: set up Include Paths

Right-click on `External Libraries` in the project explorer, and select `Configure PHP Include Pahts`

Adds the absolute path to where `PhpStorm-CI/CodeCompletion` is located.


### Method 2: set up Content Root

Windows：File > Settings > Directories > Add Content Root ，select the directory `PhpStorm-CI/CodeCompletion`

Mac: Preferences（comand+,）> Directories > Add Content Root ，select the directory `PhpStorm-CI/CodeCompletion`


# CodeIgniter Specific

Make CI's Controller and Model as Plain Text

* system/core/Controller.php
* system/core/Model.php
* application/third_party/MX/Controller.php (mx_controller)

Let the library and model available to code completion, you need add model and Library to the documentation block corresponding in the `my_cc.php`.

```
 * ***************** YOUR MODELS *****************
 * @property user_model             $user_model
 *
 * ***************** YOUR LIBRARIES *****************
 * @property Migrate                $migrate               Migrate Class
 *
```

## Preview

[ScreenShot](https://github.com/ganl/mdAssets/tree/master/img/phpStorm-ci)

![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-205656@2x.png)
![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-205735@2x.png)

### Origin Repo : [https://github.com/topdown/phpStorm-CC-Helpers]()
