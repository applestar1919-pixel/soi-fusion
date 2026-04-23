# AI赋能融合教育感官支持系统

基于神经多样性的课堂动态评价实践

鞍山市立山区教师进修学校

---

## 项目简介

本系统面向普教融合班级ASD学生支持需求，帮助普通教师在3秒内完成感官状态评估并获取干预建议。核心为SOI感官过载指数评估引擎，输出0—1.0五级评分，匹配分级干预策略。

提供三种使用入口：
- 网页端：https://yf3rsrikalnq2.ok.kimi.link
- 豆包智能体（扫码使用）
- 微信小程序（扫码使用）

---

## 文件说明

| 文件/文件夹 | 说明 |
|---|---|
| soi_assessor.py | SOI感官过载指数评估引擎（核心） |
| app/ | 网页前端源码 |

---

## 运行评估引擎

**环境要求：** Python 3.8 及以上

**安装依赖：**
```bash
pip install -r requirements.txt
```

**运行示例：**
```bash
python soi_assessor.py
```

**调用示例：**
```python
from soi_assessor import SOIAssessor

assessor = SOIAssessor()
result = assessor.assess("学生突然捂住耳朵，教室内多名同学大声朗读")
print(assessor.format_result(result))
```

---

## 配套文档

- SOI教师操作手册（含典型案例、应急流程、家校沟通模板）
- 开发与应用报告

---

## 开源协议

MIT License — 欢迎其他学校自由使用和改造
