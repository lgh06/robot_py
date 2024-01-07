# Robot Framework and Robocorp's RPA framework  
RCC is a command line tool.  
anaconda / miniconda / conda 是封装了科学计算常用的包管理器
mamba / micromamba 是conda的C++ 最小化实现，除了命令是mamba，其他功能完全一致。

# mirror 与 环境变量  

## Python  

C:\Users\Administrator\pip.ini  
C:\Users\Administrator\AppData\Roaming\pip\pip.ini  

```
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```

## conda  
C:\Users\Administrator\.condarc  
```
channels:
  - defaults
show_channel_urls: true
default_channels:
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/r
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/msys2
custom_channels:
  conda-forge: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  msys2: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  bioconda: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  menpo: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch-lts: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  simpleitk: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  deepmodeling: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/
ssl_verify: false
```



# 以下是rcc生成的项目的原始readme


# Template: Python - Minimal

This template leverages the new Python open-source structure [robo](https://github.com/robocorp/robo), the [libraries](https://github.com/robocorp/robo#libraries) from to same project as well.
The full power of [rpaframework](https://github.com/robocorp/rpaframework) is also available for you on Python as a backup while we implement new Python libraries.

The template provides you with the basic structure of a Python project: logging out of the box and controlling your tasks without fiddling with the base Python stuff. The environment contains the most used libraries, so you do not have to start thinking about those right away. 

👉 After running the bot, check out the `log.html` under the `output` -folder.

The template here is essentially empty, leaving you with a canvas to paint on.

Do note that with Robocorp tooling you:
- Do NOT need Python installed
- Should NOT be writing `pip install..`; the [conda.yaml](https://github.com/robocorp/template-python/blob/master/conda.yaml) is here for a reason.
- You do not need to worry about Python's main -functions and, most importantly, the logging setup

🚀 Now, go get'em

For more information, do not forget to check out the following:
* [Robocorp Documentation -site](https://robocorp.com/docs)
* [Portal for more examples](https://robocorp.com/portal)
* [robo repo](https://github.com/robocorp/robo) as this will developed a lot...