---
title: 开发记录 
tags: MarkDown,初探,小书匠
grammar_cjkRuby: true
---

---

* #### 顺镜流程图

```flow
st=>start: 顺镜开机
cond1=>condition: 第一次进入应用?
op1=>operation: 向导页面
op2=>operation: WIFI配置入网
op3=>operation: Index首页
op4=>operation: 扫描二维码/搜索局域网
op5=>operation: QQ IoT
op6=>operation: Insprid IoT
cond2=>condition: 绑定QQ?
cond3=>condition: QQ IoT/Insprid IoT

st->cond1
cond1(yes)->op1->op2
cond1(no)->op2->cond2
cond2(yes)->op3
cond2(no)->op4->op3->cond3
cond3(yes)->op5
cond3(no)->op6
```
