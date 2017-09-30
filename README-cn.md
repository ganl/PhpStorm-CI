# phpstorm代码自动补全， CodeIgniter3 & HMVC

HMVC: [https://bitbucket.org/wiredesignz/codeigniter-modular-extensions-hmvc]()

# 配置

## 方法一：设置Include Paths

在项目目录中`External Libraries`上右键，选择`Configure PHP Include Pahts`
![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-201933@2x.png) 

添加`PhpStorm-CI/CodeCompletion`所在位置的绝对路径。
![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/2017-09-30%2020.15.24.png) 

## 方法二：设置Content Root

Windows：菜单 File > Settings > Directories > Add Content Root ，选择`PhpStorm-CI/CodeCompletion`

Mac: Preferences（comand+,）> Directories > Add Content Root ，选择`PhpStorm-CI/CodeCompletion`

![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-203042@2x.png)


# CodeIgniter Specific

将CI的Controller和Model设为Plain text

* system/core/Controller.php
* system/core/Model.php
* application/third_party/MX/Controller.php (mx_controller)

让自己的类库和模型方法能够自动提示补全,在`my_cc.php`文档块部分增加相应的model和library即可

```
 * ***************** YOUR MODELS *****************
 * @property user_model             $user_model
 *
 * ***************** YOUR LIBRARIES *****************
 * @property Migrate                $migrate               Migrate Class
 *
```

## 效果

![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-205656@2x.png)
![s](https://github.com/ganl/mdAssets/raw/master/img/phpStorm-ci/WX20170930-205735@2x.png)



