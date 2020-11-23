# vue里面监听路由变化

###### 1监听是使用watch监听

``` js
watch:{ 
$route(to,from){
    this.crumbs(to)
   }
  },
```

######   2初始化监听不到，需要到cerated函数里面去使用

```javascript
 created() {
     this.crumbs(this.$route);
 }
```



# 特殊字符

> **1版权符号** [©](https://www.w3school.com.cn/html/html_entities.asp)

```html
&copy;
```

> **2 注册商标**[ ®](https://www.w3school.com.cn/html/html_entities.asp)

```html
&reg;
```

> **3 大于 小于 空格[ < > ](https://www.w3school.com.cn/html/html_entities.asp)**

```html
&gt; &lt; &nbsp;
```





# **Vue里的data重置**

```js
Object.assign(this.$data, this.$options.data());
```

# **计算属性可以传参数**

```js
 type(){
            return (e)=>{
            console.log(e);
                return e
            };
        }
```

# **事件总线**

```js
 this.$bus.emit('bPage', 'hello world!');//发送
 this.$bus.$on('bPage',(e)=>{//监听
                console.log(13);
                console.log(e);
                this.name=e;
            })
```

