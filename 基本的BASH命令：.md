###### 1.虚拟目录简介

在Linux PC上安装的第 一块硬盘称为根驱动器。根驱动器包含了虚拟目录的核心，其他目录都是从那里开始构建的。

Linux会在根驱动器上创建一些特别的目录，我们称之为挂载点（mount point）。挂载点是虚拟目录中用于**分配额外存储设备的目录**。虚拟目录会让文件和目录出现在这些挂载点目录中，然而实际上它们却存储在另外一个驱动器中

![image-20220709124259301](D:/TYPIC/image-20220709124259301.png)

`图3-2展示了计算机中的两块硬盘。一块硬盘和虚拟目录的根目录（由正斜线/表示）关联起 来。剩下的硬盘就可以挂载到虚拟目录结构中的任何地方。在这个例子中，第二块硬盘被挂载到 了/home位置，用户目录都位于这个位置。`



虚拟目录是让整体看起来是一体的，在一个系统内，其实很多目录并不在同一个存储设备里面。



###### 2.通用的目录名

![image-20220709124943845](D:/TYPIC/image-20220709124943845.png)



`简述下设备节点，Linux为系统上的每个设备都创建一种称为节点的特殊文件。与设备的所有通信都通过设 备节点完成。每个节点都有唯一的数值对供Linux内核标识它。数值对包括一个主设备号和一 个次设备号。类似的设备被划分到同样的主设备号下。次设备号用于标识主设备组下的某个特 定设备。`



在登录系统并获得一个shell CLI提示符后，会话将从主目录开始。主目录是分配给用户账户 的一个特有目录。用户账户在创建之后，系统通常会为其分配一个特有的目录



###### 3.Linux手册

除了对节按照惯例进行命名，手册页还有对应的内容区域。每个内容区域都分配了一个数字， 从1开始，一直到9，如表3-2所示

![image-20220709125239292](D:/TYPIC/image-20220709125239292.png)



