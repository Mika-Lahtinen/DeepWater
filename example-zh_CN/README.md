# 如何在本地使用本库

## 预先准备工作

1. 新建一个目录，这里我们假设您新建的文件夹名为 WaterDemo
2. 将本仓库的 deepwater 文件夹 及 requirements.txt 文件复制到 WaterDemo 文件夹下
3. 准备好您的数据文件，将它们集合到一个文件夹当中，并将此数据文件夹复制到 WaterDemo 文件夹下
4. 安装 Anaconda（Miniconda 也可以），详情可参考 [Anaconda Official Homepage](https://www.anaconda.com/)，中国大陆地区可参考 [清华大学镜像站 Anaconda](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/) 或 [上海交通大学 Anaconda](https://mirrors.sjtug.sjtu.edu.cn/docs/anaconda)

## 开始工作
1. 在 WaterDemo 目录下，通过命令行输入如下命令以建立、激活一个使用 Python 3.10 的虚拟环境：
```shell
conda create -n venv python=3.10
conda activate venv
```

2. 激活虚拟环境后，通过命令行输入如下命令安装 requirements.txt 下所记录的依赖项：
```shell
pip install -r requirements.txt
```
注意：中国大陆地区的用户强烈建议使用此命令时，配合大陆地区的 pypi 镜像（可参考清华大学 Tuna）使用，以免因网络或哈希验证等原因导致依赖安装失败

3. 编写具体的训练、测试模型的代码，请参考本仓库的 example 目录下的示例，这里假设您的程序是一个名为 main.py 的文件（后续我再继续更新一份示例，请允许我思考一下如何组织这份代码）

4. 在激活的虚拟环境下，命令行键入`python3 main.py`，即可运行代码