## 开发遇到的问题:


1. 图片验证码时效性是否需要的问题,不使用会导致什么危害?


不使用会有被破解的风险，而且时效可以及时删除，防止redis内存占用过多的情况。所以还是加上这个功能吧，反正也不复杂。


2. 跨域无法携带cookie的一个解决[方案](http://www.ruanyifeng.com/blog/2016/04/cors.html)

但是个人想要使用jwt的解决方案。

3. 想弄一个无状态的验证码


## 一些觉得有趣的点:



1. 
Golang 可以多参数返回

a = a ^ b 

b = b ^ a

a = a ^ b

2. robots.txt
 ( 看起来是每个网站必备的


## 一些想法

1. 用redis来记录每日pv或许是个比记录在数据库里面更好的解决方案(前提是这个redis不重启23333)。

长期uv,pv并不适合记录在redis里面。



## 一些有趣的工具:

写getter/setter很烦，于是用了lombok

遇到的坑:

用JPA的时候,字段要想好再写,不然改的时候可能会出现一些一下子想不到什么原因的错误,例如:

No property balabla found for type

