# 配置Arch Linux



## 常用软件

 1.浏览器 ：google-chrome firefox

2.下载工具：motrix

3.yay git zsh 

4.开发：visual-studio-code-bin

5.字体：**noto-fonts** **noto-fonts-cjk noto-fonts-emoji** [adobe-source-han-serif-cn-fonts](https://archlinux.org/packages/?name=adobe-source-han-serif-cn-fonts)  [wqy-zenhei](https://archlinux.org/packages/?name=wqy-zenhei)  archlinuxcn/nerd-fonts-complete

6..输入法： fcitx fcitx-libpinyin fcitx-table-other fcitx-table-extra fcitx-qt5 fcitx-configtool

7.Typora

8.create_ap

9.截图工具：deepin-screenshot

10.生产力工具 utools screenkey

11.游戏 steam （需要启用mutilib）









Kde插件

panon lanuchpad-plasma  Netspeed-Widget



yay换源

```bash
yay --aururl "https://aur.tuna.tsinghua.edu.cn" --save
```

**系统美化**

kde plasma 样式

WhiteSur-dark 

窗口装饰也是WhiteSur

图标：sudo pacman -S papirus-icon-theme

连接到github

```bash
ssh-keygen -t rsa -C "1041370212@qq.com"
```



配置终端

改变终端为zsh

````bash
chsh -s /bin/zsh #在konsole里面可以不需要这个操作直接在设置里面更改就行了
````



```bash
git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh    # 下载oh-my-zsh
```



```bash
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc 
#下载好了就有一个模板了，然后复制到家目录就好了
```

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
# 下载一些常用的插件 autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/z	sh-syntax-highlighting
#自动高亮
```

```bash
vim ~/.zshrc #在pulgin那一个括号里面加上这两个插件的名称
```

终极美化powerline10K

https://github.com/romkatv/powerlevel10k#oh-my-zsh

```bash
git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
#下载powerlne10K
```

```bash
vim ~/.zshrc
# ZSH_THEME="powerlevel10k/powerlevel10k"  将主题设置为powerline10K
```

需要下载一些字体才能正常显示完成

- [MesloLGS NF Regular.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS NF Regular.ttf)

- [MesloLGS NF Bold.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS NF Bold.ttf)

- [MesloLGS NF Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS NF Italic.ttf)

- [MesloLGS NF Bold Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS NF Bold Italic.ttf)

- 上面的字体下载不了，所以采用下面的方法，也可以试一试yay nerd-fonts

  ```bash
  git clone https://github.com/ryanoasis/nerd-fonts.git --depth 1
  cd nerd-fonts
  ./install.sh
  ```
  
  
