# Gene Annotation

#### 徐英泽 2024011267

#### [返回引导页](https://yingzexu-lala.github.io/bioinformatic/)

*******

### 1. 人类基因组的大小以及基本组成是哪些？

​	在2022年之前，人类参考基因组由GRC发布，称为GRCh38。然而该基因组包含151个未知序列，分布于基因组中，包括着丝粒周围和亚端粒区域、扩殖基因阵列和核糖体DNA（rDNA）阵列。[^1]
​	2022年，Science杂志首次发表了人类基因组的完整序列。[^1]这篇文章中发表的基因组称为**T2T-CHM13**，包括了**3,054,815,472 bp （约3.05Gb）的核 DNA** 和 **16,569 bp 的线粒体基因组**。如下图所示，相比于之前的GRCh38基因组，新增约**3400个基因**（大部分为非编码RNA基因），**约5000个转录本**。

![](https://yingzexu-lala.github.io/bioinformatic/image/gene.png)

​	2026年，西湖大学杨剑教授团队发表的一篇文章中，称构建了包含1116个二倍体基因组的泛基因组，发现传统参考基因组遗漏了约 **4.05亿个碱基对**（约占13%）。此外还编目了全谱遗传变异，包括**3540万个小变异**、**110,530个结构变异（SV）**、**485,575个串联重复序列（TRs）**以及嵌入非参考序列中的**86万个嵌套变异**。[^2]

​	截至目前，根据2025年发布的**GENCODE v49**与**GRCh38.p14**，人类基因组总碱基数为为 **3,291,585,349 bp**。[^3]其基本组成如下图所示：

![](https://yingzexu-lala.github.io/bioinformatic/image/annotation.png)

​	**78691个基因**中，含**19433个蛋白质编码基因**、**35899个长非编码RNA基因**、**7563个小非编码RNA基因**、**14701个假基因**以及**649个免疫球蛋白/T细胞受体基因片段**。除了基因外，基因组还含有大量的重复序列。根据**T2T-CHM13**数据，重复序列（repeats）占人类基因组的**53.94%**，其中包括**Satellite（卫星DNA）**、**Simple repeat（简单重复）**、**rRNA**、**LINE**、**SINE **、**LTR**等。[^1]

### 2. 基因中的非编码 RNA的最新注释是多少个了？请详细列一下其中的非编码 RNA 的细分类型的数目，并对主要的非编码 RNA 是做什么的用1-2句解释一下。

​	根据2025年发布的**GENCODE v49**与**GRCh38.p14**，共**35899个长非编码RNA基因**、**7563个小非编码RNA基因**，细分为**13种非编码RNA**。[^3]根据**GENCODE v49**的详细biotype分类，各非编码RNA的细分类型如下：

| 亚型 | 基因数 | 功能简介 |
|:---:|:---:|:---:|
| **lncRNA** | **34880** | 表观遗传调控、转录调控等 |
| **miRNA** | **1879** | 通过与mRNA的3'UTR结合抑制翻译或促进mRNA降解 |
| **snoRNA** | **942** | 主要定位于核仁，指导rRNA、tRNA和snRNA的化学修饰 |
| **rRNA** | **47** | 核糖体的结构和催化组分，直接参与蛋白质合成中的肽键形成 |
| **tRNA** | **535** | 携带特定氨基酸，在翻译过程中将mRNA密码子解码为氨基酸 |
| **snRNA** | **1901** | 参与pre-mRNA的剪接加工，作为剪接体的核心组分识别剪接位点 |
| **scaRNA** | **49** | 定位于卡哈尔体（Cajal body），指导snRNA的修饰 |
| **vault_RNA** | **4** | 构成穹窿体核糖核蛋白复合物的RNA组分 |
| **ribozyme** | **8** | 具有催化活性的RNA分子，可催化RNA链的切割和连接反应 |
| **misc_RNA** | **2207 **| 杂项非编码RNA |
| **sRNA** | **5** | 其他未分类的小非编码RNA |
| **mt_rRNA** | **2** | 核糖体的结构和催化组分，直接参与蛋白质合成中的肽键形成 |
| **mt_tRNA** | **22** | 携带特定氨基酸，在翻译过程中将mRNA密码子解码为氨基酸 |



[^1]: Nurk S, et al. *The complete sequence of a human genome*. **Science**, 2022. [DOI: 10.1126/science.abj6987](https://doi.org/10.1126/science.abj6987)
[^2]: Wang Y, Duan Z, et al. *The 1000 Chinese Pangenome empowers medical and population genetics*. **Nature**, 2026. [DOI: 10.1038/s41586-026-10315-y](https://doi.org/10.1038/s41586-026-10315-y)
[^3]: GENCODE. *Statistics about GENCODE Release 49 (GRCh38.p14)*. 2025. [Online]. Available at: https://www.gencodegenes.org/human/stats_49.html

