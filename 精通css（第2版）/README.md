###精通css读书笔记

-------

#####第4章 背景图像效果
1、黑科技——标题旁边logo
```
.h_logo{  
  padding-left: 40px;
  background-image: url('../../img/1.jpg');
  background-repeat: no-repeat;
  background-position:top left; //设置图像位置
  background-size: contain; //把图像图像扩展至最大尺寸，以使其宽度和高度完全适应内容区域。
}
```
2、不透明度opacity继承问题
```
.opacity{
  background-color:rgb(2, 124, 156);
  border-radius: 4px;
  opacity: 0.4;
  padding: 10px;
  margin-bottom: 10px;
}
.rgba{
  background-color:rgba(2, 126, 154,0.4);
  border-radius: 4px;
  padding: 10px;
}
```
3、css视差效果
设置3层背景图，根据初始位置 background-position的不同，在改变浏览器大小的时候，造成有深度的感觉
```
.bodyground{
  width: 100%;
  height: 800px;
  /* overflow: auto; */
  background-image: url("../../img/2.jpeg");
  background-repeat: repeat-x;
  background-color: #000;
  background-position: 0 0;
}
.midground{
  width: 100%;
  height: 800px;
  background-image:url(../../img/1.jpg);
  background-repeat: no-repeat;
  background-position: 30% 0;
}
.forground{
  width: 100%;
  height: 800px;
  background-image:url(../../img/3.jpg);
  background-color: transparent;
  background-repeat: no-repeat;
  background-position: 80% 0;
}
```
