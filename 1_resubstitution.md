## Extending Boolean Methods for Scalable Logic Synthesis

#### 参考文献

[1] [2]系列  还 tm 有Boolean filtering 的内容

[6] ABC

[8] permissible function

[26] [27] a method to cast don’t cares computation into a SAT problem is presented.

[32] [33] Maximum Fanout Free Cone[MFFC] of n

[34]  The method in uses BDDs and permissible functions to build fast resubstitution techniques.

[35]  Miyasaka et al. have presented a method that uses a BDD-package without variable re-ordering to accelerate the computation of permissible functions.

 [26], [27] Concerning SATbased resubstitution methods, the works in consider SAT-based don’t cares computation aiming at resubstitution frameworks.

[19], [36] Resubstitution within ABC is a technology independent version of the works in [19], [36] and it is applied to small windows of logic (up to 16 inputs) to contain the runtime complexity.

[38] The window is built

[14] voter benchmark of the EPFL suite

[6] ABC 的resub相关问题 （做resub的优化一个基准问题）

#### 特殊名词汇集：

+ Forward Functional Flexibility (FFF)  ?

+ Maximum Set of Permissible Functions (MSPF) ?

+ K-resubstitution :is a generalization of resubstitution  which adds exactly k new nodes and removes l nodes, where l is the number of nodes in the Maximum Fanout Free Cone **(MFFC)** of n. In this case, size improvement？

+ scalability, we refer to the runtime complexity of our algorithms

#### 核心汇集：

1. The idea behind Boolean methods is to use the **power of Boolean algebra together with the degree of freedom provided by the don’t cares** to construct local transformations to improve logic networks .

   Boolean methods consider the true nature of logic functions by considering Boolean identities and **don’t cares**

+ (外部无关项)external don't cares(详细 sub_don‘t care专题)

  + Satisfiability don't care 

    + belong to the wires inside the Boolean logic network
  + controllability don't cares
    + defined as those input patterns that are never produced by the environment
  + observability don't cares
    +  latter considers situations when a given output is not observed by the environment


#### 论文研究方案

+ ##### Method 1 ：

  + resubstitution method that uses **novel Boolean filtering** and **windowing techniques** to speed up the computation [1]细节参考

    + Boolean filtering（模糊）

    + windowing techniques（待参考）

    + **resubstitution flow for complex gates**（对前边铺垫的应用）

      ![method 1](C:\Users\lsazy\Pictures\Saved Pictures\method 1.png)

      



​	