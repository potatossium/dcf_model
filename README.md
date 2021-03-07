# dcf_model
1. 通过JoinQuant提供的API读取财务报表相关项目的数值
2. 选取合适的收入增长率，贴现率，永续增长率等输入参数
3. 建立DCF模型估计公司价值，并输出估计股价

聚宽网在线研究网址：https://www.joinquant.com/  
API文档：https://www.joinquant.com/help/api/help?name=api

一些需要的参数：
  Argument              | Meaning          
----------------------- | ------------------
date                    | 查表日期（年报）
period                  | (date, date+period)使用近期收入增长率，(date+period, +∞)使用永续增长率估计现金流
code                    | 股票代码
cap_ex_growth_rate      | 资本支出增长率
perpetual_growth_rate   | 永续增长率
discount_rate           | 贴现率
earnings_growth_rate    | 利润增长率

-----------------

2021.03.07 README更新

贵州茅台2021年股价峰值2601元，与2020年年初的估值相比，上涨了100%还要多；现在回过去看，当时参考的研报估值表格最乐观的情况（永续增长率=4%，WACC=8.75%）对应的股价是1724，还是保守了，故此非常佩服张坤张经理的投资眼光，增加一个张经理的访谈链接：
https://zhuanlan.zhihu.com/p/147804213

-------------------

### 参考：
[1] https://github.com/halessi/DCF  
[2] https://pyfinmod.readthedocs.io/en/latest/dcf.html  
[3] https://medium.com/swlh/intrinsic-valuation-of-stocks-using-python-5d902a34b1a0





