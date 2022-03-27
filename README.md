# DATA620004_Homework1
This repository conclude the homework1 of the course DATA620004

我们的代码主要为三个文件，分别是twolayer.py,selection.py和test.py
其中twolayer.py包含了我们训练的大部分代码，包括激活函数，反向传播，loss以及梯度的计算，学习率下降策略，L2正则化，优化器SGD，及保存模型等代码，同时twolayer.py的主函数中也包含了训练代码，如果读者想要用我们的网络进行训练，可以修改相关的参数后，运行主函数即可；除此之外，twolayer.py也包括了可视化的部分，当我们运行主函数的时候，我们也会展示我们的模型在训练过程中训练损失，测试损失和测试准确性的变化，以及网络每层参数的可视化。

selection.py主要包含了关于参数选择的代码，我们查找的参数为学习率，隐藏层大小，正则化强度。对于每个参数，我们给了他们可选的值一个列表，读者可以修改这三个列表来改变我们的参数选择范围，随后运行即可。

test.py主要是用来加载模型并在测试集上计算分类精度，在我们的twolayer.py中包含了保存模型的函数，保存在一个npz文件中，读者只需要把test.py中的npz文件改为自己保存的模型文件并运行，即可加载改模型，并得到该模型在测试集上的分类精度。

剩余文件中,save_model.npz是我们保存的最终模型的参数；selection.txt是我们在参数选择中记录的使用不同参数组在验证集上的不同分类精度；两个png文件分别是用我们最终的模型在训练时得到的在训练集上的损失，测试集上的损失，测试集上的分类精度随着迭代轮次变化情况，以及网络每层参数的可视化
