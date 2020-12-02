## 1:简答：

#### 		自动识别技术的分类有哪些？

> 答：光符号识别技术、语音识别技术、生物计量识别技术、IC卡技术、条形码技术、射频识别（RFID）技术

#### 		什么是ISBN条形码？新版 ISBN 码由几位数字组成？

> 国际标准书号，简称ISBN，是专门为识别图书等文献而设计的国际编号。新版ISBN码由**13**位数字组成（978 + 组号 + 出版社号 + 书名号 + 校验号）。

#### 		简述RFID系统中，读写器与标签之间是怎样进行无线通信的。

> 在RFID系统中，读写器产生**高频振荡能量**，经过传输线传输到发射天线，然后以**电磁波形式**向预定方向辐射。接收天线则将接收到的电磁波能量通过**馈线**送到标签，完成无线电波传输的过程。

#### 		什么是副载波调制，副载波调制在RFID系统中起什么作用

> 副载波调制是指首先把信号调制在载波1上，出于某种原因，决定对这个结果再**进行一次调制**，于是用这个结果去调制另外一个频率更高的载波2。副载波调制在RFID中起到**通信，供电的作用。**

#### 曼彻斯特码如何检测数据传输中的错误？

> 当多个电子标签同时发送数据位有不同时，接收的上升边和下降边互相抵消，
>
> 导致在整个位长度副载波信号是不跳变的，改状态是不允许的，可判断为发生碰撞。

#### 		指出下图描述分别是哪种调制方式，简述这三种调制方式的特点。

> ![image-20201127225459389](C:\Users\jack\AppData\Roaming\Typora\typora-user-images\image-20201127225459389.png)
>
> 分别为ASK，FSK和PSK。
>
> **ASK:** 即按载波的幅度受到数字数据的调制而取不同的值。调幅技术实现起来简单，但容易受增益变化的影响，是一种低效的调制技术。
>
> **FSK:** 即按数字数据的值（0或1）调制载波的频率。。该技术抗干扰性能好，但占用带宽较大。在电话线路上，使用FSK可以实现全双工操作，通常可达到1200bps的速率。
>
> **PSK:** 即按数字数据的值调制载波相位。这种调制技术抗干扰性能最好，且相位的变化也可以作为定时信息来同步发送机和接收机的时钟，并对传输速率起到加倍的作用。

#### 		通信系统中为什么要进行调制和解调？调制的分类方法有哪些？

> 答：**调制器 **用于*改变高频载波信号，使得载波信号的振幅、频率或相位与要发送的基带信号相关*。**解调器**的作用则是*解调获取到的信号，以重现基带信号*。调制的分类方法包括***振幅键控***、*频移键控*、*相移键控*和*副载波调制*。

#### 		RFID面临的攻击有哪些？

> 1.电子标签数据的攻击
>
> 2.电子标签和读写器之间的通信侵入
>
> 3.侵犯读写器内部的数据
>
> 4.主机系统侵入

#### 		RFID系统安全解决方案

> **物理方法**：杀死标签，法拉第网罩，主动干扰，阻止标签
>
> **逻辑方法**：Hash锁，随机Hash锁，Hash链，匿名ID方案和重加密方案

#### 		二进制数型搜索算法为什么选用曼切斯特编码 ?

> 在数据传输过程中，如果两个电子标签同时发送的数位有不同的值，则接收的上升沿和下降沿互相抵消，“没有变化”的状态是不允许的，将作为错误被识别。用这种方法可以按位追溯跟踪冲突的出现，可以检测出碰撞位。

#### 		EPC信息服务（EPCIS）中框架分为几层，每层的作用是什么？

> EPCIS框架被分成三层：**信息模型层，服务层，绑定层**。
>
> **信息模型层：**指定了EPCIS中包含什么样的数据，这些数据的抽象结构是什么，以及这些数据代表着什么含义。
>
> **服务层：**指定了EPC网络组件与EPCIS数据进行交互的实际接口。
>
> **绑定层：**定义信息的传输协议，比如SOAP(简单对象访问协议)或HTTP(超文本传输协议)

#### 		中间件及功能：

> 中间件是一种独立的系统软件或服务程序，分布式应用软件借助这种软件在不同的技术之间共享资源，其位于客户机、服务器的操作系统之上，管理计算机资源和网络通信。其扮演着电子标签和应用程序之间的中介角色，从应用程序端使用中间件提供的一组通用的应该程序接口API，能连到RFID阅读器，读取电子标签数据。
>
> 主要包括四大功能：
>
> （1）阅读器协调控制；  （2）数据过滤与处理；  （3）数据路由与集成；   （4）进程管理。

