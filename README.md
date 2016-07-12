# blackhatpythonbook-Chapter7
使用github作为受控程序控制中心和数据中心

ps：使用主账号存在风险，所以使用edxDev这个测试账号做测试 

# Usage
*  mv local.yaml.template local.yaml
*  填入你的github的用户名和密码
*  pip install github3.py 
*  python git_trojan.py

之后你的本机数据将每隔一段时间上传到data/abc目录中，值得注意的是，数据经过base64编码

你也可以在modules目录下新建功能脚本，脚本将被定期拉到client执行


#  坑
### pyinstaller
*  pyinstaller --onefile git_trojan.py 能能通过
*  pyinstaller 编译python2脚本时Queue会找不到， 使用2to3转为python3编译，会进进下一个问题
*  github3.py引用的requests会报错，编码问题（python2和3都存在）
