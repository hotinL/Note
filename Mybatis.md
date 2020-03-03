# `Mybatis` 报错

1. `mybatis`多表联查
   - `association` : 使用`ResultMap`映射通过一次联立查询获取一个结果集
   - 懒加载 : 开启`mybatis`懒加载配置,通过`select`两次查询,将第一次获取的`id`传给`select`语句;
     - `@Param`报错 :  参数无法获取,使用`_parameter`

2. 懒加载序列化报错 

   > `@JsonIgnoreProperties(value = { "handler" })` 忽略bean中的不需要转化的属性

3. 参数无法映射

   - 使用`@param`