#### 信源编码的作用是什么？

> 答：设法减少码元数目和降低码元速率，即通常所说的数据压缩；作用之二是将信源的模拟信号转化成数字信号，以实现模拟信号的数字化传输。

#### 请简述RFID技术所具有的的优点。

> 答：**体积小且形状多样：**RFID标签在读取上并不受尺寸大小与形状限制，不需要为了读取精度而配合纸张的固定尺寸和印刷品质。
>
> **耐环境性：**纸张容易被污染而影响识别。但RFID对水、油等物质却有极强的抗污性。另外，即使在黑暗的环境中，RFID标签也能够被读取。
>
> **可重复使用：**标签具有读写功能，电子数据可反复覆盖，因此可以被回收而重复用。
>
> **穿透性强：**标签在被纸张、木材和塑料等非金属或非透明的材质包裹的情况下也可以进行穿透性通讯。
>
> **数据安全性：**标签内的数据通过循环冗余校验的方法来保证标签发送的数据准确性。

#### 简述碰撞的解决方案

> 1）空分多址（SDMA）2）频分多址（FDMA）3）码分多址（CDMA）4）时分多址（TDMA）

#### 简述碰撞的种类

> 阅读器碰撞：多个阅读器同时与一个标签通信，致使标签无法区分阅读器的信号。
>
> 电子标签碰撞：多个标签同时响应阅读器的命令发送信息，使阅读器无法识别标签。

#### 二进制树型搜索算法的基本思想是什么？

> 它的基本思想是不断的将导致碰撞的电子标签进行划分，缩小下一步搜索的标签数量，直到只有一个电子标签进行回应。

#### 简述hush锁方案原理

> Hush锁协议中，标签不使用真实的id，而使用一个metaid代替。标签内部有一个用于存储临时metaid的内存，在锁定状态下，标签用metaid响应所有的查询，在非锁定状态下，标签向阅读器提供自己的信息。

## 2:填空：

1. RFID系统的耦合方式可以分为 **电感耦合**  和  **电磁反向散射耦合**  电感耦合系统中，电阻负载调制通过对  **读写器电压**  调控，最终完成信息的传输。
2.   电感耦合的原理是  **电磁感应原理** ，电磁反射应用的是 **电磁波的空间传播** 规律。
3.    典型的读写器终端一般由 **天线** 、 **射频模块** 、 **逻辑控制模块**  三部分构成。
4. 天线辐射最强的方向所在波瓣称为  **主瓣**  ，其宽度是衡量天线最大辐射区域  **尖锐程度** 的物理量。
5. 波瓣宽度越宽，方向性越  **差** 作用距离越 **近** 抗干扰能力越 **弱** 但是天线的覆盖范围越  **大**  。
6. 天线的种类很多，可以按照多种方式进行分类，其中按照波段可将天线分为：**长波天线**、**中波天线**、**短波天线** 、**超短波天线**、**微波天线** 。
7. ISO/IEC 14443 **近耦合**IC卡，最大的读取距离为*10cm*。ISO/IEC 15693**疏耦合**IC卡，最大的读取距离为*1m*。
8.  目前国际上广泛采用的频率分布于4种波段，**低频**、**高频**、**超高频** 和 微波。它们的典型工作频率分别是*125KHz*、*13.54MHz*、*850MHz～910MFz*和*2.45GHz*。
9.  RFID在低频段（100MHz以下）工作是基于**电感耦合**，在高频段（400MHz以上）工作是基于**电磁反向散射耦合**。
10.  在RFID系统中，为保持数据的完整性，必须采用**差错控制和防碰撞算法**。
11. ISO/IEC 14443标准由 **物理特性**  、 **射频能量**和**信号接口**  、**防初始化和防碰撞**  、 **传输协议** 四个部分组成。
12. EPC系统的信息网络系统是在全球互联网的基础上，通过 **Savant管理软件系统** 、 **ONS对象名称解析服务** 、 **实体标记语言（或EPC信息服务）**  实现全球的实物互联。
13. Savant系统完成的任务是： **数据校对**、 **读写器协调**、 **数据传输** 、 **数据存储** 、 **任务管理**。
14.  国际上具影响力三大RFID标准化体系组织是**EPC Global美**、**UID日本******、** **ISO/IEC标准体系 **。
15. EPCIS在整个EPC网络中的主要作用就是提供  **存储管理EPC捕获信息**  的接口。
16. RFID标准体系主要包括**技术标准**，**数据内容标准**，**性能标准**，**应用标准**。
17. 读写器的主要作用是：**通过天线与RFID电子标签进行无线通信，可以实现对标签识别码和内存数据的读出或写入操作**。
18. 读写器和电子标签之间的数据交换方式也可以划分为两种，分别是**负载调制** 和**反向散射调制**。
19. 差错控制时所使用的编码，常称为纠错编码。根据码的用途，可分为**检错码**和**纠错码**。 
20. 常见的密码算法体制有 **对称密码体系**和**非对称密码体系**两种。 
21. RFID系统中有两种类型的通信碰撞存在，一种是**阅读器碰撞**，另一种是**电子标签碰撞** 。
22. RFID在低频段（100MHz以下）工作是基于**电感耦合**，在高频段（400MHz以上）工作是基于**电磁反向散射耦合**。
23. 二进制树型搜索算法由  **读写器**  控制。
24. ISO/IEC 15693标准中标签有四种可处状态，分别是 **断电**、**准备**、**静默**、**选择**  。
25. ISO/IEC 14443标准由 **物理特性**  、 **射频能量**和**信号接口** 、**防初始化和防碰撞**  、 **传输协议** 四个部分组成。
26. 功率放大器的功率增益指的是**输出功率与输入功率之比**，单位是**分贝** 。
27. 常用在多路存取（多路通信）方式有：**空分多路法、时分多路法、频分多路法**。在RFID系统中，主要采用**时分多路法**
28. 为了防止碰撞的发生，射频识别系统中需要设计相应的防碰撞技术，在通信中这种技术也称为多址技术，多址技术主要分为以下四种：**空/频/码/时分多址**。
29. 二进制树型搜索算法由  **读写器**  控制。
30. TDMA算法又可以分为**基于概率的ALOHA算法**和确定的**二进制算法**两种。上述两种TDMA算法中，会出现“饿死”现象的算法是**基于概率的ALOHA算法**。
31. ISO/IEC、EPCglobal和UID这三个标准组织制定的标准相互之间并不兼容，主要差别在 **通讯方式** 、 **防冲突协议** 和 **数据格式** 三个方面
32. ISO/IEC 14443标准由 **物理特性**  、 **射频能量**和**信号接口**、**防初始化和防碰撞**  、 **传输协议** 四个部分组成。
33. RFID技术具有 **数据的读写机能**  、 **形状小型化和多样化** 、**耐环境性**、**可重复使用**、**数据记忆量大**  等优点。

