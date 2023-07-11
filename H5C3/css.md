### HTML5新增的语义化标签
- <header》头部标签
- 《nav>导航标签
- 《article>内容标签
- 《section>定义文档某个区域
- 《aside>侧边栏标签
- 《footer》尾部标签
### HTML5新增的多媒体标签
- 音频 <audio》
- 视频<video》 尽量使用mp4格式

### HTML5新增的input类型
tyle="number" 限制用户输入必须为数字类型
tyle="tel" 手机号码
tyle="search" 搜索框
### HTML5新增的表单属性


==用法：直接放在input属性后面 required=required==
- required 表示其内容不能为空，必填
- placeholder 提示信息 存在默认值将不再显示
改变默认值里面文字的颜色：input：：placeholder {
    color：颜色
}
- autofocus页面加载完毕后自动聚焦在指定表单
- multiple可以多选文件提交
### CSS3新增选择器
#### 结构伪类选择器
nth-child（n）选择某个父元素的一个或多个特定的子元素
- n可以是数字，关键字和公式
- n如果是数字，就是选择第n个子元素，里面熟悉从1 开始...
- n可以是关键字：even偶数，odd奇数
- n可以是公式
  2n    偶数
  2n+1  奇数
  5n    5 10 15...
  n+5   从第五个开始到最后包括第五个
  -n+4  前五个包括第五个
  eg；ul li：first-child {
    color
    background
  }
  ul li: nth-child(n){
    color
  }
  ul li :first-of-type {
  

}
ul li: nth-of-type(n) {
    
}
#####   nth-of-type和nth-child区别
1. nth-child会把所有的盒子排列序号。执行的时候首先看nth-child（1）之后会去看前面的盒子的，如果盒子不一样，就无法起到效果
2. nth-of-type 会把指定元素的盒子排列序号。执行的时候直接找指定的元素第几个孩子
#### 伪元素选择器
befor和after创建一个元素，但是属于行内元素
    新创建的这个元素在文档树中是找不到的，所以称为伪元素
    语法：element::before{}
    brfore after必须有content属性
    before在父元素内容面前创建元素，after在父元素后面插入元素
    伪类选择器和标签选择器一样。权重为1
### CSS新特性
#### CSS3盒子模型
通过box-sizing来指定盒模型
1. box-sizing：content-box盒子大小为width+padding+border（以前默认的）
== box-sizing：border-box盒子大小为width==
用法：box-sizing：border-box；
可以放在最开始的位置


#### CSS3滤镜filter
blur是一个函数，小括号里面的数值越大，图像越模糊
filter：blur（）
#### CSS3calc函数
with：calc（100%-30px）
指的是子盒子永远比父盒子小30px
括号里面可以使用+ — —*/
#### CSS3过渡
transition：要过渡的属性 花费时间 运动曲线 何时开始；
1. 属性：想要变化的宽度高度。背景颜色，内外边距都可以。如果想要所有的的属性都变化过渡，写一个all就可以
2. 花费时间：单位是秒（必须写单位）
3. 运动曲线:默认是ease可以省略
4. 何时开始：单位是秒（必须写单位）可以设置触发时间 默认是0s（可以省略）
5. 过渡口诀：谁做过渡给谁加





















