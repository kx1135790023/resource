## 项目测试流程

**搭建测试环境(重点)**

快速的熟悉项目

编写测试计划

编写测试方案

**设计、编写、执行测试用例(重点)**

生成测试报告



## 软件测试模型
常见的软件测试模型包括瀑布模型、V模型、W模型、H模型、X模型

#### 1. 传统的瀑布模型——最早出现的软件开发模型
![瀑布模型](/images/01-瀑布模型.jpg)

每一个阶段都是以上个阶段的输出作为下个阶段的输入。

优点：
- 强调需求、设计的作用
- 前一阶段完成后，只需关注后续阶段
- 为项目提供了按阶段划分的检查点，里程碑清晰
- 文档规范

缺点：
- 难以适应需求的频繁变化
- 项目周期后段才能看到成果
- 强制的里程碑、完成时间点
- 文档工作量大

#### 2. V模型——目前使用最广泛的模型（瀑布模型的变种）
![V模型](/images/02-V模型.jpg)

优点：
- 非常明确地标明了测试过程中存在的不同级别
- 清楚地描述了这些测试阶段和开发过程期间各阶段的对应关系

缺点：
- 把测试作为编码之后的最后一个活动，需求分析等前期产生的错误直到后期的验收测试才能发现
- 忽略了测试的对象不应该仅仅包括程序，没有明确指出对需求、设计的测试

#### 3. W模型（双V模型）——测试伴随着开发周期进行
![W模型](/images/03-W模型.jpg)

优点：
- 测试的活动与软件开发同步进行
- 测试的对象不仅仅是程序，还包括需求和设计
- 尽早发现软件缺陷可降低软件开发的成本

缺点：
- 需求、设计、编码等活动被视为串行的，测试和开发活动也保持着一种线性的前后关系，上一阶段完全结束，才可正式开始下一个阶段工作
- 不能支持迭代、自发性以及变更调整

#### 4. X模型——针对V模型的改进
![X模型](/images/04-X模型.jpg)

&emsp;&emsp;X模型的左边描述的是针对单独程序片段所进行的相互分离的编码和测试，此后将进行频繁的交接，通过集成最终成为可执行的程序，然后再对这些可执行程序进行测试。

&emsp;&emsp;己通过集成测试的成品可以进行封装并提交给用户，也可以作为更大规模和范围内集成的一部分。多根并行的曲线表示变更可以在各个部分发生。

&emsp;&emsp;由图中可见，X模型还定位了探索性测试，这是不进行事先计划的特殊类型的测试，这一方式往往能帮助有经验的测试人员在测试计划之外发现更多的软件错误。但这样可能对测试造成人力、物力和财力的浪费，对测试员的熟练程度要求比较高。

#### 5. H模型——贯穿在整个软件生命周期
![H模型](/images/05-H模型.jpg)

相对于V模型和W模型，H模型将测试活动完全独立出来，形成了一个完全独立的流程，将测试准备活动和测试执行活动清晰地体现出来。

优点：
- 强调测试是独立的，只要测试准备完成，就可以执行测试

缺点：
- 太过于模型化，重点在于理解其中的意义指导实际工作，而模型本身并无太多的可执行的指导意义

#### 总结

 &emsp;&emsp;在这些模型中，传统的瀑布模型由于缺点过于明显基本已被淘汰，V模型强调了在整个软件项目开发中需要经历的若干个测试级别，但是它没有明确指出应该对软件的需求、设计进行测试，在这一点上，W模型得到了补充。但是W模型和V模型一样没有专门针对测试的流程说明。随着软件测试的不断发展，第三方测试已经独立出来这个时候，H模型就得到了相应的体现，表现为测试独立。X模型又在此基础上增加了许多不确定的因素处理情况，这就对应了实际情况中，项目经常变更的情况发生。

&emsp;&emsp;**软件测试模型对指导测试工作的进行具有重要的意义，但任何模型都不是完美的，**
在实际的工作中，我们要灵活地运用各种模型的优点，寻找恰当的就绪点开始测试并反复迭代测试，最终保证按期完成预定目标。
