### 开发遇到的问题:

1. 图片验证码时效性是否需要的问题,不使用会导致什么危害?
   
   :white_check_mark:不使用会有被破解的风险，而且时效可以及时删除，防止redis内存占用过多的情况。所以还是加上这个功能吧，反正也不复杂。


2. 跨域无法携带cookie
   
   :white_check_mark: 解决[方案](http://www.ruanyifeng.com/blog/2016/04/cors.html),但是个人想要使用jwt的解决方案。

3. 想弄一个无状态的验证码
   
   :question: 目前仍旧无解
