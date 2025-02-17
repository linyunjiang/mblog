## [atom](https://atom.io/) 编辑器的安装/插件的安装使用

![chmod-d](https://raw.githubusercontent.com/FlowerWrong/mblog/master/screen/category-linux-atom-setiui.png)
![chmod-d](https://raw.githubusercontent.com/FlowerWrong/mblog/master/screen/category-linux-atom.png)


#### atom ubuntu 中文显示方框问题

```ruby
# 安装文泉驿正黑字体 ubuntu 14.04 and 15.04
sudo apt-get install fonts-wqy-zenhei

# 配置atom字体
DejaVu Sans Mono, 文泉驿正黑
```

#### 安装 [atom](https://atom.io/) 编辑器 via ppa

```bash
# atom
sudo add-apt-repository ppa:webupd8team/atom
sudo apt-get update
sudo apt-get install atom
```
#### 插件的安装, [linter-jshint](https://github.com/AtomLinter/linter-jshint)，`jshint`是js的语法检查插件

1. 先安装 [linter](https://github.com/AtomLinter/Linter) 插件

        mkdir -p ~/software/atom-plugins
        cd ~/software/atom-plugins/
        git clone https://github.com/AtomLinter/Linter.git
        cd ~/software/atom-plugins/Linter/
        npm install # 需要安装nodejs
        apm uninstall linter
        apm link
        apm install

2. 安装 [linter-jshint](https://github.com/AtomLinter/linter-jshint)

        cd ~/software/atom-plugins/
        git clone https://github.com/AtomLinter/Linter.git
        cd ~/software/atom-plugins/linter-jshint/
        npm install # 需要安装nodejs
        apm uninstall linter-jshint
        apm link
        apm install

3. [其他插件列表](https://atom.io/packages)
4. [主题列表](https://atom.io/themes)
5. 无论插件还是主题，安装都同上
6. 卸载插件

        cd ~/software/atom-plugins/linter-jshint/
        apm unlink
        apm uninstall linter-jshint
        cd ../
        rm -rf linter-jshint/

#### 插件推荐(不要安装过多的插件)

1. [linter and his firents](https://github.com/AtomLinter/Linter)
2. [atom-beautify](https://atom.io/packages/atom-beautify) to use erb-beautify `gem install htmlbeautifier`
3. [autocomplete-plus](https://atom.io/packages/autocomplete-plus)
4. [autocomplete-paths](https://github.com/saschagehlich/autocomplete-paths)
5. [ctrl+shift+p](https://github.com/atom/command-palette)

#### beautify html and erb
```ruby
gem install htmlbeautifier

ctrl+shift+p
B
```
