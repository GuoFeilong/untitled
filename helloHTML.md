#Hello HTML
____

###HTML基本机构
	<html>
	    <head>...</head>
    	<body>...</body>
	</html>
	
	
	1.<html>是根标签网页的内容都在这个标签内
	2.<head> 标签用于定义文档的头部，它是所有头部元素的容器。头部元素有<title>等
	3.在<body>和</body>标签之间的内容是网页的主要内容，如<h1>、<p> <img>等网页内容标签，在这里的标签中的内容会在浏览器中显示出来
	
	

###HEAD标签
   文档的头部描述了文档的各种属性和信息，包括文档的标题等。绝大多数文档头部包含的数据都不会真正作为内容显示给读者。
   
   	<head>
   		 <title>...</title>
   		 <meta>
   		 <link>
   		 <style>...</style>
   		 <script>...</script>
	</head>
					
	
最常见的一个标签				
		
		
		
	<title>标签：在<title>和</title>标签之间的文字内容是网页的标题信息，它会出现在浏览器的标题栏中。
	
	
	
###注释的表现形式
	<!--和Android中布局文件的注释一样写法-->
	
###BODY标签

 在网页上要展示出来的页面内容一定要放在body标签中
 
 
####<p>段落标签
					
	<p>第一段</p>
	<p>第二段</p>
			
类似于文章中的分段

####标题标签	
				<h1>一号</h1>	
				<h2>二号</h2>
				....
				<h6>六号</h6>
				
	标题标签的样式都会加粗，h1标签字号最大，h2标签字号相对h1要小，以此类推h6标签的字号最小。


####强调标签strong和em

两个标签都表示强调一个是粗体一个是斜体

				<strong>加粗内容</strong>
				<em>切斜内容</em>
				
				<!--同时使用-->
				<strong><em>xxxxxx</em><strong>
				
				
				
####强调标签span
1. em和strong标签是为了强调一段话中的关键字时使用，它们的语义是强调。

2. span标签是没有语义的，它的作用就是为了设置单独的样式用的。


					<span>要强调的文本需要在head中加入style标签并对声明span</span>
					
					<!--这是在header中声明的-->
					<head>
					<style>
						span{ color:red; 
								font-size:12;
							}
					</style>
					</head>
					
					
					
####引用标签q和长文本引用blockquote

在网页中引用别人的语句的时候在需要加引用的文本用
包起立即可,在网页中的效果就是加入了引用号

					<q>鹅鹅鹅,曲项向天歌</q>
					<!--长文本引用-->
					<blockquote>这是一首完整的诗词</blockquote>


####换行标签br	
类似于Android布局中字符串\n
		
			<!--在段落中的换行-->
			<p>
				第一行<br/>
				第二行<br/>
				.....
				第三行<br/>	
			</p>
在 html 中是忽略回车和空格的，你输入的再多回车和空格也是显示不出来的,要换行就得用这个标签


####空格的表示
					<!--注意后面那个分号-->
					&nbsp;
					


####水平横线
					<!--水平横线的表示-->
					<hr/>

####地址标签address
					<!--默认风格斜-->
					<address>北京市西城区德外大街10号</address>
					
####代码标签code
					<code>代码语言</code>
    
    
####大量代码pre标签
				<pre>
						android:textSize="12sp"
        				android:textColor="@color/color_red"
       			   		android:grivity="center"
				</pre>			

####无需标签的使用ul li
				<ul>
					<li>第一个标题</li>
					<li>第二个标题></li>
					.....
				</ul>
				
带一个小圆点的效果


####有序标签ol li
				<ol>
					<li>第一个</li>
					.......
				</ol>

有序标签1.2,3.4等

####容器标签div

				<div>
					<!--第一个容器-->
					<h3>无序标题</h3>
					<ul>
						<li></li>
						.....
					</ul>
				</div>
				
				<div>
					<!--第二个容器-->
					<h3>有序标题</h3>
					<ol>
						<li></li>
						.....
					</ol>
				</div>
				
				
				
				
####div命名
				<div id="id_name">
					...内容...
				</div>
				
				
####网页中的表格table

