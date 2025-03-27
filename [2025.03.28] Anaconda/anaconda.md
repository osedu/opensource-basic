![logo](./assets/logo.png)

### Anaconda简介

Anaconda 是由 Anaconda, Inc. 公司开发一种流行的Python语言发行版，专注于**数据科学**、**机器学习**和**科学计算**。旨在**简化包管理和部署**，提供一个强大的生态系统，方便用户处理复杂的数据分析任务。**尤其适合处理复杂的依赖关系和多项目开发**。

==Anaconda 通过简化工具链，让用户更专注于数据科学本身，而非环境配置问题。==

![img](./assets/nav-tabs.png)

### 核心功能

1. **包管理**
   - 集成了 **conda**（跨平台包管理器），可安装、更新、删除 Python包（包括非Python依赖，如CUDA、TensorFlow、Pytorch等）。
   - 提供超过 **7,500+ 预编译的科学计算包**（如 NumPy、Pandas、SciPy、Matplotlib、Scikit-learn 等），避免手动编译的麻烦。
2. **环境管理** 
   - 支持创建**独立虚拟环境**，隔离不同项目所需的依赖（例如：Python 2.7 和 Python 3.11 共存）。
   - 解决“依赖冲突”问题（如项目A需要 TensorFlow 1.x，项目B需要 TensorFlow 2.x）。
3. **集成工具** 
   - 包含 **Anaconda Navigator**（图形化界面），以及 **Jupyter Notebook、Spyder、VS Code** 等开发工具。
   - 提供 **Dask、Numba** 等高性能计算工具。
4. **跨平台支持** 
   它支持 Windows、macOS 和 Linux，适合不同操作系统的开发者使用。

### **适用场景**

- **数据分析**：通过 Pandas 和 Jupyter Notebook 进行数据处理和可视化。
- **机器学习**：结合 Scikit-learn、TensorFlow 或 PyTorch 构建模型。
- **科学计算**：利用 NumPy 和 SciPy 进行数学建模。

### 版本与组件

- **Anaconda Distribution** = **全家桶套餐**（省心但臃肿）
  完整版，包含所有预装包（约 3GB），适合初学者或需要全套工具的用户。

- **Miniconda** = **基础框架 + 自选配件**（灵活但需手动配置）
  轻量版（仅含 Conda 和 Python），用户可按需安装包，节省空间。

### 安装与基础命令
1. **安装** 
   官网下载安装包：[https://www.anaconda.com/download](https://www.anaconda.com/download)

2. **常用命令**  
   
   ```bash
   # 创建环境（指定Python版本）
   conda create -n myenv python=3.9
   
   # 激活环境
   conda activate myenv
   
   # 安装包
   conda install numpy pandas jupyter
   
   # 启动jupyter notebook
   jupyter notebook
   
   # 退出当前激活环境 
   conda deactivate myenv
   
   # 显示有哪些虚拟环境
   conda list
   
   # 删除指定的虚拟环境
   conda env remove -n myenv
   
   # 设置镜像 
   conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
   ```
