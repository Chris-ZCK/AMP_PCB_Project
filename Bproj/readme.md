<!--
 * @Author: your name
 * @Date: 2020-05-31 23:00:52
 * @LastEditTime: 2020-06-16 17:06:20
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \undefinedd:\项目\动物监测2019N\硬件\01 PCB绘制\AMP_PCB_Project\Bproj\readme.md
-->

# 野生动物监测系统硬件设计B版本

B版本是一个精简的版本，移除大部分暂时不用的接口，但是，设计的时候会尽量流出引脚，便于测试工作。
B版本也是为了结项为设计的。
相比于A版本，B版本有如下几个改进:

1. 电源采用12V输入，降压为3.3V分别给4G和控制器供电，降压为5V给传感器供电。
2. 电源线考虑其通电能力，加粗设计。
3. MP1584DN部分预留一定的空间。
4. 本次设计丝印层、元器件位置等，需要便于手动焊接。

## 文件布局

原理图
库文件
嘉立创的库

## 焊接说明

所有的Circuit Break均不需要焊接，调试通过后我亲自焊接。

## 绘制过程

1.sch基本确认完成，有如下改变：

* 加入有源晶振。
* 加入电源测试点。
* 优化了元器件封装，尽可能符合“嘉立创”的标准。
* 重命名部分引脚-ref："/doc/Camera7nd pin define.xlsx"/。
* 电源部分的逻辑关系-ref:"/doc/Power_map.xmind"。
* 移出冗余部分，保留核心功能。
* 将所有元器件库保存至本地库，并确认乐所有的封装。
* 编译通过无错误。
* 尽可能使用防反插接插件。
* 优化了所有的3D元器件库。
* 串口部分可以使用MicroUSB连接电脑。

2.冗余部分

* 实时时钟晶振部分。
* 多了一个串口6。
* 多了ADC采集部分。
* 多一个IIC接口。

3.库文件
移除了正点原子库和嘉立创的库，用到的部分直接移动到了私有库。

4.pcb绘制

## 材料购买
