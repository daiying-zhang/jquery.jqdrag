jquery.jqdrag
=================================
一个基于jQuery的拖动插件
---------------------------------
### 主要功能
1. 元素拖动；
2. 支持拖动前、拖动中、拖动完成时的事件处理；
3. 支持拖动方向限定；
4. 支持拖动范围限定；
5. 支持指定拖动触发器元素，
6. 提供外部方法。

### 示例代码
	$('#drag').jqdrag({
		minX:0, //不能超过右边界
		minY:0, //不能超过左边界
		type:'x', //只能水平方向拖动
		onbeforedrag:function(){
			//....
		},
		ondragend:function(){
			//...
		},
		ondrag:function(){
			//...
		}
	});

	//对外方法
	setTimeout(function(){
        	//drag实例的链式调用，无法使用jQuery操作DOM的方法 [不推荐]
        	$('#drag2').jqdrag('getObject')
                	.setOption({maxX:400,maxY:400,minX:10,minY:10})
                	.update();

        	//jQuery的链式调用，可以使用jQuery操作DOM的方法  [推荐]
        	$('#drag3').jqdrag('setOption',{maxX:500,maxY:400,minX:100,minY:100})
                   	.jqdrag('update')
                   	.css({'background':'red'});
	},10000);

### E-Mail
  97532151@qq.com

### Site
  http://sanjh.cn