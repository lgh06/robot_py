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

# 其它链接  
rcc github https://github.com/robocorp/rcc/blob/v17.12.0/docs/recipes.md  
.condarc https://docs.conda.io/projects/conda/en/23.11.x/user-guide/configuration/use-condarc.html  
micromamba https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html  
robot framework 如何安装 https://github.com/robotframework/robotframework/blob/v6.1.1/INSTALL.rst  
robot framework 用户指南 v6.1.1  https://robotframework.org/robotframework/6.1.1/RobotFrameworkUserGuide.html  
robot framework 用户指南 v6.1.1 github https://github.com/robotframework/robotframework/blob/v6.1.1/doc/userguide/README.rst  
Robot Framework Guides https://docs.robotframework.org/docs  
Robot Framework Guides Github https://github.com/MarketSquare/robotframeworkguides  
此项目从这篇教程而来 https://docs.robotframework.org/docs/getting_started/rpa  

Robocorp:  
https://github.com/robocorp/robocorp  
https://github.com/robocorp/robo  
https://github.com/robocorp/robo/blob/robocorp-1.3.0/docs/guides/using-with-rcc.md  
https://github.com/robocorp/rcc  

防火墙内环境变量设置 https://robocorp.com/docs/troubleshooting/firewall-and-proxies  
template-python https://github.com/robocorp/template-python  

# 目前版本  
日期 2024-01-07  
```  
python --version
Python 3.11.4

robot --version
Robot Framework 6.1.1 (Python 3.11.4 on win32)

rcc --version
v17.12.0


```

# Github  
git config http.sslVerify false
Watt Toolkit  





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