网页中的表格,类似于Android中的TableLayout表格布局

				1,<table>标签,标记表格的开始和结束</table>
				2,<tbody>…</tbody>：当表格内容非常多时，表格会下载一点显示一点，但如果加上<tbody>标签后，这个表格就要等表格内容全部下载完才会显示。如右侧代码编辑器中的代码。
				3,、<tr>…</tr>：表格的一行，所以有几对tr 表格就有几行
				4,<td>…</td>：表格的一个单元格，一行中包含几对<td>...</td>，说明一行中就有几列。
				5,<th>…</th>：表格的头部的一个单元格，表格表头
				
				
				没有增加样式之前默认的表格是没有横线的
				在header中加入style给table使用
				
				 <style type="text/css">
        				table{border:1px solid coral;} 
        				tr{border:1px solid rebeccapurple;} 
        				td{border:1px solid cornflowerblue;}
        				th{border:1px solid royalblue;}
    			</style>
    			
    			<!--类似于Android中注释-->
    			<table summary="表格的摘要增强寓意不会再网页中展示">
    			</table>
    			
    			<!--显示在表格上方的描述-->
    			 <caption>标题文本</caption>

				
				记忆上面几个标签
				tr--->tableRow    行数 包含在table中 或者 tbody中
				th--->tableHeader 标题 包含在tr中
				td--->tbaleData (cell) 单元格列数 包含在tr中
				
			
				
####超链接a标签
网页中的链接,无处不在....
					
					
					
					
				       <a  href="http://www.baidu.com"  title="进入百度">www.baidu.com</a>
				       <!--默认的是在当前标签中打开,在新标签中打开用target属性-->
				        <a  href="http://www.baidu.com"  title="进入百度" target="_blank">www.baidu.com</a>
				        
				        
####在网页中插入图片img标签
				
				<img src="图片地址" alt="下载失败时的替换文本" title = "提示文本">
				<!--demo-->
				        <img src="http://pic.orsoon.com/uploads/allimg/2016/01/27/24-43311453876336.png">

				
				
				src:图片的网络地址
				alt:图片下载不成功显示的文本
				title:图像课件对图片的描述
				


				
				
####与用户交互form表单

使用HTML表单(form)。表单是可以把浏览者输入的数据传送到服务器端，这样服务器端程序就可以处理表单传过来的数据。

所有表单控件（文本框、文本域、按钮、单选框、复选框等）都必须放在 form 标签之间（否则用户输入的信息可提交不到服务器上）。



					<!--登录-->
		 <form action="index.html" method="post">
            <label for="username">用户名:</label><br/>
            <input type="text" name="username" id="username" value=""/><br/>
            <label>密码:</label><br/>
            <input type="password" name="password" id="password" value=""/><br/>
            <input type="submit" value="确定"  name="submit" />
            <input type="reset" value="重置" name="reset" /><br/>
        </form>
        
        
        action:浏览器输入的数据被传送的目的地
        method:请求方式,get post
        name:该属性给配合后台使用类似于id,
        
        <input>标签类似于Android的editext
        
        
        
        
####多行文本输入textarea 
      比如网页中的意见反馈等
       <form>
        <label>意见反馈:</label><br/>
        <textarea rows="10" cols="100">
                请输入您的宝贵意见....
            </textarea><br/>
        <input type="submit" value="重置"/>
        <input type="submit" value="提交"/>

    </form>
      
      
      
####单选框和复选框

类似于我们Android中的radiobutton和checkbox,在网页中这些交互的东西就是一个标签<input,根据不同的type展示不同的样式  ,有点类似于自定义组合view,根据传入的值展示不同的layout布局

	 <form>
        <label>性别:</label>
        <br/>
        <label>男</label>
        <input type="radio"  value="1" name="man"/>
        <br/>
        <label>女</label>
        <input type="radio"  value="2" name="woman"/>
    </form>
      
      
     <!--复选框-->
	 <form>
        <label>兴趣爱好</label>
        <br/>
        <label>旅游</label>
        <input type="checkbox"/>
        <label>旅游</label>
        <input type="checkbox"/>
        <label>旅游</label>
        <input type="checkbox"/>
        <label>旅游</label>
        <input type="checkbox"/>
    </form>
     
     
     注意:同一组的单选按钮，name 取值一定要一致，比如上面例子为同一个名称“radioLove”，这样同一组的单选按钮才可以起到单选的作用。
     
     
     
     
     
     