## 3:选择题

- 下列哪一项不是低频RFID系统的特点？**（A）**

  A、**它遵循的通信协议是ISO18000-3**

  B、它采用标准CMOS工艺，技术简单

  C、它的通信速度低

  D、它的识别距离短(<10cm)

  **【解析】**低频RFID系统遵循的通信协议是*ISO18000-2*，高频RFID系统遵循的通信协议是*ISO18000-3*。

  

- 绝大多数射频识别系统的耦合方式是**（A）**

  **A、电感耦合式** B、电磁反向散射耦合式 C、负载耦合式 D、反向散射调制式

- RFID系统的电感耦合方式可以分为**（A、C）**

  **A、密耦合系统**  B、疏耦合系统  **C、遥耦合系统**  D、近耦合系统

- 目前低成本射频识别系统的主流是**（C）**
  A、密耦合系统   B、疏耦合系统   **C、遥耦合系统**   D、近耦合系统

- 在射频识别系统中，最常用的防碰撞算法是**(C)**

  A、空分多址法  B、频分多址法   **C、时分多址法**  D、码分多址法。

- 在RFID系统中，一般采用**（D）**法来解决碰撞

  A、空分多址（SDMA）  B、频分多址（FMDA） 

  C、码分多址（CDMA）  D**、时分多址（TDMA）**

- ONS服务器由（ **A** ）和（ **B**）两部分组成。

  **A ONS根服务器** **B 本地ONS服务器** C 本地服务器 D 远程ONS服务器
  
- Savant系统可提供以下哪几项功能。**（ A ）**

  **①** **数据校对 ② 数据存储  ③ 任务管理**  ④ 信息捕获  ⑤ 域名解析

  **A ①②③**   B ②③④    C ②④⑤    D ①②⑤

-  ISO/IEC 18000标准系列中包含了（）个部分，18000-7定义的（）频段(**C**)

   A.七、高频 B.七、超高频 **C.六 超高频** D.六 微波

- 纯Aloha算法的碰撞周期为**(B)**

  A.3T     **B.2T**     C.T     D.1.5T

