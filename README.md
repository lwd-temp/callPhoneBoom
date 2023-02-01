
# callPhoneBoom
思路：通过爬取使用「莆田系医院」这一营销组件的企业,
我们可以得到数以万计真实企业的网址。
并通过程序模拟浏览，可以将攻击信息给到这些企业。最终达到「电话攻击」的目的。


## 声明
本项目仅供学习交流使用，勿作商业或非法用途。

所有用户个人行为与本项目无关。

## 搜集接口
本项目起步阶段，如果你对效果不满意，欢迎你为本项目寻找可用接口

利用百度搜索

找百度的莆田广告只要是https://ada.baidu.com/site/开头的都行

找到后提交本项目Issues或者提交pr皆可

## 使用教程
1. 下载
    ```shell script
     $ git clone https://github.com/olyble/callPhoneBoom.git
    ```
2. 安装 Selenium
   ```shell script
   $ pip3 install selenium
   ```
   安装 Selenium 之后，**需要安装对应浏览器的 Driver** ，参见 Selenium 文档 [1.3 节](https://selenium-python.readthedocs.io/installation.html#drivers)。 
    >Seleium 具体的介绍及使用方法可参见 [Selenium 文档](https://selenium-python.readthedocs.io)。

3. 配置

  在main.py中填入需要轰炸的手机号
  
<!--     配置文件为`config.py`，参数说明如下：
   ```python
   """
   攻击对象信息
   """ 
   target = { 
       "phone": "13012345678",             # 手机号
       "name": "小小明",                    # 姓名
       "email": "xx@xx.xx",                # 邮箱
       "address": "宇宙银河太阳系地球村",     # 地址
       "comment": "你好 不会～"             # 留言信息
   }
   
   """
   参数设置
   """
   settings = {
       "times": 100,                 # 攻击次数
       "timeout": 5,                 # 超时
       "driver":webdriver.Firefox(), # 使用的 driver
   }
   ``` -->

4. 运行程序
    ```shell script
    $ python3 main.py
    ```
5. Enjoy!

    运行截图：


## 目录说明


## TODO
1. 使用 PyQt5 实现用户界面。
2. 定时任务。
3. 使用 「HTTP 请求」替代「模拟浏览」。


## 许可
MIT
