# sketch2code be moved and comprehend #

sketch2code 带给了大家对网页的开发的一种人工智能化的美好期望，当我听到这消息的时候，心情是这样的---我的天呢。还有这种操作!后来开始研究它的基本原理和工作流程。其实我想大家和我一样同样都是比较的震惊的，虽然正式的产品还没有面世，不过一众Twitter网友都惊呆了，他们看到这个话题的反应是这样：

   ![](https://img.huxiucdn.com/article/content/201810/15/150554487286.gif?imageView2/2/w/1000/format/gif/interlace/1/q/85)

![](https://img.huxiucdn.com/article/content/201810/15/150554106186.gif?imageView2/2/w/1000/format/gif/interlace/1/q/85)

其实我和他们的反应效果差不多，一种吃惊状。
同样的就像刚刚了解到的一样，它包含了的基础组件是些什么呢？

Sketch2Code 使用了以下组件：
 

微软自定义视觉模型（Custom Vision）：这个模型是基于不同的手绘稿的图象训练得出的，并标记了与常见 HTML 元素（如文本框、按钮、图像等）相关的信息。

微软计算机视觉服务：用于识别设计元素中的文本。

Azure Blob Storage：保存与 HTML 生成过程的每个步骤相关的信息，包括原始图像、预测结果、布局和分组信息等。

Azure Function：它作为后端入口点，通过与其他服务发生交互来协调生成过程。

Azure Website：用户界面前端，用户可以在这里上载设计图，并查看生成的 HTML。

