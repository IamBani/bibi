# **1.条件编译css**

```css
/* #ifndef APP-PLUS-NVUE */
		@import url("/components/gaoyia-parse/parse.css");
		
		@import "uview-ui/index.scss";
		
		page{
			background-color:#f7f8fa; 
		}
	/* #endif */
```

# **2.条件编译js**

```javascript
// #ifdef APP-PLUS
							      			  this.left=e.touches[0].pageX+'px';
					    this.top=e.touches[0].pageY+'px';
// #endif
// #ifdef MP-WEIXIN
	this.left=e.detail.x+'px';
	this.top=e.detail.y+'px';
// #endif
```

# **3.条件编译html**

```
<!-- #ifdef APP-PLUS -->
	<List></List>
<!-- #endif -->
```

# **4.条件编译json**

<font color=#F40>**注意：如果是最后一项一定要逗号**</font>

```json
//#ifdef APP-PLUS
		,
		{
            "path" : "pages/list/list",
            "style" : {
				"navigationBarTitleText": "list"
			}
        }
//#endif
```

