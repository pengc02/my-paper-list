![[image-20231104114714570.png]]


SfM：
Structure-from-Motion（SfM）的出现使得一组照片即可用于合成新视图。SfM可估算相机校准期间的稀疏点云，最初用于3D空间的简单可视化。
本质上是一些角点之类的关键点，把这些关键点作为稀疏点云，在这里是用来初始化。


assume each point is a small planar circle with a normal

$$
G(x)=e^{-\frac{1}{2}(x)^T \Sigma^{-1}(x)}$$

3D高斯点云中的每一个点里面储存了：位置坐标，协方差矩阵（决定高斯形状），不透明度（用于Splatting），球谐函数（拟合视角相关的外观）。


![[image-20231104152858267.png]]

自适应地调整点云密度。



![[image-20231104154047002.png]]

