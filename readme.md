# 项目描述

agy项目的接口自动化测试用例

# 环境准备
- python3.6
- windows/linux/mac

# 依赖包
使用pip 安装python依赖包，在项目根目录下有个requirements.txt文件
cd到项目根目录，命令行安装
导出依赖包：
pip freeze > requirements.txt
安装依赖包：
pip install -r requirements.txt

# 运行用例
cd到项目根目录，直接通过pytest命令行执行
> pytest

# 测试报告
1、安装allure
pip install pytest==4.5.0 
pip install allure-pytest==2.8.6
2、安装allure命令行工具，bin目录配置到系统环境变量

使用Allure在./report目录下会生成html报告，dos命令如下：
pytest --alluredir ./report/allure_raw --clean-alluredir
allure serve -p 9099 report/allure_raw