####下拉列表select+option

		<form>
        <label>下拉列表</label>
        <select>
            <option value="1" >语文</option>
            <option value="2" selected>数学</option>
            <option value="3">历史</option>
            <option value="4">地理</option>
        </select>
    </form>
	
	vale值是给服务器的,使用selected属性可以默认选中并展示在下拉框中
	
	下拉框多选属性:在select中 加入multiple="multiple"即可
	
	
	
	
	
####input标签中的reset和submit
				
		<form>
        <label>姓名</label>
        <input type="text"/>
        <label>班级</label>
        <input type="text" >
        <input type="reset" value="重置"/>
    </form>
    
    reset类型才会清空,submit类型提交表单
    
    
    
    
    
    
#Hello CSS
____

####CSS全称为“层叠样式表 (Cascading Style Sheets)”，它主要是用于定义HTML内容在浏览器内的显示样式，如文字大小、颜色、字体加粗等。Android中好比一个view的style属性:可以把view的各种装饰属性,颜色大小背景图标等,抽取程style,应用的时候只要用这个一个style就可以包含刚才抽取的所有的属性.

					<!--在header中加入style标签-->
					<style type="text/css">
					<!--网页中的段落样式-->
					p{
  							 font-size:20px;/*设置文字字号*/
  							 color:red;/*设置文字颜色*/
  							 font-weight:bold;/*设置字体加粗*/
						}
						<!--网页中的表单样式-->
					form{
						.....
					}
					</style>

	
	
####CSS代码语法

css 样式由选择符和声明组成，而声明又由属性和值组成

选择符：又称选择器，指明网页中要应用样式规则的元素，如本例中是网页中所有的段（p）的文字将变成蓝色，而其他的元素（如ol）不会受到影响。

声明：在英文大括号“｛｝”中的的就是声明，属性和值之间用英文冒号“：”分隔。当有多条声明时，中间可以英文分号“;”分隔
					
				<!--span标签的样式-->
				span{
					font-size:12px;
					color:red;
					.....;
				}
				
				
####CSS注释代码

				<!--这是html的注释方式-->
				/*这是CSS的注释方式*/
				
				
				
				
####内联式css样式，直接写在现有的HTML标签中
这个就类似于Android中写XML文件直接在View上面加颜色,背景,字体,图标等

			     <label style="font-size: 19px;color: aqua;">我是内联式CSS样式</label>
			     
			     
			     
内联式css样式代码要写在style=""双引号中，如果有多条css样式代码设置可以写在一起，中间用分号隔开。


####嵌入式css样式,直接写在当前html的header中
				嵌入式css样式，就是可以把css样式代码写在<style type="text/css"></style>标签之间。如下面代码实现把三个<span>标签中的文字设置为红色：
				
				<style type="text/css">
						span{
   							color:red;
   							.....
   							
							}
						</style>
						
						
				<!--这个就是嵌入式css样式的表达,他在当前html的header中声明要加入样式的节点即可上面的代码就是给span标签加入红色字体-->
				
				
				
####外部式css样式，写在单独的一个文件中
外部式css样式(也可称为外联式)就是把css代码写一个单独的外部文件中，这个css样式文件以“.css”为扩展名，在head内（不是在style>标签内）使用<link标签将css样式文件链接到HTML文件内，如下面代码：





				<link href="style.css" rel="stylesheet" type="text/css" />
				
				1、css样式文件名称以有意义的英文字母命名，如 main.css。
				2、rel="stylesheet" type="text/css" 是固定写法不可修改。
				3、<link>标签位置一般写在<head>标签之内。
				
				<!--实例代码-->
				<!DOCTYPE html>
				<html lang="en">
				<head>
				    <meta charset="UTF-8">
				    <title>外链CSS</title>
				    <link href="helloCss.css" rel="stylesheet" type="text/css"/>
				</head>
				<body>
				    <div>
				        <p>
				           p的样式外链css代码<span>span的样式</span>
				        </p>
				    </div>
				</body>
				</html>


####三种css方式用起来的感觉类似Andorra中的变量作用域
				内联式---->局部变量(当前方法内生效)
				嵌入式---->成员变量(当前类中生效)
				外链式---->外部静态常量(引入即可用)
				
				
