# plot_example
## /depth/
depth文件夹下包含与测序深度相关的数据结果。
### OG170250216N1LEUD2kx9b1.boxplot_panel_depth.png
目标捕获区域测序深度的箱线图：共411个不连续的目标捕获区域，每个区域的箱线图展示了该区域的深度的范围（中位数，四分位数和异常点），箱线图的颜色展示了目标捕获区域的宽度，从图中可知某些区域的深度的范围较分散，波动大，且深度偏低（或高），以提示数据的异常。
### OG175910119T1CFD20kx11b1.panel_depth_samtools.png
测序深度展示图：按染色体分类，分别展示数据的深度在染色体上的分布情况，红色表示该部分数据在目标捕获区域内，蓝色表示在目标捕获区域外（为无用数据，且表明捕获的特异性不高），绿色表示经过一定的筛选条件，在目标捕获区域外出现的异常数据，由此图可检测数据的捕获覆盖度和深度是否异常。
### OG175910119T1CFD20kx11b1.panel_abnormal_samtools.bed
异常数据输出：上述提到的异常数据的位置信息。



## /panel/
### ALK.pn
ALK基因上靶点的分布情况：划分的每块小图代表靶点所处的外显子，蓝色线段是该外显子的位置信息，红色线段为目标捕获区域的位置信息，黑色点为靶点所在位置，靶点上的文字为该靶点所影响的蛋白质信息。


### CA-PM.gc_depth_boxplot.png
每根探针上测序深度和GC含量（G碱基和C碱基的和占所有碱基的百分比，衡量数据质量的重要指标）的分布图，图的上半部分（y=0以上）为GC含量的箱线图加散点图，红色三角形为标准GC含量，不同颜色的圆点代表不同批次数据的GC含量，箱线图展示了GC含量的范围（中位数，四分位数和异常点）；图中间部分的蓝色线段表示相邻探针间是否存在重叠，每一根蓝色线段代表其所覆盖到的探针间有重叠部分；图的下半部分（y=0以下）为测序深度经过数据变换后得到的值，不同颜色的菱形点代表不同批次的测序深度，箱线图展示了测序深度的范围（中位数，四分位数和异常点）。该图可以提示哪些探针存在异常。

### abnormal_needle.png
异常探针的分布情况，经过阈值的筛选，进一步直观提示异常探针，横坐标为异常探针的位置，纵坐标为批次信息，点的颜色表示在该批次中出现异常的样本数量。
### abnormal_needle_output.txt
异常探针在不同批次数据中的具体呈现，表明了探针捕获存在异常的具体方面，有利于进一步调整实验方法。

### depth_gc.png



## /qc/
数据质量评估体系中各具体指标的展示。
### coverage.png

### gc.png


### mutation_bar.png


### mutation_heat.png

### signature.png