- RFID标准ISO 14223-1（动物的无线射频识别－高级标签第一部分的空中接口）属于哪一类标准（**B**）

  A、技术标准   **B、应用标准**  C、数据内容标准  D、性能标准式

  **【解析】**技术标准：主要定义了不同频段的空中接口及相关参数，包括基本术语、物理参数、通信协议和相关设备等。应用标准：主要涉及特定应用领域或环境中RFID的构建规则。通用标准提供了一个基本框架，应用标准是对它的补充和具体规定。

- 1.   GB/T20563 2006在RFID标准体系中属于（ **D** ）。

  A,技术标准  B .数据内容标准   C.性能标准    **D.应用标准**

## 3:笔记：

1. 修正密勒码为曼彻斯特编码反向的上升沿产生一次波形跳变（一个凹槽），此为密勒码。

2. > 2.将掩码长度和掩码值初始化为零。
   >
   > 3.将插槽号指针初始化为零。
   >
   > 4.发送带有掩码长度和掩码值的库存请求。
   >
   > 5.等待发送中断结束。
   >
   > 6.等待下一个中断。这可能是由于以下任何原因：
   >
   > 一种。接收结束b。碰撞c。没有反应
   >
   > 如果中断是由于RX结束引起的，则意味着FIFO中接收到UID，没有任何错误/冲突。读取FIFO以获得完整的UID。
   >
   > 如果由于冲突导致中断，请在插槽号指针中记下插槽号。递增插槽号指针。
   >
   > 如果中断是由于VICC没有响应而引起的，请忽略。
   >
   > 7.复位FIFO。
   >
   > 8.如果插槽数为16，则发送EOF。如果插槽数为1，则退出。
   >
   > 9.对所有16个插槽重复步骤5和6。在16个插槽的末尾，禁用无响应中断。
   >
   > 10.检查插槽号指针。如果不为零，请计算新的掩码。如果为零，请退出。
   >
   > A.将掩码长度增加4位。
   >
   > B.计算新的掩码=插槽号（发生冲突）+旧的掩码
   >
   > 11.转到步骤4（新的掩码值和长度）。
   >
   > 12.将插槽指针减1。
   >
   > 13.转到步骤10。

## 4:设计题：

1. #### 简述智能公交系统怎样实时将公交位置信息显示在站台显示屏上的。

> 公交车通过站台时，装在公交车顶部的识别卡（RFID）将公交车的车辆身份信息和到站时间无线发送到识别基站，识别基站利用移动通信的GSM或GPRS平台，将车辆信息发送至每条线路的调度室，市级交通管理部门利用各调度室收集的信息来监控市内公交线路的整体质量。通过对公交车辆的识别定位和数据的网络传输，在站台的显示屏上就可以实时显示该条公交线路的运行情况以及下一趟车将要到站的情况。

1. #### 简述基于RFID技术的不停车收费系统的工作流程。

> ETC系统的工作流程：
>
> （1）车主去银行办理ETC速通卡，到高速公路管理部门购置RFID电子标签，并写入相关信息；
>
> （2）发行系统将相关信息输入收费系统。车主将RFID标签贴在车上相应部位；
>
> （3）当车辆进入高速公路ETC通道入口时，该站的RFID读写器发出射频信号，由RFID电子标签的天线接收射频信号，激活RFID电子标签，向电子标签写入入口信息；
>
> （4）当车辆通过高速公路ETC通道出口时，该站的读写器发出射频信号，由电子标签的天线接收射频信号，激活电子标签，读写器读出电子标签中存储的信息。（5）收费计算机系统向执行机构输出执行信号。当速通卡里金额足够支付过站的费用时，出站口绿灯亮，自动栏杆升起，给予放行。
>
> （5）收费完成。

## 5:翻译：

1：The following figure shows the memory map of ATA5577C.

The memory is a 363-bit EEPROM, which is arranged in 11 blocks of 33 bits each. Each block includes a single lock bit, which is responsible for write-protecting the associated block. Programming takes place on a block basis, so a complete block (including lock bit) is programmed with a single command. The memory is subdivided into two page areas:

