# ai-learning

AI 学习环境（任务一）。环境由 conda 创建，包用 pip 安装。

## 环境信息

| 项目 | 值 |
| --- | --- |
| 环境名 | `ai-learning` |
| 环境路径 | `D:\python\envs\ai-learning` |
| Python | 3.12.14 |
| numpy | 2.5.3 |
| pandas | 3.0.6 |
| matplotlib | 3.11.2 |
| scikit-learn | 1.9.1 |

## 在 PyCharm 里使用

1. 打开 `D:\pythonProject\ai-learning` 作为项目。
2. `File -> Settings -> Project: ai-learning -> Python Interpreter`。
3. `Add Interpreter -> Add Local Interpreter`。
4. 左侧选 `Conda Environment`（或 `System Interpreter`），解释器路径填：
   `D:\python\envs\ai-learning\python.exe`
5. 确定后等待索引完成，右下角应显示 Python 3.12 (ai-learning)。
6. 打开 `01_hello_sklearn.py`，右键 `Run`，控制台输出 `test accuracy = 1.0000`。

> 如果选 Conda Environment：Base conda 填 `D:\python`，Environment 选 `ai-learning`。

## 在终端里使用

```powershell
D:\python\Scripts\activate.bat ai-learning
python 01_hello_sklearn.py
```

或者不激活、直接用绝对路径：

```powershell
D:\python\envs\ai-learning\python.exe 01_hello_sklearn.py
```

## 安装依赖

```powershell
D:\python\envs\ai-learning\python.exe -m pip install -i https://pypi.tuna.tsinghua.edu.cn/simple -r requirements.txt
```

国内直连 pypi.org 经常超时，建议固定用清华镜像。永久配置：

```powershell
D:\python\envs\ai-learning\python.exe -m pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```

## 说明

- 该环境由 `ms312` 克隆而来，因此自带 scipy、pillow 等依赖，属于正常现象。
- 示例 `01_hello_sklearn.py` 是 10 行的随机森林分类，跑通即代表环境可用。
