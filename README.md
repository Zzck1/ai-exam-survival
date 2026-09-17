# AI期末保命速学 Skill

一个面向考前时间有限、基础薄弱学生的可迁移 Skill。它在一次简短问诊后，先检查课程资料是否足以可靠生成，再基于学生提供的资料制作模块化 Markdown 学习包。

它的目标是让学生优先复习最有依据、最值得投入时间的内容；默认以“及格线加约 10 分”的**备考覆盖目标**安排学习，不预测成绩，也不承诺及格。

## 功能

- 资料清点、可读性检查与最低启动标准
- 缺少核心范围或可靠答案时，只输出资料缺失报告
- 基于固定证据层级与 40 / 25 / 20 / 15 权重的考点取舍
- 背诵型、计算型和混合型课程的不同复习工具
- 按剩余时间生成每日任务；时间不足时切换到极限保命模式
- 原题精选、资料内改编题、资料闭环的 AI 仿题和模拟卷
- 题目、答案、风险、冲突、导航及模块化输出的交叉检查

## 资料边界

课程知识、公式、题目和答案依据只能来自学生当次上传的资料。Skill 不使用网络、模型记忆或其他课程资料补全内容。资料无法完整读取、课程范围不足或核心题目没有可靠答案时，必须阻断完整学习包生成。

## 文件结构

```text
ai-exam-survival/
├── SKILL.md
├── 安装与使用.md
├── references/
│   ├── intake-questionnaire.md
│   ├── material-audit-rules.md
│   ├── exam-point-ranking.md
│   ├── course-type-strategies.md
│   ├── time-compression-rules.md
│   └── quality-checklist.md
└── templates/
    ├── missing-material-report.md
    ├── output-folder-structure.md
    ├── study-package.md
    ├── memorization-course.md
    ├── calculation-course.md
    └── mixed-course.md
```

完整安装和调用示例见 [安装与使用.md](安装与使用.md)。

## 快速调用

```text
$ai-exam-survival
请用我提供的课程资料文件夹生成期末保命学习包。
课程：管理学
考试：2026-09-24 09:00，Asia/Shanghai
每天可学习：3小时
考试方式：闭卷
题型及分值：不清楚
满分及及格线：100分，60分
当前基础：零基础
请开始；仅使用上传资料。
```

## 许可证

本项目采用 [MIT License](LICENSE)。

