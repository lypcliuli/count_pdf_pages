# count_pdf_pages

查看pdf文件总页数：

cd 进入到count_pdf_pages.py文件所在目录

查看文件夹内所有pdf文件页数总和：
python3 count_pdf_pages.py /Users/LYPC/Documents/jieyafile/shuxue

查看一个文件夹内所有子文件夹内的pdf页数总和：
 python3 count_pdf_pages.py /Users/LYPC/Documents/jieyafile -r

如果是加密的一些pdf文件 无法读到回报错
raise utils.PdfReadError("File has not been decrypted")

 
<img width="649" alt="LYPCOLYPC oMRenEssncurorvagesl" src="https://user-images.githubusercontent.com/12068023/137250085-036f68b6-8b6d-47e1-a950-b8cc725cee27.png">


￼运行.py文件时，python 可执行文件文件名即可运行，但此时可能使用的是系统默认的python2，如果以后每次都想用自己的python3来运行，修改配置文件.zprofile(使用echo $SHELL,可以查看当前使用的shell，我的是zsh，如果是bash的话，则去修改.bash_profile)即可，vi ~/.zprofile打开文件，在文件中加入一行代码：
alias = "/Library/Frameworks/Python.framework/Versions/3.9/bin/python3.9"


