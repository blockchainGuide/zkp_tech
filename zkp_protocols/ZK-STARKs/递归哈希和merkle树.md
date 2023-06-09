## 递归哈希

###  原理

递归哈希是一种哈希函数，可以将原始数据转换为多项式数据。递归哈希过程如下：

1. 将原始数据分为多个分段。
2. 对分段哈希，将结果作为新的分块。
3. 对新的分块哈希，重复2-3步，直到仅剩一个分块。

递归哈希通常基于多项式，如f(x)=xn+an−1xn−1+...+a2x2+a1x+a0*f*(*x*)=*x**n*+*a**n*−1*x**n*−1+...+*a*2*x*2+*a*1*x*+*a*0，其中x*x*为多项式自变量，an−1，...，a0*a**n*−1，...，*a*0为多项式系数。递归哈希可以根据多项式进行，如f(Hi−1)=Hi*f*(*H**i*−1)=*H**i*，其中Hi−1*H**i*−1为输入数据的哈希值，Hi*H**i*为第i*i*个多项式。

###  优点

递归哈希主要优点是具有高度可靠性和安全性。由于其递归性质，递归哈希可以生成不可预测的哈希值，因此很难对哈希值进行暴力破解或伪造。

###  应用

递归哈希在许多应用程序中都有广泛的应用，例如加密货币、数据压缩和安全存储等领域。在加密货币中，递归哈希可以用于构建区块链，确保区块链中数据的可靠性和安全性。在数据压缩中，递归哈希可以用于将原始数据压缩为更小的哈希值，从而节省存储空间。在安全存储中，递归哈希可以用于确保数据在传输过程中的完整性。



## merkle 树

Merkle树是一种数据结构，由哈希值构成，用于快速验证大量数据的完整性和一致性，其在zk-STARKs中的应用主要是用于证明中的数据约束检查和蒙古尔面积证明。

在zk-STARKs中，证明过程是非交互式的，即它仅通过计算来实现。因此，当需要证明的数据量庞大时，通常需要采用一些加速技术来提高证明的效率。Merkle树就是一种很好的加速技术，它可以通过哈希值来快速定位证明数据的位置，同时保证数据的完整性，防止篡改和欺骗。

例如，假设有一个包含1,000,000个元素的数据数组，我们需要证明其中某些元素是否满足某些条件。如果我们将这些元素依次进行哈希计算，最终得到一个哈希值集合，然后构建一个Merkle树，我们就可以通过Merkle树来快速验证证明数据的正确性，避免对整个数据集进行重复计算和检查。

另外，Merkle树也可以应用于蒙德佳尔面积证明，蒙德佳尔面积证明是一种计算图形面积的技术，通常用于验证计算过程的正确性。在zk-STARKs中，蒙德佳尔面积证明需要证明一组离散点组成了一个特定的区域，这时可以使用Merkle树来进行区域验证，避免重复计算和不必要的计算。

总之，Merkle树在zk-STARKs中的应用主要包括数据约束检查和蒙德佳尔面积证明。通过哈希值和Merkle树的快速查找和验证功能，可以提高证明过程的效率和安全性。