####CSS样式选择器
				
				选择器{
				
						样式;
				}

				大括号前面的是选择器,括号里面的是样式
				选择器对应html中的各种标签,
				样式对应,各种属性,比如大小颜色,背景 描边 位置等
				
				
####CSS标签选择器
				标签选择器其实就是html代码中的标签。如右侧代码编辑器中的				<html>、<body>、<h1>、<p>、<img>
				
				作用于生命的 标签
				
				
				
				
####CSS类选择器

				语法:
				.类选器名称{css样式代码;}
				1、英文圆点开头
				2、其中类选器名称可以任意起名
				
				
				使用方法：

				第一步：使用合适的标签把要修饰的内容标记起来，如下：
				
				<span>胆小如鼠</span>
				第二步：使用class="类选择器名称"为标签设置一个类，如下：
				
				<span class="stress">胆小如鼠</span>
				第三步：设置类选器css样式，如下：
				
				.stress{color:red;}/*类前面要加入一个英文圆点*/
				
				
如果直接使用标签选择器的话当前html所有的标签都会用这个属性,如果用类选择器的话,就可以实现同样的标签使用不同的style效果;
									
				<!DOCTYPE html>
					<html lang="en">
					<head>
					    <meta charset="UTF-8">
					    <title>类选择器</title>
					    <style>
					        .first{
					            font-size: 12px;
					            color: aqua;
					        }
					        .second{
					            font-size: 19px;
					            color: pink;
					        }
					    </style>
					</head>
					<body>
					    <div>
					        <p class="first">
					            这是第1个段落;
					        </p>
					        <br/>
					
					        <p class="second">
					            这是第2个段落;
					        </p>
					
					    </div>
					</body>
					</html>

####CSS ID选择器
				在很多方面，ID选择器都类似于类选择符，但也有一些重要的区别：

				1、为标签设置id="ID名称"，而不是class="类名称"。
				
				2、ID选择符的前面是井号（#）号，而不是英文圆点（.）。
				
		<style type="text/css">
			<!--#后面的是要用次选择器的id-->
			#stress{
			    color:red;
			}
			
		</style>
		
		
		
####类和ID选择器的区别

相同点:

	可以应用于任何元素

不同点:
		
		
	1、ID选择器只能在文档中使用一次。与类选择器不同，在一个HTML文档中，ID选择器只能使用一次，而且仅一次。而类选择器可以使用多次。
	<!--类选择器多次用OK的-->
	<p>
		<span class = "class">第一次用</span>
		<span class = "class">第二次用</span>
	</p>
	
	<!--id选择器多次用不OK的,这样的代码是错误的-->
	<p>
		<span id = "id">第一次用</span>
		<span id = "id">第二次用</span>
	</p>



	2、可以使用类选择器词列表方法为一个元素同时设置多个样式。我们可以为一个元素同时设多个样式，但只可以用类选择器的方法实现，ID选择器是不可以的（不能使用 ID 词列表）。
	
	<!--类选择器是OK的-->
	<p>
		<span class = "class1 class2">类选择器多个一起用</span>
	</p>
	
		
	<!--ID选择器是不OK的-->
	<p>
		<span id = "id1 id2">id选择器不能多个一起用</span>
	</p>

	
	
	
	
####CSS子选择器
				子选择器，即大于符号(>),用于选择指定标签元素的第一代子元素。
				.sport>li{font-size: 12px;color: aqua;}
				
				这个选择器会使class为sport的下面的li标签加入字体和颜色,sport2则不会匹配
				
				
			<!DOCTYPE html>
				<html lang="en">
				<head>
				    <meta charset="UTF-8">
				    <title>子选择器</title>
				    <style type="text/css">
				        .sport>li{
				            font-size: 12px;
				            color: aqua;
				        }
				
				    </style>
				</head>
				<body>
				    <ul class="sport">
				        <li>篮球</li>
				        <li>乒乓球</li>
				        <li>羽毛球</li>
				        <li>足球</li>
				    </ul>
				    <ol class="sport">
				        <li>篮球</li>
				        <li>乒乓球</li>
				        <li>羽毛球</li>
				        <li>足球</li>
				    </ol>
				    <ol class="sport2">
				        <li>篮球</li>
				        <li>乒乓球</li>
				        <li>羽毛球</li>
				        <li>足球</li>
				    </ol>
				
				</body>
				</html>
