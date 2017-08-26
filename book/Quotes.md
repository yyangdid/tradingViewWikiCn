# 报价

---

报价是一组简短说明交易的数据。Charting Library支持观察列表（在**交易终端**配置中），并使用报价来显示有关商品的相关信息。

Charting Library 中不管是[JS API](https://github.com/tradingview/charting_library/wiki/JS-Api)还是[UDF](https://github.com/tradingview/charting_library/wiki/UDF)都使用相同的数据结构来进行报价。

以下是响应对象的描述：

# 商品报价数据

* `s`: 商品的状态码。预期的值为:`ok`\|`error`
* `n`: 商品名称。 此值必须与请求中完全相同
* `v`: object, 商品报价对象
  * `ch`: 价格变动（通常从当天的开盘价计算）
  * `chp`: 价格变动百分比
  * `short_name`: 商品略称
  * `exchange`: 交易所名称
  * `description`: 商品的简短描述
  * `lp`: 最后的成交价格
  * `ask`: 买盘价
  * `bid`: 卖盘价
  * `spread`: 费率
  * `open_price`: 当天开盘价
  * `high_price`: 当天最高价
  * `low_price`: 当天最低价
  * `prev_close_price`: 昨天收盘价
  * `volume`: 当天成交量