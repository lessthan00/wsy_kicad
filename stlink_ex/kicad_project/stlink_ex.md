# stlink v2 转接板

## 标准20针(2×10)IDC插座

https://www.waveshare.net/wiki/ST-LINK/V2_(CN)

IDC-20P 2.54mm间距 2X10双排

简易牛角2.54mm直针座排线插头JTAG插座IDC3-6p8P10P12P20P40P50P
简易牛角2.54mm 直针 20P (10只)

### [引脚定义](https://www.st.com/resource/en/user_manual/dm00026748-st-link-v2-in-circuit-debugger-programmer-for-stm8-and-stm32-stmicroelectronics.pdf)

#### Table 4. JTAG/SWD cable connections on STLINK-V2

1. JTAG标准接口信号
JTAG通常包含以下5个基本信号(4线标准接口 + 可选信号)：

信号名  方向(相对于目标设备)	描述
TMS	    输入	    测试模式选择(Test Mode Select),控制JTAG状态机的状态切换.
TCK	    输入	    测试时钟(Test Clock),同步JTAG操作的时钟信号.
TDI	    输入	    测试数据输入(Test Data In),数据或指令从主机输入到目标设备.
TDO	    输出	    测试数据输出(Test Data Out),数据从目标设备输出到主机.
TRST	输入(可选)   测试复位(Test Reset,低电平有效),异步复位JTAG状态机(非必须).



