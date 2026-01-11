# 关于PCB
## 文件说明
*.epro2: 立创EDA项目文件

`XTAL_RC/*`: 只使用一个简易RC滤波的版本，成本较低，但增益值非常高时能出现一些干扰信号（这些干扰在原版PCB上也会出现）。

`XTAL_LPFOB/*`: 使用两个运放进行高阶滤波，成本较高，高增益下的抗干扰效果略好。

两个版本的有源晶振均可以不焊接，使用AG32内部晶振替代（此时建议使用AGM DAP-LINK以校准内部晶振），对应烧录使用外部晶振或内部晶振的固件即可。

## 制作说明
嘉立创PCB制作参数：4层（JLC04081H-3313），板厚0.8mm，沉金。

## BOM说明
待更新

# About the PCB
## File Descriptions
`*.epro2`: EasyEDA (LCSC) project file.

`XTAL_RC/*`: A version utilizing a simple RC filter. This version is more cost-effective; however, at very high gain settings, some noise signals may occur (note: these noise are also present on the original PCB design).

`XTAL_LPFOB/*`: A version utilizing two OpAmps for high-order filtering. The cost is higher. It offers slightly better signal at high gain settings.

For both versions, the crystal oscillator is optional. You may omit it and use the AG32’s internal oscillator instead. If choosing this route, it is recommended to use the **AGM DAP-LINK** to calibrate the internal oscillator; make sure you flash the firmware corresponding to either the internal or external oscillator as appropriate.

## Manufacturing Instructions
**JLCPCB Manufacturing Parameters:**
* **Layers:** 4-Layer (Stackup: JLC04081H-3313)
* **Board Thickness:** 0.8mm
* **Surface Finish:** ENIG

## BOM (Bill of Materials)
To be updated.
