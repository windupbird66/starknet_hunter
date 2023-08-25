![Image text](https://github.com/windupbird66/img_folder/blob/main/31631692951655_.pic_hd.jpg)

## 1. 准备环境

确保你安装了以下组件：

**Python**：该脚本使用Python编写，所以您需要安装Python。

**ChromeDriver**：脚本使用Selenium库与Chrome浏览器交互，因此您需要安装ChromeDriver。  

> 下载对应的版本：https://googlechromelabs.github.io/chrome-for-testing/  

**Selenium和undetected_chromedriver**：这些是Python库，您可以使用以下命令安装：

```bash
pip install selenium undetected-chromedriver
```

## 2. 配置config.ini文件

确保以下设置正确：

#### chrome：设置Chrome的用户数据目录

chrome目录里面user_data_dir是自己的要打开的chrome用户数据目录，下面profile_directory是具体哪个个人资料 这两个配置可以通过chrome://version获取到。

#### argent：设置argent钱包密码

argent目录仅仅只需要修改argent_password就可以，这个是解锁argent钱包，后续可以优化下，浏览器打开解锁页面，让用户输入。但是这样没有办法无人值守了，反正各种有利有弊。

#### task：设置交换任务的相关信息

task里面第一个是打开网址，第二个是input_number输入法数量，目前刷选出来是usdc/usdt交易兑，如果延展开发，可以做input_number随机数值，然后其他交易对也可以更改。

## 3. 运行脚本

在配置文件和脚本都准备好之后，你可以通过以下命令在命令行中运行脚本：

```bash
python starknet_swap.py
```

## 4. 安全注意事项

不保证是否会泄漏私钥：请自行选择是否使用。

测试和审查：如果可能的话，在生产环境之外的安全环境中先测试脚本，确保它的功能和安全性符合您的要求。

## 微信：wind-up-bird2
