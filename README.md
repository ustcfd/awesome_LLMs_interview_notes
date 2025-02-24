# awesome_LLMs_interview_notes
LLMs interview notes and answers

## **内容说明**

问题来自 [LLMs 千面郎君： km1994 - LLMs_interview_notes ](https://github.com/km1994/LLMs_interview_notes)

**答案 为 自己编写，不保证正确，仅供参考。**

**有些问题，提供的答案更多是一种线索，如想深入了解，请自行参考更多资料**

## 更新记录

1. 2023.09 发布： 大模型（LLMs）基础面，大模型（LLMs）进阶面，大模型（LLMs）微调面，大模型（LLMs）langchain面，基于LLM+向量库的文档对话 经验面，大模型（LLMs）参数高效微调(PEFT) 面，大模型（LLMs）推理面，大模型（LLMs）评测面，大模型（LLMs）强化学习面， 大模型（LLMs）训练集面， 大模型（LLMs）agent 面
2. 2023.10 新增：Token及模型参数准备篇， LLMs 位置编码篇， LLMs Tokenizer 篇， Layer Normalization 篇， LLMs 激活函数篇
3. 2023.11 新增： LLM文档对话 —— pdf解析关键问题，怎么让英文大语言模型支持中文？（一） —— 构建中文tokenization，怎么让英文大语言模型支持中文？（二） —— 继续预训练篇，怎么让英文大语言模型支持中文？（三） —— 对预训练模型进行指令微调


## 目录

- [x] **[大模型（LLMs）基础面](./大模型（LLMs）基础面.md)**
  - [x] 1. 目前 主流的开源模型体系 有哪些？
  - [x] 2. prefix LM 和 causal LM 区别是什么？
  - [x] 3. 涌现能力是啥原因？
  - [x] 4. 大模型LLM的架构介绍？
- [x] **[大模型（LLMs）进阶面](./大模型（LLMs）进阶面.md)**
  - [x] 1. LLMs 复读机问题
    - [x] 1. 什么是 LLMs 复读机问题？
    - [x] 2. 为什么会出现 LLMs 复读机问题？
    - [x] 3. 如何缓解 LLMs 复读机问题？
  - [x] 2. llama 系列问题
    - [x] 1. llama 输入句子长度理论上可以无限长吗？
  - [x] 3. 什么情况用Bert模型，什么情况用LLaMA、ChatGLM类大模型，咋选？
  - [x] 4. 各个专业领域是否需要各自的大模型来服务？
  - [x] 5. 如何让大模型处理更长的文本？
- [x] **[大模型（LLMs）微调面](./大模型（LLMs）微调面.md)**
  - [x] 1. 如果想要在某个模型基础上做全参数微调，究竟需要多少显存？
  - [x] 2. 为什么SFT之后感觉LLM傻了?
  - [x] 3. SFT 指令微调数据 如何构建?
  - [x] 4. 领域模型Continue PreTrain 数据选取？
  - [x] 5. 领域数据训练后，通用能力往往会有所下降，如何缓解模型遗忘通用能力？
  - [x] 6. 领域模型Continue PreTrain ，如何 让模型在预训练过程中就学习到更多的知识？
  - [x] 7. 进行SFT操作的时候，基座模型选用Chat还是Base?
  - [x] 8. 领域模型微调 指令&数据输入格式 要求？
  - [x] 9. 领域模型微调 领域评测集 构建？
  - [x] 10. 领域模型词表扩增是不是有必要的？
  - [x] 11. 如何训练自己的大模型？
  - [x] 12. 训练中文大模型有啥经验？
  - [x] 13. 指令微调的好处？
  - [x] 14. 预训练和微调哪个阶段注入知识的？
  - [x] 15. 想让模型学习某个领域或行业的知识，是应该预训练还是应该微调？
  - [x] 16. 多轮对话任务如何微调模型？
  - [x] 17. 微调后的模型出现能力劣化，灾难性遗忘是怎么回事？
  - [x] 18. 微调模型需要多大显存？
  - [x] 19. 大模型LLM进行SFT操作的时候在学习什么？
  - [x] 20. 预训练和SFT操作有什么不同
  - [x] 21. 样本量规模增大，训练出现OOM错
  - [x] 22. 大模型LLM进行SFT 如何对样本进行优化？
  - [x] 23. 模型参数迭代实验
- [x] **[大模型（LLMs）langchain面]()**
  - [x] **[大模型（LLMs）langchain 面](./大模型（LLMs）langchain面/大模型（LLMs）langchain面.md)**
    - [x] 1. 什么是 LangChain?
    - [x] 2. LangChain 包含哪些 核心概念？
      - [x] 1. LangChain 中 Components and Chains 是什么？
      - [x] 2. LangChain 中 Prompt Templates and Values 是什么？
      - [x] 3. LangChain 中 Example Selectors 是什么？
      - [x] 4. LangChain 中 Output Parsers 是什么？
      - [x] 5. LangChain 中 Indexes and Retrievers 是什么？
      - [x] 6. LangChain 中 Chat Message History 是什么？
      - [x] 7. LangChain 中 Agents and Toolkits 是什么？
    - [x] 3. 什么是 LangChain Agent?
    - [x] 4. 如何使用 LangChain ?
    - [x] 5. LangChain 支持哪些功能?
    - [x] 6. 什么是 LangChain model?
    - [x] 7. LangChain 包含哪些特点?
    - [x] 8. LangChain 如何使用?
      - [x] 1. LangChain 如何调用 LLMs 生成回复？
      - [x] 2. LangChain 如何修改 提示模板？
      - [x] 3. LangChain 如何链接多个组件处理一个特定的下游任务？
      - [x] 4. LangChain 如何Embedding & vector store？
    - [ ] 9. LangChain 存在哪些问题及方法方案？
      - [x] 1. LangChain 低效的令牌使用问题
      - [ ] 2. LangChain 文档的问题
      - [ ] 3. LangChain 太多概念容易混淆，过多的“辅助”函数问题
      - [ ] 4. LangChain 行为不一致并且隐藏细节问题
      - [x] 5. LangChain 缺乏标准的可互操作数据类型问题
    - [x] 10. LangChain 替代方案？
  - [x] **[基于LLM+向量库的文档对话 经验面](./大模型（LLMs）langchain面/基于LLM+向量库的文档对话经验面.md)**
    - [x] 1. 基于LLM+向量库的文档对话 基础面
      - [x] 1. LLMs 存在模型幻觉问题，请问如何处理？
      - [x] 2. 基于LLM+向量库的文档对话 思路是怎么样？
      - [x] 3. 基于LLM+向量库的文档对话 核心技术是什么？
      - [x] 4. 基于LLM+向量库的文档对话 prompt 模板 如何构建？
    - [x] 2. 基于LLM+向量库的文档对话 优化面
      - [x] 1. 痛点1：文档切分粒度不好把控，既担心噪声太多又担心语义信息丢失
      - [x] 2. 痛点2：在基于垂直领域 表现不佳
      - [x] 3. 痛点3：langchain 内置 问答分句效果不佳问题
      - [x] 4. 痛点4：如何 尽可能召回与query相关的Document 问题
      - [x] 5. 痛点5：如何让LLM基于query和context得到高质量的response
    - [ ] 3. 基于LLM+向量库的文档对话 工程示例面
      - [ ] 1. 避坑记录
      - [ ] 2. 本地知识库问答系统（Langchain-chatGLM）
  - [x] **[LLM文档对话 —— pdf解析关键问题](./大模型（LLMs）langchain面/LLM文档对话%20——%20pdf解析关键问题.md)**
    - [x] 一、为什么需要进行pdf解析？
    - [x] 二、为什么需要 对 pdf 进行解析？
    - [x] 三、pdf解析 有哪些方法，对应的区别是什么？
    - [x] 四、pdf解析 存在哪些问题？
    - [x] 五、如何提取长文档（书籍）中关键信息？
    - [x] 六、为什么要提取标题甚至是多级标题？
    - [x] 七、如何提取 文章标题？
    - [x] 八、如何区分单栏还是双栏pdf？如何重新排序？
      - [x]  区分单栏和双栏PDF：
      - [x]  重新排序页面：
    - [x] 九、如何提取表格和图片中的数据？
      - [x]  提取表格中的数据：
      - [x]  提取图片中的数据：
      - [x]  结合LLM进行数据提取：
    - [x] 十、基于AI的文档解析有什么优缺点？
      - [x]  优点：
      - [x]  缺点：
- [x] **[大模型（LLMs）参数高效微调(PEFT) 面]()**
  - [x] **[大模型（LLMs）参数高效微调(PEFT) 面](./大模型（LLMs）参数高效微调(PEFT)面/大模型（LLMs）参数高效微调(PEFT)面.md)**
    - [x] 微调方法是啥？如何微调？
    - [x] 为什么需要 PEFT？
    - [x] 介绍一下 PEFT？
    - [x] PEFT 有什么优点？
    - [x] 微调方法批处理大小模式GPU显存速度？
    - [x] Peft 和 全量微调区别？
    - [x] 多种不同的高效微调方法对比
    - [x] 当前高效微调技术存在的一些问题
    - [x] 高效微调技术最佳实践
    - [x] PEFT 存在问题？
    - [x] 能不能总结一下各种参数高效微调方法？
  - [x] **[适配器微调（Adapter-tuning）篇](./大模型（LLMs）参数高效微调(PEFT)面/适配器微调（Adapter-tuning）篇.md)**
    - [x] 一、为什么 需要 适配器微调（Adapter-tuning）？
    - [x] 二、适配器微调（Adapter-tuning）思路？
    - [x] 三、 适配器微调（Adapter-tuning）特点是什么？
    - [x] 四、AdapterFusion 思路 是什么？
    - [x] 五、AdapterDrop 思路 是什么？
    - [x] 六、AdapterDrop 特点 是什么？
    - [x] 七、MAM Adapter 思路 是什么？
    - [x] 八、MAM Adapter 特点 是什么？
  - [x] **[提示学习（Prompting）](./大模型（LLMs）参数高效微调(PEFT)面/提示学习（Prompting）.md)**
    - [x] 一、为什么需要 提示学习（Prompting）？
    - [x] 二、什么是 提示学习（Prompting）？
    - [x] 三、提示学习（Prompting） 有什么优点？
    - [x] 四、提示学习（Prompting）有哪些方法，能不能稍微介绍一下它们间？
      - [x] 4.1 前缀微调（Prefix-tuning）篇
        - [x] 4.1.1 为什么需要 前缀微调（Prefix-tuning）？
        - [x] 4.1.2 前缀微调（Prefix-tuning）思路是什么？
        - [x] 4.1.3 前缀微调（Prefix-tuning）的优点是什么？
        - [x] 4.1.4 前缀微调（Prefix-tuning）的缺点是什么？
      - [x] 4.2 指示微调（Prompt-tuning）篇
        - [x] 4.2.1 为什么需要 指示微调（Prompt-tuning）？
        - [x] 4.2.2 指示微调（Prompt-tuning）思路是什么？
        - [x] 4.2.3 指示微调（Prompt-tuning）优点是什么？
        - [x] 4.2.4 指示微调（Prompt-tuning）缺点是什么？
        - [x] 4.2.5 指示微调（Prompt-tuning）与 Prefix-tuning 区别 是什么？
        - [x] 4.2.6 指示微调（Prompt-tuning）与 fine-tuning 区别 是什么？
      - [x] 4.3 P-tuning 篇
        - [x] 4.3.1 为什么需要 P-tuning？
        - [x] 4.3.2 P-tuning 思路是什么？
        - [x] 4.3.3 P-tuning 优点是什么？
        - [x] 4.3.4 P-tuning 缺点是什么？
      - [x] 4.4 P-tuning v2 篇
        - [x] 4.4.1 为什么需要 P-tuning v2？
        - [x] 4.4.2 P-tuning v2 思路是什么？
        - [x] 4.4.3 P-tuning v2 优点是什么？
        - [x] 4.4.4 P-tuning v2 缺点是什么？
  - [x] **[LoRA 系列篇](./大模型（LLMs）参数高效微调(PEFT)面/LoRA系列篇.md)**
    - [x] 一、LoRA篇
      - [x] 1.1 什么是 LoRA？
      - [x] 1.2 LoRA 的思路是什么？
      - [x] 1.3 LoRA 的特点是什么？
    - [x] 二、QLoRA篇
      - [x] 2.1 QLoRA 的思路是怎么样的？
      - [x] 2.2 QLoRA 的特点是什么？
    - [x] 三、AdaLoRA篇
      - [x] 3.1 AdaLoRA 的思路是怎么样的？
    - [x] 四、LoRA权重是否可以合入原模型？
    - [ ] 五、ChatGLM-6B LoRA后的权重多大？
    - [x] 六、LoRA 微调优点是什么？
    - [x] 七、LoRA微调方法为啥能加速训练？
    - [x] 八、如何在已有LoRA模型上继续训练？
- [x] **[大模型（LLMs）推理面](./大模型（LLMs）推理面.md)**
  - [x] 1. 为什么大模型推理时显存涨的那么多还一直占着？
  - [x] 2. 大模型在gpu和cpu上推理速度如何？
  - [x] 3. 推理速度上，int8和fp16比起来怎么样？
  - [x] 4. 大模型有推理能力吗？
  - [x] 5. 大模型生成时的参数怎么设置？
  - [x] 6. 有哪些省内存的大语言模型训练/微调/推理方法？
  - [x] 7. 如何让大模型输出合规化
  - [x] 8. 应用模式变更
- [x] **[大模型（LLMs）评测面](./大模型（LLMs）评测面.md)**
  - [x] 大模型怎么评测？
  - [x] 大模型的honest原则是如何实现的？
  - [x] 模型如何判断回答的知识是训练过的已知的知识，怎么训练这种能力？
- [x] **[大模型（LLMs）强化学习面](./大模型（LLMs）强化学习面.md)**
  - [x] 奖励模型需要和基础模型一致吗？
  - [x] RLHF 在实践过程中存在哪些不足？
  - [x] 如何解决 人工产生的偏好数据集成本较高，很难量产问题？
  - [x] 如何解决三个阶段的训练（SFT->RM->PPO）过程较长，更新迭代较慢问题？
  - [x] 如何解决 PPO 的训练过程同时存在4个模型（2训练，2推理），对计算资源的要求较高 问题？
- [x] **[大模型（LLMs）软硬件配置面](./大模型（LLMs）软硬件配置面.md)**
- [x] **[大模型（LLMs）训练集面](./大模型（LLMs）训练集面.md)**
  - [x] SFT（有监督微调）的数据集格式？
  - [x] RM（奖励模型）的数据格式？
  - [x] PPO（强化学习）的数据格式？
  - [x] 找数据集哪里找？
  - [x] 微调需要多少条数据？
  - [x] 有哪些大模型的训练集？
  - [x] 进行领域大模型预训练应用哪些数据集比较好？
- [ ] **[大模型（LLMs）显存问题面](./大模型（LLMs）显存问题面.md)**
- [ ] **[大模型（LLMs）分布式训练面](./大模型（LLMs）分布式训练面.md)**
- [x] **[大模型（LLMs）agent 面](./大模型（LLMs）agent面.md)**
  - [x] 如何给LLM注入领域知识？
  - [x] 如果想要快速体验各种模型，该怎么办？
- [ ] **[Token及模型参数准备篇](./Token及模型参数准备篇.md)**
  - [x] 预训练数据 Token 重复 是否影响 模型性能？
  - [ ] SFT需要训练Token数？
- [ ] **[LLMs 位置编码篇](./LLMs位置编码篇.md)**
  - [x] 1 什么是位置编码？
  - [x] 2 什么是绝对位置编码？
  - [x] 3 什么是相对位置编码？
  - [ ] 4 旋转位置编码 RoPE篇
    - [x] 4.1 旋转位置编码 RoPE 思路是什么？
    - [ ] 4.2 推导一下 旋转位置编码 RoPE ？
    - [x] 4.3 旋转位置编码 RoPE 有什么优点？
    - [ ] 4.4 旋转位置编码 RoPE 被哪些 LLMs 应用？
  - [ ] 5 长度外推问题篇
    - [x] 5.1 什么是 长度外推问题？
    - [x] 5.2 长度外推问题 的 解决方法 有哪些？
  - [ ] 6 ALiBi (Attention with Linear Biases)篇
    - [x] 6.1 ALiBi (Attention with Linear Biases) 思路是什么？
    - [x] 6.2 ALiBi (Attention with Linear Biases) 的偏置矩阵是什么？有什么作用？
    - [x] 6.3 ALiBi (Attention with Linear Biases) 有什么优点？
    - [ ] 6.4 ALiBi (Attention with Linear Biases) 被哪些 LLMs 应用？
- [ ] **[LLMs Tokenizer 篇](./LLMs%20Tokenizer%20篇/)**
  - [x] **[LLMs Tokenizer 篇](./LLMs%20Tokenizer%20篇/LLMs%20Tokenizer篇.md)**
    - [x] Byte-Pair Encoding(BPE)篇
      - [x] 1 Byte-Pair Encoding(BPE) 如何构建词典？
    - [x] WordPiece 篇
      - [x] 1 WordPiece 与 BPE 异同点是什么？
    - [x] SentencePiece 篇
      - [x] 简单介绍一下 SentencePiece 思路？
    - [x] 对比篇
      - [x] 1 举例 介绍一下 不同 大模型LLMs 的分词方式？
      - [x] 2 介绍一下 不同 大模型LLMs 的分词方式 的区别？
  - [x] **[怎么让英文大语言模型支持中文？（二） —— 继续预训练篇](./LLMs%20Tokenizer%20篇/怎么让英文大语言模型支持中文？（二）%20——%20继续预训练篇.md)**
    - [x] 一、为什么需要进行继续预训练？
    - [x] 二、如何对 继续预训练 数据预处理？
    - [x] 三、如何 构建模型？
    - [x] 四、如何 使用模型？
  - [x] **[怎么让英文大语言模型支持中文？（三） —— 对预训练模型进行指令微调](./LLMs%20Tokenizer%20篇/怎么让英文大语言模型支持中文？（三）%20——%20对预训练模型进行指令微调.md)**
    - [x] 一、为什么需要对预训练模型进行指令微调？
    - [x] 二、对预训练模型进行指令微调 数据 如何处理？
    - [x] 三、对预训练模型进行指令微调 tokenization 如何构建？
    - [x] 四、对预训练模型进行指令微调 模型 如何构建？
    - [x] 五、是否可以结合 其他库 使用？
- [x] **[Layer Normalization 篇](./LayerNormalization篇.md)**
  - [x] Layer normalization-方法篇
    - [x] Layer Norm 篇
      - [x] Layer Norm 的计算公式写一下？
    - [x] RMS Norm 篇 （均方根 Norm）
      - [x] RMS Norm 的计算公式写一下？
      - [x] RMS Norm 相比于 Layer Norm 有什么特点？
    - [x] Deep Norm 篇
      - [x] Deep Norm 思路？
      - [x] 写一下 Deep Norm 代码实现？
    - [x] Deep Norm 有什么优点？
  - [x] Layer normalization-位置篇
    - [x] 1 LN 在 LLMs 中的不同位置 有什么区别么？如果有，能介绍一下区别么？
  - [x] Layer normalization 对比篇
    - [x] LLMs 各模型分别用了 哪种 Layer normalization？
- [ ] **[LLMs 激活函数篇](./LLMs激活函数篇.md)**
  - [x] 1 介绍一下 FFN 块 计算公式？
  - [x] 2 介绍一下 GeLU 计算公式？
  - [x] 3 介绍一下 Swish 计算公式？
  - [x] 4 介绍一下 使用 GLU 线性门控单元的 FFN 块 计算公式？
  - [x] 5 介绍一下 使用 GeLU 的 GLU 块 计算公式？
  - [x] 6 介绍一下 使用 Swish 的 GLU 块 计算公式？
  - [ ] 各LLMs 都使用哪种激活函数？

------
## **Star-History**

![star-history](https://api.star-history.com/svg?repos=jackaduma/awesome_LLMs_interview_notes&type=Date "star-history")

------

## Donation
If this project help you reduce time to develop, you can give me a cup of coffee :) 

AliPay(支付宝)
<div align="center">
	<img src="./misc/ali_pay.png" alt="ali_pay" width="400" />
</div>

WechatPay(微信)
<div align="center">
    <img src="./misc/wechat_pay.png" alt="wechat_pay" width="400" />
</div>

------

