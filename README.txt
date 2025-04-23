python版本：3.8.19

1、创建conda环境命令
conda create --name test1 python=3.8

2、安装库包
①安装单个库包
pip install streamlit==1.33.0 -i https://pypi.tuna.tsinghua.edu.cn/simple

②直接从文档导入安装库包
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple

需要的包
streamlit==1.33.0
pandas==1.5.3
scikit-learn==1.2.2
wordcloud==1.9.3
matplotlib==3.7.1
selenium==4.15.0
jieba==0.42.1
webdriver-manager==3.8.6

3、生成一个requirements.txt文件，以便能够使用pip命令批量下载并安装所有列出的库包
pip freeze > requirements.txt
【注意，pip freeze命令会导出当前环境中所有库包的信息，包括那些可能不是通过pip安装的库包。如果你只想导出通过pip安装的库包，可能需要手动编辑requirements.txt文件，或者使用额外的脚本来过滤库包列表。】


