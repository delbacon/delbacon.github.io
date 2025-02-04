cds.lib：设计库管理文件，包含一些基础设计库定义和用户自定义工程库
.cdsinit：包含cadence的初始化信息和快捷键设置

pwd：当前thermal所在文件夹
which virtuoso：virtuoso所在文件夹

在GUI用ctrl+L搜索路径

virtuoso &运行，&是为了在运行virtuoso后仍能使用thermal


mim：电容
rm：电阻
pxx：pmos
nxx：nmos

p33r5：p是pmos，33是最大承受电压

快捷键：
w：wire布线
p：pin引脚
q：修改参数
i：导入元件
f：大小自动适应


定义GND的方法：
1. analog库内有gnd符号
2. L键输入gnd！，默认这条线为gnd


仿真时要调用相关文件，一般在工艺库的models/spectre/，结尾为.scs/.lib/.l

csmc的这个工艺不会自动加载，需手动添加，模型在model文件夹下s05mixdtssa01v11.scs。看model文件夹下的readme.txt文件有关于模型的介绍。
mos管的section 写tt，双极型三极管bjttypical，电阻restypical，电容captypical

注意：库命名一定要和文件夹一样！！！！不然调用的时候会因为和内部定义的库名称变量不同而出问题