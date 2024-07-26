# test
![镇楼图.png](https://www.freeimg.cn/i/2024/07/26/66a3adca9a136.png)    
1.如何拉半格高？  
众所周知，按上下键盘可以抬升高度或降低高度，但只能降低一格。  
![alt text](传送带高度.png)  
如果新建的带子跨越带子，比如拉拉十字，建造系统会尝试建造半格高的带子来跨过原有带子。  
当然，受限于坡度，必须预留2格距离，不能急转弯。  
![alt text](十字传送带.png)  
![alt text](十字传送带错误.png)  
但如果我们尝试在带子上建造带子，就会造出一长段0.5格的带子。  
删除不需要的带子后，使用蓝图功能复制(ctrl+C),即可批量使用这根带子。  

[![alt text](半格高.png)  ](https://www.freeimg.cn/i/2024/07/26/66a3adca9a136.png)

2.密铺怎么建？
密铺的意思是，传送带可以塞进正常的两根按格点建造的传送带之中。  
密铺不需要蓝图，但蓝图更方便。  
众所周知，按R可以切换建造模式，共三种建造模式。  
按多次R切换为笔直连接。  
![alt text](密铺带1.png)  
在笛卡尔坐标系做一根直线的传送带，两端坐标为原点  和（1，2，0）。  
截取中间一点，删去其他，它的坐标就有0.5了。  
这个点是可以蓝图复制的。  
![alt text](密铺带2.png)  
做两点相同的两点，直线相连，密铺完成。  

同样的办法也可以造出1/3 1/4 1/5的带子。
也可以造出1.5格长的带子。
![alt text](镇楼图.png)

3.传送带耗电量的问题  
传送带不需要电，不会连接电网，而且在黑夜传送带会自动发光。真正的永动机。  
![alt text](白天不懂夜的黑.png)

4.转弯让直行
![alt text](转弯让直行.png)
众所周知，传送带的一个节点，最多有3个输入和1个输出，多一个都不行。  
![alt text](3进1出.png)

最中间的那根会被认为成是同一根带子。  
同一根带子的线路ID是一样的。  
所以想要多个输出，只有依靠其他建筑，比如分拣器，比如四向分流器。  
  
所谓的传送带转弯让直行。因为一般情况下，笔直的带子是同一根，同一个ID。  
同一个ID的带子优先级最高。  
![alt text](转弯让直行-ID.png)

有一般就二般。k字带直线带子就不是同一根。  
![alt text](k字带.png)

当然，和新人解释起来，转弯让直行是最容易解释的。
这个称呼也已经约定俗成。  

转弯让直行被广泛应用于混带、并带、数字电路等。  
最简单的应用就是小太阳。  
路口金棒直行，黑棒转弯。  
有金棒优先用金棒。  
![alt text](金棒.png)
没金棒会尝试黑棒。  
![alt text](黑棒.png)

其他T字带涉及到buffer，空隙，我不懂。  
但是如果2根180，留出足够空隙。  
可以变成一根360这是确定的。  
![alt text](t字带.png)
