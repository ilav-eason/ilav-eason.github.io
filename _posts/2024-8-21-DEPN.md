---
title: DEPN复现过程
author: ilav
date: 2024-8-21
category: Jekyll
layout: post
---
# DEPN复现过程

### 环境依赖：

1. ls指令查看服务器中的所有已经存在的应用，发现CUDA的程序，推测CUDA已经安装完成，使用nvidia -smi查看具体安装情况

2. 根据requirements.txt中的内容，判断使用的python版本为3.9，因此使用miniconda创建一个python3.9的虚拟环境女尺寸-

3. 使用的命令：
   ```bash
   conda create --name DEPN python=3.9
   conda activate DEPN
   ```

4. 为了便于下载依赖包，下载pip，观察到requirements.txt的pip版本为22.2.2

   ```bash
   conda install pip==22.2.2
   ```

5. 然后使用pip批量下载依赖（github库中所给的requirements.txt文件无法直接使用，需添加“==”）：

   ```bash
   pip install -r requirements.txt
   ```

6. 下载到sklearn==0.0.post1这一行报错，发现这句没有确切指出sklearn的版本，使用发行版即可，因此修改为

   ```bash
   scikit-learn
   ```

   下载后查包发现是1.1.3版本

7. 下载到pytorch报错，根据报错原因是说官方库中没有2.1.1+cu118版本，手动下载
   报错内容如下：

   ```txt
   Solving environment: failed
   
   PackagesNotFoundError: The following packages are not available from current cha
   nnels:
   
   pytorch-cuda-12.1
   
   Current channels:
   
   - https://conda.anaconda.org/pytorch
   - https://conda.anaconda.org/nvidia
   - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
   - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free
   - defaults
   
   To search for alternate channels that may provide the conda package you're
   looking for, navigate to
   
   https://anaconda.org
   
   and use the search bar at the top of the page.
   ```

   解决方案为手动安装：
   ```bash
   # 安装 CUDA 工具包
   conda install cudatoolkit=11.8 -c nvidia
   
   # 安装 PyTorch
   conda install pytorch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 -c pytorch
   ```

   安装成功后将txt文件中的这三行删除，重新安装

   发现顺利安装完所有的依赖

8. 查看依赖包安装情况：
   ```bash
   pip freeze
   ```

   > pip list 无法查看安装的所有依赖包，因此使用pip freeze进行完整查看。

### 数据处理：

1. 下载安然数据集到目录位置：~/DEPN/DEPN/
   ```bash
   wget https://www.cs.cmu.edu/~enron/enron_mail_20150507.tar.gz
   ```

2. 下载后将数据（maildir）解压到~/DEPN/DEPN/data

3. 修改preprocess_enron.py文件中数据的路径，并运行。
   ```bash
   python preprocess_enron.py
   ```

4. copy BERT模型：

   ```bash
   wget https://raw.githubusercontent.com/huggingface/transformers/main/examples/pytorch/language-modeling/run_mlm_no_trainer.py
   ```

5. 