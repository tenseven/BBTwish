typora-copy-images-to: BBTwish

# 设置6张表

### 第1张 pre_wish

* 用来储存我们预先设定好的wishes,给用户参考

* ![data1](https://github.com/tenseven/BBTwish/blob/master/BBTwish/data1.png)

  

### 第2张 custom_wish (用户自定义)

- 用来储存所有用户的许愿信息

- ![data6](https://github.com/tenseven/BBTwish/blob/master/BBTwish/data6.png)

  

- 包括了

  * wish_content ：文本内容
  * wisher_id ：许愿者的open_id
  * helper_id ：祝愿者的open_id
  * situation ：愿望是否被领取的状态，两个值（已领取，未领取）
  * cometure: 这是给许愿者用来确认愿望是否实现，两个值，0和1，只有当situation为已领取时，许愿者才有权限改变cometure的值，根据cometure为1的个数来累计小精灵的个数
  * ball_path:每个愿望相对应的精灵球的图片路径（我猜可能需要）
  * fairy_path:每个精灵球相对应的精灵的图片路径
  * weixin、name、telephone：这三个数据如果是按设计的第一次想法，每次许愿后都填写信息，可根据最后方案来决定要不要在这里删掉
  * time :时间这个我在想可不可以~~去掉~~，因为有点鸡肋

 ### 第3张 accumulate_help_times

* 用来累计每天祝愿的次数
* ![data3](https://github.com/tenseven/BBTwish/blob/master/BBTwish/data3.png)
* 其中

  * day: 精确到天，根据日数来累计

  * times:次数
* 这个方法好像不是很好，但是我目前想到的就是这个

### 第4张 accumulate_wish_times

* 许愿次数限制，与第3张类似

* ![data7](https://github.com/tenseven/BBTwish/blob/master/BBTwish/data7.png)

  

### 第5张 user

* 统计精灵球个数，和精灵个数，以及基本信息（这个根据设计的方案来最终决定要不要）

* ![data4](https://github.com/tenseven/BBTwish/blob/master/BBTwish/data4.png)

  

### 第6张 game_rule

* 储存游戏规则

  


