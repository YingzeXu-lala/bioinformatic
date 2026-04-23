# 上机作业 Iris_Plot_with_R

#### 徐英泽 2024011267

#### [返回引导页](https://yingzexu-lala.github.io/bioinformatic/)

*******

### 0. 加载Iris数据集

```R
> library(ggplot2)
> data(iris)
```

### 1.Violin Plot

```R
> p <- ggplot(iris, aes(x = Species, y = Sepal.Length, fill = Species))+
# 参数中横轴为Species，纵轴为Sepal.Length，填充颜色按照Species分组。

+ geom_violin(trim = FALSE, alpha = 0.7)+
# 绘制violin图，不修剪尾部，设置透明度为0.7。

+ stat_summary(fun = median, geom = "point", size = 2, color = "white")+
# 计算中位数，以点的形式展示，颜色为白色，大小为2。

+ stat_summary(fun = quantile, fun.args = list(probs = c(0.25, 0.75)), geom = "point", size = 1, color = "white", alpha = 0.5)+
# 计算四分位数，选取上下四分位数，颜色白色，大小1，透明度0.5，与中位数点区分。

+ labs(title = "Sepal Length Distribution", 
+      x = "Species", 
+      y = "Sepal Length") +
# 设置x轴、y轴、标题的标签。

+ scale_y_continuous(limits = c(3, 9)) +
# 控制 y 轴（连续变量）的刻度、范围在3-9之间。

+scale_fill_manual(values = c("#C44E52", "#55A868", "#4C72B0")) +
# 按变量水平顺序，依次赋予颜色。

+theme_minimal() +  
# 使用简洁主题

+ theme(plot.title = element_text(hjust = 0.5, face = "bold"))
# 标题对齐居中，字体加粗。

> print(p)

```

### 2.保存图形

```R
ggsave("C:/Users/54727/Desktop/sepal_length_violin_plot.png", 
+        p, width = 8, height = 6, dpi = 300)
```
### 3.结果

![](https://yingzexu-lala.github.io/bioinformatic/image/sepal_length_violin_plot.png)
