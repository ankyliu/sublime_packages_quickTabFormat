# sublime_快速格式化宏

很多时候我们在看别人网页原码的时候，代码排版都很乱，于是找到了HTML-CSS-JS Prettify，可以通过Ctrl+Shift+H来在Sublime中快速格式化代码。但是格式化完有时候可能是tab2空格缩进的，有时候又是tab4字节缩进的。总要手动去改完再执行一个格式化操作。

在知乎上看到有朋友用宏做了一系列的操作。受益匪浅，现学现用的写了这个快速将代码进行缩进替换并格式化的宏。分享出来大家可以按需修改。


使用前请确认已正确安装HTML-CSS-JS Prettify（插件地址：https://packagecontrol.io/packages/HTML-CSS-JS%20Prettify）

以下是Win版本的快捷键设置，请确认两个文件正确解压到Sublime3安装目录下的Data\Packages下  
在快捷键中增加以下绑定，可以自己自己习惯修改
安装成功后用Ctrl+2来格式化成tab2空格缩进  
安装成功后用Ctrl+4来格式化成tab4字节缩进(默认是不使用空格缩进的)  

```
{
        "keys": ["ctrl+2"],
        "command": "run_macro_file",
        "args": {
          "file": "Packages/tab2fmt.sublime-macro"
        }
      },
      {
        "keys": ["ctrl+4"],
        "command": "run_macro_file",
        "args": {
          "file": "Packages/tab4fmt.sublime-macro"
        }
      }
```
