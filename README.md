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

### E-Mail
  97532151@qq.com

### Site
  http://sanjh.cn