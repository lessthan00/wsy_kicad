[远程手指 参考](https://item.taobao.com/item.htm?abbucket=16&id=833846252278&ns=1&priceTId=213e382717355496226727759e0600&skuId=5582785377783&spm=a21n57.1.hoverItem.3&utparam=%7B%22aplus_abtest%22%3A%222645ff784be81bc2db9027298f363181%22%7D&xxc=taobaoSearch)

软件
1. 简易客户端开发
2. 指令服务端开发
硬件部分
3. 指令接收、处理部分
4. 电机控制部分

## [ESP8266](https://item.taobao.com/item.htm?abbucket=8&id=581718021666&ns=1&pisk=gSNo3Sc0d8k5wvr92ol5CYozS66x2UGIFkdKvXnF3moXwvodFkD3voMUwbU8mDrTx2F89W2XtPaQwaGdPbaSOXSOX1F3PzGC4tKZI70qu2a2ULRFHjSJuXfAX1CTPTuS9rSTwvQwAVu9TXkrLmzqc2meavrE3IuI0Quea2-Vo2iqT2oEUnRq-VOyTBregEuK54-ETvl23V0tTDrETZ4qZk6rVWP4gicnNeFmJEFxrYmaz0z82S-xnLajmIA4i-Drb1nDTBPmzre9AoAGpcys2Ana0sdotru32mEN_IcqIRaK-ufkabe4h7G8MGxKEkmrpSDD4LuiZ0Daax5OlrkUnSc8aM9_krmrIjeAhgHKZu2sfYWfck4m2kPo33jxvRUYaxqNDIqIKRaK-ufkalSPUKJNMSdIuwF2dpMrlqmOvE9lja6iTx_cod7IUqgSXZbDdpMrlqmOoZvNOYujPcC..&priceTId=2147823017355725984758642ebc08&skuId=4061882779590&spm=a21n57.1.hoverItem.2&utparam=%7B%22aplus_abtest%22%3A%22517b8673f2726b9f3fd54ad2eeca3ba9%22%7D&xxc=taobaoSearch)
## [ESP8266 ESP-12F](https://www.jlcsmt.com/lcsc/detail?componentCode=C82891)

## 需求
```
wifi控制
按动开关，短按，长按
```
## 实现
```
ESP8266 集成wifi 和 MCU
MQTT协议发送指令
MCU发送PWM控制舵机SG90
SG90做手指动力.

3.7V锂电池包供电,需要省电
ESP-12F light sleep mode current consumption 2mA
舵机电源通过NMOS 关断.

arduino IDE and vscode and cursor ai 写嵌入式code.

软件逻辑
初始化

light mode

get messeg form wifi by MQTT协议

run mode

GPIO14 servos power on

GPIO4 PWM servos

GPIO5 电压拉低说明 接触到按钮

send meeseg to sever by MQTT

得到按下的时间和深度

GPIO4 控制 PWM servos执行。

记录本次运行的数据，比如前行了多少，返回多少。

根据记录的数据，返回到原位置。

把记录的数据发送到sever

GPIO14 servos power off

light mode
```







