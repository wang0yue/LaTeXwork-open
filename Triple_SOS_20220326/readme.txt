Triple_SOS机器配方程序安装说明
该说明文档大致可以帮助不会用python的人使用上Triple_SOS

作者：豪神
说明文档：浩于长空
时间：20220326
系数阵交流群：875413273
系统：Windows 7 64位


安装python-3.7.5-amd64.exe

打开安装目录(C:\Users\Administrator\AppData\Local\Programs\Python\Python37)......(a)
和(C:\Users\Administrator\AppData\Local\Programs\Python\Python37\Scripts)......(b)

Triples Code 20220218里的是作者的源代码，将其复制到(a)
将patch1里的两个文件替换到(a)(只有这两个里面调用了pyside2，因为PySide6我用不了)

(b)下改目录为cmd，依次输入：

pip -V

pip.exe config set global.index-url https://mirrors.aliyun.com/pypi/simple/

pip.exe install --upgrade pip

pip -V

pip.exe install sympy
pip.exe install numpy
pip.exe install scipy
pip.exe install pyside2
pip.exe install matplotlib

(a)下输入python.exe graphics_main.py

如果没有LaTeX，将patch2里的sos_manager.py替换到(a)(区别在line 431)

以后就可以直接双击打开python.exe graphics_main.py了(可创建快捷方式)