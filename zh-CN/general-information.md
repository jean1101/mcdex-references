# 概览

## 简介
蒙特卡洛去中心化交易所（MCDEX）是一个去中心化衍生品交易平台，提供高效透明的杠杆交易。

MCDEX目前支持以下两种合约：

**MP到期合约**
- MP到期合约是一种具有到期日期的创新金融工具。杠杆率由上限价格和下限价格决定。
- MP到期合约完全抵押，无需追加保证金。同时，它意味着合约的价格无法高于上限价格或低于下限价格，高于上限价格的价格依旧被视为上限价格，低于下限价格的价格依旧被视为下限价格。

**永续合约**
- 永续合约是一种没有到期日的期货合约。
- 其市场价格通过资金费用机制将市场价格与基础资产的现货价格锚定。

## 订单类型
**市价单**

此类型的订单会立即与当时订单蒲上的最好价格（市场价格）匹配。市场单会被立即执行。

**限价单**

当市场价格达到用户设置的价格时，此类型的订单才会被匹配。买入限价单不会以高于限价的价格进行匹配。卖出限价单不会以低于限价的价格进行匹配。

## 费用
**MP到期合约**

- 挂单方：0.02%
- 吃单方：0.07%

**永续合约**

与订单簿交易：
- 交易手续费：对于挂单方为-0.025％，对于吃单方为0.075％。      
- Gas费：无（所有交易的Gas费完全由MCDEX承担）

与自动做市商交易：
- 交易手续费：0.3％，归属于流动性提供方。
- Gas 费：用户自行支付Gas费。

对于订单簿和自动做市商：
- 存款和取款：在MCDEX上存/取款均无需支付费用。但是，用户需自行支付存/取款链上事务的Gas费。
- 清算：清算将收取比平常交易更高的费用。罚金2.5％，1.5％用于奖励清算者，1％自动注入保险基金。