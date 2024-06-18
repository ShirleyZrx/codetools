
## static check

pycodestyle -- pycodestyle是一款简单的代码检查工具，之前名字叫pep8，为了减少混淆改名成pycodestyle
pylint -- pylint是代码检查工具，不能自动修改代码，有对于的配置文件，可以参考google开源的pylintrc配置文件
PyFlakes -- 一个简单的python错误检查工具,通过解析源代码而不是import来检测不同的错误，通常只能检查出一些逻辑错误
flake8 -- 针对PEPE8进行代码规范提示，是对PyFlakes，pycodestyle的封装
autopep8 -- autopep8是一款将python代码自动排版为PEP8风格的工具，它使用 pycodestyle来决定哪部分代码需要格式化
yapf--yapf是google开源的一个用于格式化Python代码的工具，可以一键美化代码，支持两种规范：PEP8和Google Style
