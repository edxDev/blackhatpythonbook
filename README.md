# blackhatpythonbook-Chapter7
test 

# Usage
*  mv local.yaml.template local.yaml
*  填入你的github的用户名和密码
*  pip install github3.py 
*  python git_trojan.py

之后你的本机数据将每隔一段时间上传到data/abc目录中，值得注意的是，数据经过base64编码

你也可以在modules目录下新建功能脚本，脚本将被定期拉到client执行
