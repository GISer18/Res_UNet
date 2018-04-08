# Res_UNet
Residual unet

声明： tensorflow 1.2.1 及其之后版本均可以使用。
残差U_Net：主体结构由tensorflow高级轻量级模块（slim）实现。all variables are initialized ! 

结构原创不是本人，本人只是复现了tensorflow版本的残差 U_Net。

与U_Net不同的是 残差模块代替了原来的block（conv+pool），
残差模块没有pool layer，可以减轻由于pool layer带来的伤害。（pool太暴力）

注意：
res_unet尺度变化相当于有4个pool layer，输入大小 128 或者 192 或者 256 比较合适。
