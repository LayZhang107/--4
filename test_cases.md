# 测试样例

1. 输入完整评论且评分 5：应保留，情绪编码为好评。
2. 输入含“破损”且评分 1：应编码为差评，并命中包装与配送。
3. 输入评分超出 1-5 或日期格式错误：应被过滤，不进入 sample_size。

运行方式：`python src/consumer_insight_engine.py`；检查 `outputs/statistics.json` 的 sample_size、topics_ranked 和 `outputs/audit_10.csv`。