####CSS包含(后代)选择器
				包含选择器，即加入空格,用于选择指定标签元素下的后辈元素。
				>作用于元素的第一代后代，空格作用于元素的所有后代。">"只需要作用于“儿子”，而“空格”则是子子孙孙都被作用了

				用法和>子选择器一样
				
				
####CSS通用选择器

			通用选择器是功能最强大的选择器，它使用一个（*）号指定，它的作用是匹配html中所有标签元素，如下使用下面代码使用html中任意标签元素字体颜色全部设置为红色：

		<style type="text/css">
			<!--这个会作用于整个网页文字全部变成红色-->
			* {color:red;}
			
			
		</style>


####CSS伪类选择符
			伪类选择符，它允许给html不存在的标签（标签的某种状态）设置样式，比如说我们给html中一个标签元素的鼠标滑过的状态来设置字体颜色
			
			
		<!DOCTYPE html>
			<html lang="en">
			<head>
			    <meta charset="UTF-8">
			    <title>伪类选择符</title>
			    <style type="text/css">
			    		/*伪类选择器*/
			        a:hover{
			            color: rebeccapurple;
			            font-size: 20px;
			        }
			    </style>
			</head>
			<body>
			    <div>
			        <p>
			            老是纠结死垃圾死垃圾费老师家里附近,老师交流时<a>这是一个伪类选择器!</a>
			        </p>
			    </div>
			</body>
			</html>

#####    关于伪类选择符，到目前为止，可以兼容所有浏鉴器的“伪类选择符”就是 a 标签上使用 :hover 了（其实伪类选择符还有很多，尤其是 css3 中，但是因为不能兼容所有浏览器，本教程只是讲了这一种最常用的）。其实 :hover 可以放在任意的标签上，比如说 p:hover，但是它们的兼容性也是很不好的，所以现在比较常用的还是 a:hover 的组合。


####CSS分组选择符

多个标签元素设置同一个样式时，可以使用分组选择符（，）
				
				
				比如一段文章第一段全部+ 第二段id为red的span标签,
				
				.第一段,#第二段red span{
						....选择器内容...
				}
				
				
				h1,span{color:red;}
				等同于
				h1{color:red;}
				span{color:red;}		
				
				
####CSS样式的继承
CSS的某些样式是具有继承性的,继承是一种规则，它允许样式不仅应用于某个特定html标签元素.

					
	<!--比如在header中的style写入如下两句代码,相当于p节点在body中的应用会同事应用其三个属性-->
					p{color:blue;}	
					p{border:1px solid green;}
					
					
					
####CSS特殊性
同时给同一个标签设置几个css样式,浏览器会根据设置的样式的权值高低来决定用哪一个

					
					标签的权值为1，
					类选择符的权值为10，
					ID选择符的权值最高为100
					
					p{color:red;} /*权值为1*/
					.class{color:white;} /*权值为10*/
					#id{color:red}/*权值为100*/
					
					.class #id p span li{color:black}????


加入两个css样式有相同的权值,那么会按照先后顺序,进行覆盖
					
					<!--比如在body中给同时应用如下样式的结果-->
					
					p{color:red;}
					p{color:green;}
					p{color:pink;}
					.first{color:blue;}
					<!--结果粉色-->
					<p>
						,.....内容1
					</p>
					<!--结果蓝色-->
					<p class="first">
						,......内容2
					</p>

最高权值!important,在css样式中分号前面加入!important这个,那么他就是最高权值,同时几个css样式应用给标签,生效的就是带有!important的

					p{color:red !important;}
					p.first{color:green ;}
					
					<!--结果全部为红色-->
					<p>
						,.....内容1
					</p>
					<p class="first">
						,......内容2
					</p>
					
					
					
					
					
					<!--只有frist是绿色,其他全部是红色-->
					p{color:red !important;}
					p.first{color:green !important; }
					
					<p>
						,.....内容1
					</p>
					<p class="first">
						,......内容2
					</p>
					<p class="second">
						,.....内容3
					</p>
					<p >
						,......内容4
					</p>
					
					
					
####CSS文字排版属性

