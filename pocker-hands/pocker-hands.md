# 游戏：德州扑克

德州扑克共有52张牌（没有王牌），分为4种花色：红桃，黑桃，梅花，方块，包括13种面值：2、3、4、5、6、7、8、9、T、J、Q、K、A。其中，2最小，A最大；相同面值，花色不同，但具有相同等级。

存在两个玩家，各持5张牌，请实现一个比较算法，决定哪一方胜出。其中，比较规则按照如下升序排列：

1. 高牌：5张散牌，由最高值的牌决定等级；如果最高牌相同，则比较次高的牌，依次类推。
2. 对子：存在1对，3张散牌，优先使用对子的面值决定等级；如果对子面值相同，剩余三张散牌的高牌决定等级。
3. 两对：2对，1张散牌，按照对子的面值的降序依次决定等级。如果两个对子面值都相同，则比较剩余的1张散牌。
4. 三条：3张相同的面值，2张散牌。如果两个都是三条，由三条的面值决定等级。
5. 顺子：5张面值连续的牌，花色不一样。如果两个都是顺子，由高牌决定等级。
6. 同花：5张花色相同的牌。如果两个都是同花，由高牌决定等级。
7. 葫芦：3张相同的面值，1个对子。如果两个都是葫芦，由3条的面值决定等级。
8. 四条：4张面值相同的牌，1张散牌。如果两个都是四条，由四条的面值决定等级。
9. 同花顺：5张面值连续，并具有相同花色的牌。如果两个都是同花顺，由高牌决定等级。

