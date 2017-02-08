# 分享组件
一个东凑西凑改出来的分享组件,效果貌似还行~<br>
Demo:http://demo.gfwboom.com/myshare
```
var config = {
            url: window.location.href,
            title: document.title,
            desc: _desc,
            img: document.getElementsByTagName('img').length > 0 && document.getElementsByTagName('img')[0].src,
            img_title: document.title,
            from: window.location.host,
			
			// 如果使用UC、QQ浏览器可调用其分享接口
			// 1：底部(有微信)、有右上角
			// 2: 底部(有微信)、无右上角
			// 3: 底部(无微信)、有右上角
			// 4: 底部(无微信)、无右上角
			// 5: 底部(有微信、但点击后提示复制下方链接)、有右上角
			// 6: 底部(有微信、但点击后提示复制下方链接)、无右上角
			// 7: 底部(有微信、但点击后提示复制下方链接)、点击微信、朋友圈才显示右上角提示
			
			//指定app弹出某个类型的分享组件,通过浏览器ua来判断
			//(UC浏览器、QQ浏览器、手机QQ内置浏览器、微信已在js文件里判断,如需改动需要到js里改,此处无需再填)，
            appShowType: {//格式： '【UA(全小写)】':【类型1~7】
                'weibo': 3
            },
            defaultShowType: 6 //默认显示类型6
        };
```