字体
					
					<!--可以写中文-->
					body{font-family:"宋体";}
					<!--听说英文兼容性好-->
					body{font-family:"Microsoft Yahei";}
					
					
字号,颜色
					
					body{font-size:12px;color:#666}
		
粗体,斜体
						
					p span{font-weight:bold;}
					p a{font-style:italic;}
下划线,删除线
					
					p a{text-decoration:underline;}
					p a{text-decoration:line-through;}

					
段落缩进<Android中的paddingleft>
					
					
				<!--2em的意思就是文字的2倍大小-->
					p{text-indent:2em;}
					
行间距,字间距(中文字间距、字母间距)奇葩
					
					p{line-height:1.5em;}
					
					<!--中文字间距-->
					h1{
						  letter-spacing:50px;
						}
						
					<!--英文字间距-->	
					h1{
					    word-spacing:50px;
					}
					
					<!--在Android中属性都是设置行间距-->
					<!--设置具体间距-->
					android:lineSpacingExtra 
					<!--设置行间距是原始的倍数-->
					android:lineSpacingMultiplier 
					
					<!--Android中的字间距需要自定义view了-->
					这个属性是缩放文字,也能实现间距,不能输入具体的值,这个是比例
					android:textScaleX

					

对齐属性
					<!--Android中类似的gravity属性-->
					
					h1{
					    text-align:center;
					    text-align:left;
					    text-align:right;
					}

					
					
####CSS布局
在CSS中，html中的标签元素大体被分为三种不同的类型：块状元素、内联元素(又叫行内元素)和内联块状元素。

常用的块状元素有：

					
					<div>、<p>
					<h1>...<h6>
					<ol>、<ul>
					<dl>、<table>
					<address>
					<form>


常用的内联元素有：

					
					<a>、<span>、
					<br>、<i>、
					<em>、<strong>、
					<label>、<q>、
					<var>、<cite>、
					<code>

常用的内联块状元素有：
					
					<img>、<input>

将一个普通标签具有块状特点

					<!--添加display属性为block-->
					a{display:block;}
					


块级元素特点：
					
					1、每个块级元素都从新的一行开始，并且其后的元素也另起一行。
					
					2、元素的高度、宽度、行高以及顶和底边距都可设置。
					
					3、元素宽度在不设置的情况下，是它本身父容器的100%（和父元素的宽度一致），除非设定一个宽度。
					
将一个标签具有内联元素特点
					
				 div{
				     display:inline;
				 }

内联元素特点：

					
					1、和其他元素都在一行上；

					2、元素的高度、宽度及顶部和底部边距不可设置；
					
					3、元素的宽度就是它包含的文字或图片的宽度，不可改变。


将一个标签具有内联块特点
					<!--有点类似Android中的属性组合比如清单文件中的adjust|hidden控件的Gravity组合等-->
					
					<!--用中横线有点怪,平时定义名字习惯下划线-->
					 div{
                			 display:inline-block;
             			}
             			
             			
inline-block 元素特点：

					
					1、和其他元素都在一行上；

					2、元素的高度、宽度、行高以及顶和底边距都可设置。


####CSS边框属性
类似于Android的矩形描边的实现,一个shape.xml的实现

					
					<!--缩写-->
					标签名{
						 border:2px  solid  red;
					}
					
					<!--完整的写法-->
					div{
					    border-width:2px;
					    border-style:solid;
					    border-color:red;
					}
					
					<!--边框样式style的值-->
			dashed（虚线）| dotted（点线）| solid（实线）
			
			
在Android中经常会有圆角矩形只有上面或者下面的倒角的,但是如果边框只要某个方向的就需要自己去拼组合view或者自定义,在CSS中,他的border是可以向Android中的Corner一样分方向来写的,
比如

					
					标签{
					<!--这就是只有下边线的边框,同理还能设置top left right-->
						border-bottom:1px solid red;
					}


####CSS宽度和高度
CSS定义的宽度和高度,和我们Android中定义view的size是不一样的.

在Android中,写一个View定义了具体的宽度和高度,那么这个view的大小就限制,就是刚才定义的宽和高,然后我们在view上面使用padding和margin属性的时候,是基于定义的size来使用的,无论怎么写margin或者padding,影响的都是View在父布局的位置,以为view的内容,本身view的大小不受影响,

在CSS中,定义的宽度和高度指的是内容范围,如果是文本那么就是文本的承载范围,如果是图片就是图片内容的显示范围,但是一个元素的实际宽度

					
	实际宽度=左边界+左边框+左填充+内容宽度+右填充+右边框+右边界。
	
高度也一样

####CSS中的padding和margin
用法和Android中是那么的统一,
				
				标签{
					<!--四个方向全部设置-->
					padding:10px;
					margin:10px;
				}
				
				<!--不一样值可以分开写-->
				标签{
					   margin-top:20px;
					   margin-right:10px;
					   margin-bottom:15px;
					   margin-left:30px;
					}	
								
				<!--CSS中还能这么偷懒,Android中没有这个-->
				标签{margin:20px 10px 15px 30px;}


####CSS中的布局
在网页中有三种布局,
					
1.流动模型(Flow)
					
					流动模型是默认的网页的布局模式,在这种布局中块状元素(div, h, li ,ul,table...)都会以行的形式占据位置,
					在布局中按顺序垂直分布,说白了 " ≈" Android中的Linearlayout的vertical模式,
					因为块状元素不指定宽度的情况下默认是100%,所以会占据一行,
					在Flow布局中,内联元素都会在所处的包含元素内从左到右水平分布显示。(a,span,em,strong...)他们就会按照水平分布,这回就又变成Android中的LinearLayout的horizontal模式.
					不同的是CSS中水平排列到头会折行,这样又有点像一个满屏幕textview......
					
					
					
2.浮动模型(Float)
						
						任何元素在默认的情况下是不能浮动的,
						用CSS样式可以把他变成浮动,
						
						p{
						    width:200px;
						    height:200px;
						    border:2px red solid;
						    <!--这样标签就会从左边开始水平排队-->
						    float:left;
						}
					
					<!--如果不加float,他是从下往下排列的,加完就是水平从左边开始排列的-->
					<p>
						....
					</p>
					<p>
						....
					</p>

					
		如果两个p 一个左边,一个右边 ,那么只能给p加id ,然后写两个css样式分别给不同的标签p应用
		

3.层模型
	就像图像软件PhotoShop中的图层一样可以对每个图层能够精确定位操作。CSS定义了一组定位（positioning）属性来支持层布局模型。
	
	层模型有三种形式：
	1、绝对定位(position: absolute)

	2、相对定位(position: relative)

	3、固定定位(position: fixed)

		
绝对定位,需要设置position:absolute(表示绝对定位)，这条语句的作用将元素从文档流中拖出来，然后使用left、right、top、bottom属性相对于其最接近的一个具有定位属性的父包含块进行绝对定位。如果不存在这样的包含块，则相对于body元素，即相对于浏览器窗口。

大白话:一个标签的style中加入了position:absolute,那么这个标签中的绝对属性值,是直接参考于他的最近的一个容器,如果没有就是参考浏览器,坐标系和Android是一样左上角0.0点

					<!--距上50px,距左100-->
					div{
						    width:200px;
						    height:200px;
						    border:2px red solid;
						    position:absolute;
						    left:100px;
						    top:50px;
						}	
			
相对定位:
相对于自己之前的位置改变的偏移量:position:relative
					
					<!--距上50px,距左100-->
					div{
						    width:200px;
						    height:200px;
						    border:2px red solid;
						    position: relative;
						    left:100px;
						    top:50px;
						}	
					
假如一个网页中就一个div节点,这两个代码都能实现div块偏移,但是两个偏移有着实质性的差异;

第一种局对偏移,标签做过对应的偏移量流出的空白位置,别的标签是可以用的,
第二种相对于自己做偏移,标签做过对应的偏移量后流出的空白位置,别的标签依然不能占用,

大白话:第一种 地铁上三个座位你做中间:一对情侣站你对面,说往右边做一下,我们两个想坐一起,你向右偏移了一个像素,那么此时你左边的两个座位那对情侣就可以在你面前秀恩爱了.....

所以此时情况就应该用第二种方式:
地铁上三个座位你做中间:一对情侣站你对面,说往右边做一下,我们两个想坐一起,然后你礼貌的像右边移动了一个像素,然后啪的一下把自己的书包放到了原来的你的中间位置上.........


					
					<!--代码-->
					<!DOCTYPE HTML>
						<html>
						<head>
						<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
						<title>relative样式</title>
						<style type="text/css">
						#div1{
						    width:200px;
						    height:200px;
							border:2px red solid;
							position:absolute;
						    top:50px;
						    left:100px;  
						}
						
						</style>
						</head>
						<body>
							<div id="div1"></div>
						    <span>地铁上三个座位你做中间:一对情侣站你对面,说往右边做一下,我们两个想坐一起,你向右偏移了一个像素,那么此时你左边的两个座位那对情侣就可以在你面前秀恩爱了.....</span>
						</body>
						</html>
			
					
