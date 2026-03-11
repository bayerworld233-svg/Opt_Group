# Optimization Models and Methods - Group Project

## 项目简介 / Project Overview

本项目是优化模型与方法（Optimization Models and Methods）课程的小组作业，主要研究和实现线性规划/整数规划相关的优化问题。

This is a group project for the Optimization Models and Methods course, focusing on linear programming and integer programming optimization problems.

## 团队成员 / Team Members

- Member 1: [姓名]
- Member 2: [姓名]
- Member 3: [姓名]
- Member 4: [姓名]

## 项目结构 / Project Structure

```
Opt_Group/
├── README.md                    # 项目说明
├── requirements.txt             # Python依赖包
├── .gitignore                   # Git忽略文件配置
├── data/                        # 数据文件夹
│   ├── raw/                     # 原始数据
│   └── processed/               # 处理后的数据
├── src/                         # 源代码
│   ├── models/                  # 优化模型定义
│   ├── solvers/                 # 求解器实现
│   └── utils/                   # 工具函数
├── notebooks/                   # Jupyter notebooks（数据探索、结果分析）
├── results/                     # 实验结果
│   ├── figures/                 # 图表
│   └── tables/                  # 数据表格
├── report/                      # LaTeX项目报告
│   ├── main.tex                 # 主文档
│   ├── sections/                # 各章节
│   ├── figures/                 # 报告中的图片
│   └── references.bib           # 参考文献
└── tests/                       # 单元测试
```

## 环境配置 / Environment Setup

### 1. 克隆仓库 / Clone Repository

```bash
git clone https://github.com/[your-username]/Opt_Group.git
cd Opt_Group
```

### 2. 创建虚拟环境 / Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. 安装依赖 / Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. （可选）安装商业求解器 / Optional: Install Commercial Solvers

如果需要使用 Gurobi 或 CPLEX，请：
- 获取学术许可证
- 安装对应的 Python 包
- 配置许可证文件

## 使用方法 / Usage

### 运行优化模型 / Run Optimization Model

```bash
python src/models/your_model.py
```

### 运行 Jupyter Notebook

```bash
jupyter notebook notebooks/
```

### 编译 LaTeX 报告 / Compile LaTeX Report

```bash
cd report
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## 项目进度 / Project Timeline

- [ ] 问题定义与文献调研
- [ ] 数据收集与预处理
- [ ] 模型设计与实现
- [ ] 算法求解与结果分析
- [ ] 报告撰写
- [ ] 最终展示准备

## 贡献指南 / Contributing

1. 从 `main` 分支创建新的功能分支
2. 在新分支上进行开发
3. 提交前确保代码可以正常运行
4. 创建 Pull Request 并请求审查

## 许可证 / License

本项目仅用于学术目的。

This project is for academic purposes only.

## 联系方式 / Contact

如有问题，请联系：[your-email@example.com]
