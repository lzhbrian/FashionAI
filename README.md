# FashionAI
按照此代码训练效果不好。
目前有两个问题尚未解决：
* 一个是此代码是做语意分割、box回归、和分类的代码，目前我只改了数据接口，还未按照maskrcnn论文中的方式修改成关键点检测。
* 二是图片标注问题，数据集中假如含有裤子和上衣，标注数据时只标注了上衣，但是网络输入同时会输出裤子关键点，在构建损失函数时应该把裤子的输出信息屏蔽掉。
有木有一起搞的额
