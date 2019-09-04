
# 打地鼠效果预览

# https://newway7.github.io/poke-a-mole/index.html


# 打地鼠逻辑：



建立一个4*4的table；

每个table放置默认图片:img/00.jpg；

开始游戏：

     1：每秒调用一次修改剩余时间的函数；

     2：每秒随机设置一个图片为img/01.jpg；同一个函数中设置一秒后这个图片变回img/00.jpg；并修改得分

     3：每个图片绑定click函数play(this);打中img/01.jpg的变为img/02.jpg；打中后还原img/00.jpg；并修改得分

     4：开始游戏：调用修改剩余时间函数、随机设置地鼠出现函数和地鼠消失函数；设置设置地鼠出现的时间间隔等设置为不可修改；

     5：暂停游戏；将所有setTimeout停止；并记录剩余时间；

     6：继续游戏：调用另一个修改剩余时间函数；地鼠每秒出现和消失函数；

     7：结束游戏：将所有setTimeout停止；设置地鼠出现的时间间隔等设置为可修改；
