# TOMORROW PORTFOLIO 开源项目介绍
TOMORROW PORTFOLIO 是一个开源简约的个人摄影和作品集框架，旨在为摄影爱好者提供网上展示空间，代码开源
项目示范地址 [portfolio.mrzxr.com](https://portfolio.mrzxr.com)
项目示范：
![image](https://github.com/user-attachments/assets/bd789fa7-12ef-4d7f-94e3-8d96c7bbc4cb)
![image](https://github.com/user-attachments/assets/77ad9a72-aea8-4c81-8ed5-176915385640)
![image](https://github.com/user-attachments/assets/cd3cd3c8-909c-4811-95eb-168496d22fe1)


当前最新版本：v1.2.1
# 1 项目特点
### 1.1 上手简单
   - 为方便开源，此项目所有的css，js代码经过作者优化，均在同一个html文件中，上手非常方便。仅需下载，编辑，部署三步即可上线，您可快速拥有属于自己的照片作品集
   - 照片自适应：本项目开发了照片自适应功能，您无需更改照片大小，页面会根据您的照片大小自动适应。只需准备一个图床直接引入链接即可（图床推荐sm.ms）
### 1.2 动画丝滑
   - 动画效果：网站应用了多种动画效果，包括开屏动画，标题渐入等。使页面切换和元素展示更加流畅和吸引人。
   - 滚动触发动画：使用 GSAP 和 ScrollTrigger 实现的滚动触发动画，让页面内容在用户滚动时逐步显现，提升用户体验。
   - 图片悬停效果：图片在鼠标悬停时会放大并显示阴影效果，增强视觉效果和互动性。
   - 文字动画效果：当鼠标悬停在文字上时，文字会放大并呈现青蓝色（颜色可改）。
   - 图片淡入效果：您的图片会随着用户的滚动位置而淡入，给予访客良好的视觉体验，展现您的个性。
   - 彩色渐变背景：最新版本v1.2.0开发了渐变背景，让您的个性得到更好的展现
### 1.3 布局灵活
   - 移动优先设计：网站采用响应式设计，确保在不同设备和屏幕尺寸上都能有良好的展示效果。
   - 自适应布局：开发了灵活的布局和媒体自适应代码，使网站在桌面、平板和手机上都能正常显示。
### 1.4 UI简洁优雅
   - 现代化设计：网站采用简洁优雅的设计风格，配色和排版都经过精心设计，使整个页面看起来干净整洁。
   - 易于导航：清晰的导航栏和页面结构，使用户可以轻松找到所需内容

# 2 安装（分为本地和线上两部分，因本项目规模不大，推荐使用线上安装）
## 2.1 线上安装

1.在您的GitHub账户中新建一个仓库，标题随意

2.新建index.html

3.将本仓库中的index.html中的所有代码拷到您的仓库中

4.打开您的index.html

VOLA

## 2.1本地安装
要在本地运行此项目，请按照以下步骤操作：
1. 克隆存储库：

    ```bash
    git clone https://github.com/terryzhangxr/terryzhang-portfolio.git
    ```

2. 进入项目目录：

    ```bash
    cd terryzhang-portfolio
    ```

3. 打开 `index.html` 文件

VOLA

# 3配置教程 
无论您是线上安装还是本地运行，以下方法均适用

1.更改标题
  在index.HTML中找到```<head>```部分的```<title>```，在字符串中将原本示范站标题改为您的标题。随后在紧接着下面一行的```<link real="icon" href="此处改成您的logo图床链接" type="image/x-icon">```改成您的logo效果如下
  ![image](https://github.com/user-attachments/assets/2ac1f6a5-5d0b-4943-903a-d831d5268c30)


  
2.更改开屏动画，首页显示
  在```<body>```中找到```<div id="overlay">您的标题</div>```改标题，当开屏动画出现时将显示
  在```<body>``` ```<header id="main-header">```部分找到```<h1>Terryzhang's Photo Portfolio</h1>```将两个h1之间的内容改为您的标题，效果如下
  ![image](https://github.com/user-attachments/assets/3ff83abb-0824-482c-9fc0-a13d1785413d)




3.更改首页链接
  在刚刚改动的标题部分下方找到如下代码
  ![image](https://github.com/user-attachments/assets/99d64acf-2c80-4672-8680-a99f0848546e)
  这样编辑您的链接```<div><a class="fx0" href="您的链接" onclick="return handleLinkClick(event)">文本</a></div>```
   ```
      <div><a class="fx0" href="#portfolio" onclick="return handleLinkClick(event)">Photos</a></div>
      <div><a class="fx0" href="#contact" onclick="return handleLinkClick(event)">Contact</a></div>
   ```
  这两行是本站快捷定位链接，您可以改动文本中的内容，但建议您不要随意改动前面链接里的定位链接，可能导致点击后无法对应定位
  
  效果如下
   ![image](https://github.com/user-attachments/assets/19d1f9c4-7cf4-4203-b82a-70b4c7539977)



  
 4.更改关于界面
   找到如下代码
   ![image](https://github.com/user-attachments/assets/c1eacae2-1635-49f3-8782-f855b424d6e7)
   将中文字和最后一行链接内容改为您自己的内容
   若要增加行数，请按照如下格式并按照前行缩进
   ```<p>内容</p>```
   效果如下
   ![image](https://github.com/user-attachments/assets/73bccbcd-fd20-4e05-9e65-67477c0bce76)



  5.增加您的图片
    找到如下代码
    ![image](https://github.com/user-attachments/assets/430c60cf-41f2-4e16-ac18-8ea1fb252043)
    将```<div class="photo"><img src="photo2.jpg" alt="Photo 2"></div>```的photo改成您的图床链接，您可继续用这种格式添加图片，数量不限
    效果如下
    ![image](https://github.com/user-attachments/assets/ebe37e96-0b2c-4f51-8df8-2e48332494fa)




  6.更改联系板块
    紧接着图片的就是联系板块，将```<p class="email">Email: zhang@mrzxr.com</p>```中的Email改为您的邮箱，同样您可以按照您的喜好添加联系方式




  7.进阶玩法
    本项目为开源作者已经添加好了所有的注释，希望有更高自定义度并且有代码基础的用户可以根据注释更改。新手请慎重




# 部署（此处为vercel）

   (本地用户需先将index.html推到GitHub仓库上)
   
   1.注册并登录 Vercel
   
   2.访问 [Vercel](https://vercel.com) 并注册一个账号，或者登录你的现有账号。

   3.新建项目
     点击 "New Project" 按钮，然后选择 "Import Git Repository"。
     授权并选择存储库
     授权 Vercel 访问你的 GitHub 账号，然后选择您的本项目存储库。


   4.配置部署设置
     在部署设置页面：
      Framework Preset 选择 "Other"。
      Build command 留空
      Output directory 设为 /（根目录）。
     点击部署即可
     注：部署完成后vercel会自动分配一个 xxx.vercel.app,在国内被墙，如果您想要让国内用户访问，建议绑定自己的域名
     好啦，现在就可以看看你的网站了

# 贡献
   项目创建者：[terryzhang](https://github.com/terryzhangxr)
   
   欢迎对本项目做出贡献！请遵循以下步骤提交您的贡献：
   1. Fork 此存储库
      
   2. 创建一个新的分支 (`git checkout -b feature-branch`)
 
   3. 提交您的更改 (`git commit -m '添加新特性'`)
    
   4. 将更改推送到分支 (`git push origin feature-branch`)
    
   5. 打开一个 Pull Request
    
   6. 向作者写一封邮件到 [zhang@mrzxr.com](mailto:zhang@mrzxr.com)

      在此感激您的伟大贡献
      
   ### 如果您觉得项目还不错，还恳请您给个star支持下作者，感激不尽！
   
项目持续更新中，更多精彩欢迎移步 [www.mrzxr.com](https://www.mrzxr.com)



## 更新情况：
   2025.1.20 v1.0.0发布  初版
   
   2025.1.21 v1.0.1发布  更新了页面的布局排版以及优化了适配度

   2025.1.21 v1.2.0发布  增加动态背景，对于用户图片增加懒加载 

   2025.1.23 v1.2.1发布  优化代码逻辑，修改bug
   
版权所有 © 2025 Terryzhang. 保留所有权利。

本项目的代码和文档可随意转发使用。但未经授权不得用于商业用途。


  



  
  