固定定位:
		视图本身是固定的，它不会随浏览器窗口的滚动条滚动而变化
		(类似于Android中的framelayout 上面一层中间放了一个ImageView,下面是一个满屏的Listview,Listview的滑动时不会影响imageView的位置跟着滑动的,因为他不是listview的一部分,)
		
		
							
							#div1{
							    width:200px;
							    height:200px;
							    border:2px red solid;
							    <!--固定-->
							    position:fixed;
							    left:100px;
							    top:50px;
							}
							
							
							
####CSS元素水平居中

水平居中设置-行内元素
如果被设置元素为文本、图片等行内元素时，水平居中是通过给父元素设置 text-align:center

就是Android中对于一个满屏的textview设置gravity属性center_horizontal,

水平居中设置-定宽块状元素
就是在css中标签的宽度是固定的,相对于浏览器他就是不是满屏幕的,此时给他设置居中属性内容居中明显是不管用的除非你能设置给浏览器,因为此时,定宽度的view是属于浏览器的内容,
这个时候就需要给标签设置css样式,
				
				div{
					    border:1px solid red;
					    
					    width:200px;/*定宽*/
					    margin:20px auto;
					}

			/* margin-left 与 margin-right 设置为 auto */

这样设置标签的宽度就可以了水平居中了,

