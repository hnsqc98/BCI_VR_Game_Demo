# BCI_VR_Game_Demo
这是我们从2017.9-2019.5，在本科阶段完成的国家大学生创新创业项目  
《基于视觉刺激和运动想象的脑机接口-虚拟现实动态密室逃脱游戏研发》  
  
选择这样一个课题主要是从以下两个方面考虑：  
* 对于BCI交互而言，我们认为主动式的BCI这种需要外部刺激诱发的交互方式不够自然，被动式的BCI又一直缺少典型的交互场景。何为典型应用场景，简而言之，就是别的交互方式所不能取代的，这点我们在下面展开。
  
* 对于VR而言，我们虽然现在有手柄，但是手柄实现的还是键盘鼠标的移动点击菜单模式。相比之下，语音和手势识别，并不能被别的交互方式所取代，那这就算是种完全新的交互模式。与之类似的，BCI也有其独特性的一面，特别是对“个人状态”“情绪”的衡量上。  
我们可以回想一下各种游戏中对“魔法”“精神力”这类操作的定义模式，比如一个咏唱的进度条，或者长按某个键蓄能，那如果我们可以直接检测用户自己的注意力集中程度，那这个交互方式就能够更让人沉浸。  
这就是这个BCI-VR项目后续项目的出发点，也就是我的毕设，之后等项目完成了，也会在github上公开。
  
* ~~还有我的个人情怀，总觉得脑机接口是人类发展必经之路，希望能够推动人类进步那么一点点，但是目前看来这个想法破灭了。~~
  
稍微有点遗憾的事情是，因为这个项目进行过程中一波三折，所以最后实现的是基础的SSVEP控制移动和场景切换，预期中运动想象控制和注意力检测的部分没有完成。  


## 文件结构
由于源文件是一口气上传上来了，没有具体的内容说明，所以这里简单介绍一下各个部分：  
`Export_Program` 导出的Unity程序  
`Matlab_Code` 数据处理代码，主要是脑电的收取，预处理，切割，和CCA结果输出  
`NovWork` Unity源程序（不要问为什么叫这个，问就是有故事）  


## 项目介绍
我们使用的是八导盐水电极脑电帽，利用nural平台采集设备数据，利用通讯接口传输到matlab中进行数据切片和预处理；之后利用CCA算法，输出识别的分类，将结果输入到Unity项目中，从而实现场景切换和人物移动控制。
![image](https://github.com/Mr-strlen/BCI_VR_Game_Demo/blob/master/Images/eeg_equipment.jpg)
项目结构：
![image](https://github.com/Mr-strlen/BCI_VR_Game_Demo/blob/master/Images/total_model.png)
项目流程：
![image](https://github.com/Mr-strlen/BCI_VR_Game_Demo/blob/master/Images/total_process.png)


## 场景展示
我们也是给场景编了两个故事。

## 写在最后的话
上传这个项目的时候已经是2020的七月底，2020年并不太平，就像我大学这四年一样。  
因为对神经工程的兴趣，我在大一下遇到了想哥，得以遇见张老师以及后来不断教导我的各位老师和学长学姐们，也因此有了这个项目。  
很感谢遇到各位!  
  
这个项目虽然做了两年，但是并不顺利，组员变更，状况不断，曾因为种种原因，一度陷入了停滞。  
后来在我们的努力，老师的协助，朋友的支持下，我们还是完成了这个课题。  
结项的那天我意识到，大学几年的悲观离合都是围绕着这个项目展开的，不过没过多久现实又教我这也不算什么。  
所以谨以此纪念那不悔的大学青春。
    
别人都祝你快乐  
我愿你，遍历山河，觉得人间值得
