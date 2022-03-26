## Boolean Decompositions

#### Shannon Expansion

+ Cofactor
  + positive Cofactor
  + negative Cofactor

+ Shannon Expansion Theorem (证明)

  + Give any Boolean function F(x1,x2,...,xn)and pick any xi inF()'s input F() can be represented as F(x1,x2,...,***xi,***......,xn)= ***xi***•F(***xi***=1)+***xi'***•F(***xi***=0)
  + mux形式
  + Multiple Variables
    + 一个方程写两项，两项变四项

+ Boolean difference

  + properties of Cofactors

    + Complements
    + and
    + or
    + exor

  + boolean 微分表示df/dx = exor of the Shannon cofactors with respect to x(布尔微分性质)

    + df/dxdy = df/dydx   (order)

    + d(f ⊕g)/dx = df/dx⊕dg/dx (异或的微分等于微分的异或)

    + if function f is actually constant(f=1 or f= 0,always for all inputs)                                                                                   df/dx = 0 for any x

    + 布尔微分的实际应用：当df/dx = 1时，如果x改变呢f必改之，f对x 的灵敏性（sensitive）

      + 例：与门f = xy   df/dx = y  if y = 1 则when  *x* wiggle *f* chang

        ​		或门，异或门

    + ![adder](C:\Users\lsazy\Pictures\Saved Pictures\adder.png)                               

      计算dcout/dcin =？全加器的问题（待解决）

+ Quantification operator (quantification away)
  + Universal  Quantification（原理） 
  + Existential Quantification （原理） 
  + 对于Universal Quantification and Existential Quantification 的应用：Network Repair
    + 操作时用上技巧（function property）

+ Recursive tautology

  + cube 表示方法 SOP

  + use a 3-var Boolean cube ,with solid circles where  f() = 1

  + each product term (circle in a Kmap) called a " cube " ==2 的 k次幂 corners circled

  + 标号之后加表示Position cube notation

    <img src="C:\Users\lsazy\Pictures\Saved Pictures\PCN.png" alt="PCN" style="zoom:50%;" />

    a' = [10 11 11]

    bc = [11 01 01]

    ![represent func](C:\Users\lsazy\Pictures\Saved Pictures\represent func.png)

  + if f  tautology both pos neg  tautology are  tautology 可证

  + Recursive Cofactoring 接cube 表示方程f  一个方程里好几个 cube 例如 f = abd+a'b 两个cube

    cube里 f 中 对于x =1 时 10 删 ，01 改11， 11(表示不含x)不动

    cube里 f 中 对于x = 0时 01 删，10改11，11(表示不含x)不动

  +  Unate function is SOP representation  单调性

    f 中的所有单字只含有一极 true or complemented

    like： f = ab+ac'd+c'de'

    postive unate   in var x changing *x* 0→1 f  constant or make f : 0→1

    negtive unate   in var x changing *x* 0→1 f  constant or make f : 1→0