水平居中设置-不定宽元素

1,用table标签包裹

					<!--css样式代码-->
					<style>
						table{
						    border:1px solid;
						    margin:0 auto;
						}
					</style>
					
					
					<!--html代码-->
					<div>
					 <table>
					  <tbody>
					    <tr><td>
					    <ul>
					        <li>我是第一行文本</li>
					        <li>我是第二行文本</li>
					        <li>我是第三行文本</li>
					    </ul>
					    </td></tr>
					  </tbody>
					 </table>
					</div>
2,将要居中的标签变成行内元素,然后用text-align就是把他当成父布局的内容

					
					<!DOCTYPE HTML>
						<html>
						<head>
						<meta charset="utf-8">
						<title>不定宽块状元素水平居中</title>
						<style>
						<!--类选择器属性内容居中-->
						.container{
								text-align:center;
								}
						<!--类选择器的加空格 后代选择器,下面的UL标签变成行内元素-->
						.container ul{
							list-style:none;
							margin:0;
							padding:0;
							display:inline;
						}
						<!--同上-->
						.container li{
							margin-right:8px;
							display:inline;
						}
						</style>
						</head>
						
						<body>
						<div class="container">
						    <ul>
						    	<li><a href="#">1</a></li>
						        <li><a href="#">2</a></li>
						        <li><a href="#">3</a></li>
						    </ul>
						</div>
						</body>
						</html>
						
						
3.改变元素的display类型
通过给父元素设置 float，然后给父元素设置 position:relative 和 left:50%，子元素设置 position:relative 和 left: -50% 来实现水平居中。

			<style>
				<!--div标签相对于浏览器往右边移动了一半-->
				.container{
				    float:left;
				    position:relative;
				    left:50%
				}
				<!--div标签内的ul标签,相对于div往左边移动了一半-->
				.container ul{
				    list-style:none;
				    margin:0;
				    padding:0;
				    
				    position:relative;
				    left:-50%;
				}
				<!--改变为行内元素-->
				.container li{float:left;display:inline;margin-right:8px;}
				</style>
					
					
					
				<body>
					<div class="container">
					    <ul>
					        <li><a href="#">1</a></li>
					        <li><a href="#">2</a></li>
					        <li><a href="#">3</a></li>
					    </ul>
					</div>
					</body>
					
			