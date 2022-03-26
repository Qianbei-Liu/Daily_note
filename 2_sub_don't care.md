#  Don't cares

## Base digital design

+ ### Don't care = an input pattern that never happen in multi -level

+ ### Different in multi-level

  1. arise implicitly

  2. example 大概了解 satisfiability Don't care /controllability Don't care/observability don't cares

  3. 由网络后级（POS）向前的don't cares 简化

  4. example：![image-20220315155916732](C:\Users\lsazy\AppData\Roaming\Typora\typora-user-images\image-20220315155916732.png)

  5. Satisfiability don't care 

     + belong to the wires inside the Boolean logic network

  6. Controllability don't care（待完成）

     + patterns that cannot happen at inputs to a network node

  7. Observability don't cares（待完成）

     + Patterns input to node that make network outputs insensitive to outputs insensitive to  output of the node 
     + Patterns that "mask"outputs

  8. How to represent don't care patterns at a node?

     + As a Boolean function that make a 1 when the **pattern** is impossible

       + ###### represent

         If the function is F ,with inputs (a,b,c,...) write as :SDC(F,a,b,c...) =1

         The SDC represents **impossible patterns** of input to and output of each node

         SDC就是一根线表示 F 的output,不可能等于1 的输入的情况(pattern)

       + ###### Compute：Easy comepute an SDC for each output wire for each internal Boolean node。

         expression that F ==1

         when x ≠（Boolean expression for x）
  
         so X ⊕（expression for X）
  
         ![image-20220315204647072](C:\Users\lsazy\AppData\Roaming\Typora\typora-user-images\image-20220315204647072.png)
  
     + This is often called a Don't Care Cover 
  
     + So each SDC CDC ODC is really just another Boolean function,in thos strategy
  
     