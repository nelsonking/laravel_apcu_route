### 优化方式

##### 劫持laravel生成路由缓存的命令，添加apcu 缓存，通过提供者服务方法劫持，加载路由方式

#### 更改文件 list

###### app/Console/Kernel.php  ## 添加劫持命令方法
###### app/Console/RouteCache.php ## 命令方法
###### app/Console/stubs/routes.stub ## 路由缓存模板
###### app/Providers/RouteServiceProvider.php ## 注册者服务，劫持路由加载方法