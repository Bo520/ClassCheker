# Class Checker
一个用于核对班级应到人数以及班级对应学院的程序，前端基于PyQt5，数据分析与处理基于pandas。
Author: Bo Cai  
Mail: [caibo0520@qq.com](caibo0520@qq.com)
# 开发环境搭建
建议基于以下步骤使用`Anaconda`重建程序开发环境：
1. 创建`Anaconda`环境
```shell
 conda env create -f environment.yml
```
2. 进入刚刚新建好的`Anaconda`环境
```shell
conda activate pyqt5
```
3. 导出`requirements.txt`
```shell
while read requirement; do  pip install $requirement; done < requirements.txt
```
# 运行方式
在搭建好的环境中直接运行`ClassCHecker.py`即可：
```shell
python ClassCHecker.py
```
在PyCharm中的配置方式请自行解决。

# 程序打包方式

这里只是用了最简单的打包方式--`pyinstaller`，简单易操作，但是打包后的文件很大，后续再优化。

```shell
pyinstaller -F -w --clean --i ".\header.ico" .\ClassCHecker.py
```

# 运行效果

![image-20210627180447023](https://gitee.com/vancomycin_bo/markdown_img/raw/master/img/20210627180449.png)
