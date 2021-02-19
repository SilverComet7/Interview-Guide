[TOC]
# [Interview-Guide](https://github.com/qiu-deqing/FE-interview#fe-interview) 
前端总结


# CSS
1. css选择器  ID,类,标签,*,伪类选择器 :link，:visited :focus，:hover，:active, 伪元素::after/::before, 关系选择器 X +>~ Y , [attr] [:checked] , 
2. 优先级
  1. 选择器优先级  !important > 内联 > ID > 类 > 标签 > 继承   
  2. 内联样式表（标签内部）> 内部样式表（当前文件中）> 外部样式表（外部文件中）
- !important
- 内联样式（1000）
- ID选择器（0100）
- 类选择器/属性选择器/伪类选择器（0010）
- 元素选择器/伪元素选择器（0001）
- 关系选择器/通配符选择器（0000）
3. display:none   visibility:hidden   前者不占据空间，造成重排/回流，后者占据空间，自身重绘    v-if 与 v-show
4. css盒模型   box-sizing属性  W3C标准盒模型 content-box  和 IE盒模型 border-box
5. 居中方法  
   1. 块级元素 margin: 0 auto
   2. 针对inline, 内联块inline-block, 内联表inline-table, inline-flex元素及img,span,button等元素
   3. flex方法
   4. 绝对布局方式
```
已知高度
.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 50%;
  height: 100px;
  margin-top: -50px; 
}
未知高度
.parent {
    position: relative;
}
.child {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}

```
6. 继承属性
   1. 文字排版属性 font
   2. line-height
   3. color
   4. visibility
   5. cursor
7. BFC 块格式化上下文 
   1.  决定了元素如何对其内容进行定位以及与其他元素的关系和相互作用
   1.  用display: inline-block 解决垂直外边距重叠问题
8. css预处理器 sass为例 
   1. 变量   $
   2. 嵌套
   3. 控制指令  @if @for  @each
   4. 混合指令  @mixin  @include 
   4. 模块  @import  
9. animation/transtion/transform/filter/box-shadow/@media 
10. 从右向左的渲染机制


# html 
  1. 语义化标签  利于阅读维护,SEO
  2. 行内元素  img span 
     块级元素  h1-h6 header footer div p 
  3. 渲染机制 
  4. [输入URL到显示](https://juejin.cn/post/6844903616101220366#heading-13)
     1. 解析URL获取协议，主机，端口 分装
     1.浏览器缓存-本机缓存-hosts文件-路由器缓存-isp DNS-DNS递归查询
     2. 建立TCP链接 3次握手 确保客户端与服务端通讯政策
     3. 发送http请求
     4. 服务器处理请求 返回响应
     5. 接收HTML CSS JS 构建dom树 -> 构建render树 -> 布局render树 -> 绘制render树
     6. 4次挥手
# http
1. 方法  get/POST/PUT/DELETE
2. 状态码 1xx - 5xx
   - 1XX 信息 100
   - 2XX 成功  200 OK  204 No Content
   - 3XX 重定向  304   
   - 4XX 客户端错误 404 请求资源不存在
   - 5XX 服务器错误 500   504


# 算法



# js



# 正则 
[掘金](https://juejin.cn/post/6844903845227659271#heading-2)
[搜狐](https://www.sohu.com/a/279549933_713028)
  1. 字符
  2. 循环与重复  []
  3. 边界 
  4. 子表达式  分组 / 回溯引用 / 逻辑处理
>   千分位 "123456789999".replace(/(?!^)(?=(\d{3})+$)/g, ",");

# webpack / vite



# [vue  2.x](https://juejin.cn/post/6844903918753808398#heading-7)   
1. 生命周期
   - beforeCreate
   - created  调取接口
   - beforeMounted
   - Mounted   操作DOM
   - beforeUpdate
   - update    
   - beforeDestory  
   - destoryed   
2. 组件传值
   - props emit 
   - vuex
   - ref $parent $children
   - provide / inject 
3. 路由
   - 
   - 

# vue 3.0
1. 组合式api  逻辑放在一起便于管理
2. 提升速度  diff算法
3. 

# uni-app/微信小程序



# 网站优化
1.SEO优化 
  - title的重要性 
  - 语义化HTML 重要HTML放前面
  - 少用iframe 不用js输出
  - 图片 + alt     alt-当图片不存在显示
  -

