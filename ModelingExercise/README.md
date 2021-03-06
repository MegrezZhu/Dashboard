## 建模要求
1.建模答案需包括：
  - 用例图
  - 新建清单及任务的活动图
  - 清单/任务管理领域模型
  - 清单/任务的状态图
  - 任意一个场景的系统顺序图
  - 操作协议

2.具体的制图要求同课程规范

## 建模者答案与评价
1.https://blog.csdn.net/Alice_am/article/details/80294682
  - 【用例图】这个应用中涉及的操作有很多，对象之间也有嵌套关系，所以用例图是比较难画的。这份答案的用例图逻辑很清晰，没有遗漏操作——搜索和云同步功能可以暂时不考虑进系统。只不过添加任务的用例因为它有不同层级的两个入口，所以既可以认为是管理清单内容的子用例，也可以认为是一个单独的用例，这时候“选择清单”这个动作会有差别，很难同时把两种意思表达出来。
  - 【活动图】其实我感觉，站在用户的角度，这个应用的业务里面随便一个动作都可以单拎出来做一个活动：开始->修改XXX->结束。就比方说，复制清单跟管理任务没有绝对的先后关系。不过既然如此这里的活动图也没啥好画的，答案中的图或许进一步理清了系统的功能架构吧。
  - 【领域模型】没毛病，很好。
  - 【状态模型】理由和活动图那里一样，我觉得如果不考虑云同步的功能，没啥好画的。答案里面有点bug就是：框里面应该都是些像“被删除”、“被创建”这样的表状态的词，而编辑、添加、删除这样的动词应该放在直线旁边。
  - 【系统顺序图】也没什么大问题。如果要更好的话，或许可以再仔细考虑参数，以及系统分本地和云端去考虑。

2.https://yinghongzhang.github.io/2018/05/13/Lesson9-%E5%A5%87%E5%A6%99%E6%B8%85%E5%8D%95/

- 【用例图】：搜索清单那里可以支持对所有任务的名称和描述进行搜索，用例图没表现出来
- 【活动图】：没好好利用符号
- 【领域模型】：没毛病，很好
- 【状态模型】：整体挺不错的，但是缺少了终止状态
- 【系统顺序图】：没有考虑到传参

3.https://mikexuq.github.io/2018/05/11/Lesson9/

- 【用例图】：用例图名称需要以动词开头，且“清单管理”仅是其中某一子用例；建议增加“管理任务”子用例，且将各个子用例细化，如“创建清单”创建清单子用例可拓展出“填写名称”、“邀请成员”和“选择清单夹”。
- 【活动图】：比较难画，可选择将业务中“创建清单”、“管理清单”、“创建任务”、“管理任务”等用例拆分成单个的活动图，这些用例之间没有绝对的先后关系。
- 【领域模型】：缺少“清单夹”，还有部分实体的属性有缺漏，如“文件”缺少“文件内容”。
- 【状态模型】：笔误将某些“清单”打成“订单”。
- 【系统顺序图】：考虑“创建任务”，以及细化参数。
