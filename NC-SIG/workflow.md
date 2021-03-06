# NC-SIG工作流
## 任务领取

NC-SIG 任务以 issue 的形式组织，每个任务都会被打上标签，社区开发者和小组成员可结合自己的兴趣和对源码的理解程度在github projects的任务列表中选择适合自己难度的issue，难度划分如下：

- **low**: 低难度，只需要了解FISCO BCOS一小部分知识并使用较少代码量完成
- **medium**: 中难度，需要了解FISCO BCOS多种知识或需要显著代码量完成
- **high**: 高难度，需要完全了解FISCO BCOS或需要非常多代码量完成
- **super high**: 超高难度，需要结合系统编程等综合性知识完成

## 编码

当选定 issue 之后需要根据 issue 的类型以及难度进行后续的工作，**对于简单的任务可以直接进行编码**；对于复杂或者大量重构的 issue 需要先写提案文档，文档需要覆盖一下内容：

- **方案概述**：对于这个方案的概括性介绍
- **可行性分析**：在目前的架构下当前方案是否可行
- **兼容性分析**：本次改动是否会打破向后兼容性
- **性能分析**：本次改动是否存在性能提升或性能回退

提案通过后，开发负责人需要通过 issue 或者PR的形式与组员进行讨论，最终达成一致后，形成完整的设计文档，设计文档讨论通过后，可着手编码，设计文档主要包含如下内容：

- **背景**：方案提出的背景
- **竞品调研**：对竞品的调研情况
- **方案概述**：对方案进行概括性的介绍
- **功能列表**： 概括性介绍方案的功能列表
- **系统/模块架构**：给出模块图
- **接口与数据结构设计**: 设计相关接口与数据结构
- **时序图**：可选，若涉及到复杂的流程，需要给出流程的时序图
- **兼容性说明**：说明设计方案的兼容性
- **开发计划**：给出开发和提测规划
## 测试

为了保证代码的执行和代码的维护性，以及约束后续 PR 不破坏当前定义的行为（如果是有意识的修改当前行为，需要有测试能反馈出行为的修改），对于任何有逻辑改动的 PR，都需要添加对应的**单元测试**和**集成测试**。

大特性的提测，需要先给出提测文档，提测方案讨论通过后，测试同学开始介入测试，提测文档主要包括如下内容：
- **背景**
- **使用方法**
- **功能测试方法**
- **稳定性测试方法**
- **性能测试方法**
- **兼容性测试方法**
- **迁移方案测试方法**