![img](https://mooc1-1.chaoxing.com/js/editor20150812/themes/default/images/spacer.gif)• Page 0 contains eight blocks

• Page 1 contains three blocks

All 33 bits of a block, including the lock bit, are programmed simultaneously. Block 0 of page 0  contains the mode/configuration data, which are not transmitted during Regular-Read mode operations.

Addressing block 0 always affects block 0 of page 0  regardless of the page selector. Block 7 of page 0  may be used as a protection password. Block 3 of page 1 contains the AFE Option register, which is also not transmitted during Regular-Read mode operation. Bit ‘0’ of every block is the lock bit for that block.

Once locked, the block (including the lock bit itself) is not reprogrammable via the RF field. Blocks 1 and 2 of page 1  contain traceability data and are transmitted with the modulation parameters defined in the Configuration register after the opcode ‘11’ is issued by the reader. The traceability data blocks are programmed and locked by ATA5577C.

> 下图显示了ATA5577C的内存映射。
>
> 该存储器是一个363位EEPROM，它分为11个块，每个块33位。每个块都包含一个锁定位，该锁定位负责对相关块进行写保护。编程是基于块进行的，因此可以使用单个命令对整个块（包括锁定位）进行编程。内存分为两个页面区域：
>
> •页面0包含八个块
>
> •第1页包含三个块
>
> 块的所有33位（包括锁定位）均被同时编程。第0页的块0包含模式/配置数据，在常规读取模式操作期间不会发送该数据。
>
> 无论页面选择器如何，寻址块0始终会影响页面0的块0。第0页的块7可用作保护密码。第1页的块3包含AFE选项寄存器，在常规读取模式操作期间也不会发送该寄存器。每个块的位“ 0”是该块的锁定位。
>
> 一旦锁定，该块（包括锁定位本身）就不能通过RF字段重新编程。第1页的块1和2包含可追溯性数据，并在读取器发出操作码“ 11”后，使用配置寄存器中定义的调制参数进行传输。可追溯性数据块由ATA5577C编程和锁定。

During transmission, the FIFO is checked for an almost-empty condition, and during reception for an almost-full condition. The maximum number of bytes that can be loaded into the FIFO in a single sequence is 12 bytes.

 During transmission, the MCU loads the TRF7960A FIFO (or, during reception, the MCU removes data from the FIFO), and the FIFO counter counts the number of bytes being loaded into the FIFO. Meanwhile, the byte counter keeps track of the number of bytes being transmitted. An interrupt request is generated if the number of bytes in the FIFO is less than 3 or greater than 9, so that MCU can send new data or remove the data as necessary. The MCU also checks the number of data bytes to be sent, so as to not surpass the value defined in TX length bytes. The MCU also signals the transmit logic when the last byte of data is sent or was removed from the FIFO during reception. Transmission starts automatically after the first byte is written into FIFO

> 在发送过程中，检查FIFO是否为空，而在接收过程中检查为几乎满。 单个序列中可装入FIFO的最大字节数为12个字节。
>
>   在发送过程中，MCU加载TRF7960A FIFO（或在接收过程中，MCU从FIFO中删除数据），并且FIFO计数器对正在加载到FIFO中的字节数进行计数。 同时，字节计数器跟踪正在传输的字节数。 如果FIFO中的字节数小于3或大于9，则会生成一个中断请求，以便MCU可以根据需要发送新数据或删除数据。 MCU还检查要发送的数据字节数，以不超过TX长度字节中定义的值。 当数据的最后一个字节被发送或在接收期间被从FIFO中删除时，MCU还向发送逻辑发出信号。 在第一个字节写入FIFO之后，传输自动开始

1. Anti-Collision Sequence for ISO15693

The following describes the inventory procedure/anti-collision sequence for the ISO15693.

The VCD sends a mask value and number of slots along with the inventory request. The VICC compares the least significant bits of its UID to the slot counter + mask value. If it matches, it sends a response. If only one VICC responds, then there is no collision and the VCD receives the complete UID. If the reader detects a collision, it makes note of the slot number in which collision occurred. The reader sends an EOF to switch to the next slot. The VICC increments its slot counter on reception of EOF. This is repeated for all 16 slots. At the end of 16 slots, the slot pointer contents are examined. If it is not zero, it means that collision has occurred in one or more slots. A new mask value is calculated and the inventory request is sent with the new mask. This is repeated until there are no collisions.

> ISO15693的防撞序列
> 下面介绍了ISO15693的清点程序/防撞顺序。
> VCD随清单请求一起发送掩码值和插槽数。 VICC将其UID的最低有效位与时隙计数器+掩码值进行比较。 如果匹配，则发送响应。 如果只有一个VICC做出响应，则不会发生冲突，并且VCD会接收到完整的UID。 如果读取器检测到冲突，则会记下发生冲突的插槽号。 阅读器发送EOF切换到下一个插槽。 VICC在接收到EOF后递增其时隙计数器。 对所有16个插槽重复此操作。 在16个插槽的末尾，将检查插槽指针的内容。 如果不为零，则表示冲突发生在一个或多个插槽中。 计算新的掩码值，并与新的掩码一起发送库存请求。 重复进行直到没有碰撞为止。