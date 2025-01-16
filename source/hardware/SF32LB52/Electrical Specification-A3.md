#### 处理器供电要求

```{table} 电源供电要求
:align: center
:name: sf32lb52x-B--POWER

|电源管脚| 最小电压(V) | 典型电压(V) | 最大电压(V) | 最大电流(mA) |   详细描述 |
|:--|:--|:--|:--|:--|:----------------------------------------------------|
|VBUS       |4.5    |5.0    |5.5    |500    |VBUS电源输入 
|VBAT       |3.5    |-      |4.6    |500    |VBAT电源输出
|VCC        |3.5    |-      |4.6    |500    |系统电源输入
|VSYS       |-      |3.3    |-      |500    |VSYS电源输出{sup}`(1)`   
|BUCK_LX    |-      |1.25   |-      |50     |BUCK输出脚，接电感 
|BUCK_FB    |-      |1.25   |-      |50     |BUCK反馈和内部电源输入脚，接电感另一端，且外挂电容 
|VDD_VOUT1  |-      |1.1    |-      |50     |内部LDO，外挂电容 
|VDD_VOUT2  |-      |0.9    |-      |20     |内部LDO，外挂电容 
|VDD_RET    |-      |0.9    |-      |1      |内部LDO，外挂电容 
|VDD_RTC    |-      |1.1    |-      |1      |内部LDO，外挂电容 
|VDD18_VOUT |-      |1.8    |-      |30     |SIP电源{sup}`(2)` 
|VDD33_VOUT1|-      |3.3    |-      |150    |3.3V LDO 输出1{sup}`(3)`
|VDD33_VOUT2|-      |3.3    |-      |150    |3.3V LDO 输出2
|AVDD33_AUD |3.15   |3.3    |3.63   |50     |3.3V音频电源输入 
|AVDD_BRF   |3.15   |3.3    |3.63   |100    |射频电源输入 
|MIC_BIAS   |1.4    |-      |2.8    |-      |MIC电源输出 

```
:::{note}

{sup}`(1)` VSYS电源，给AVDD_BRF供电 

{sup}`(2)` VDD18_VOUT电源 \
SF32LB520U36，外供3.3V电源 \
SF32LB523UB6，SF32LB525UC6，SF32LB527UD6，使用内部LDO，不需要外供电源 

{sup}`(3)` VDD33_VOUT1电源 \
SF32LB520U36，给VDD18_VOUT、外挂Flash和AVDD33_AUD供电 \
SF32LB523UB6，SF32LB525UC6，SF32LB527UD6，给外挂Flash和AVDD33_AUD供电

:::