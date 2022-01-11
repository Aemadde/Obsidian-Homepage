**中文说明请往下翻**

2022-01-11 Update:
1. Add status bar styling to the project tracking section. 


<img width="400" alt="Screen Shot 2022-01-11 at 3 46 06 PM" src="https://user-images.githubusercontent.com/58488160/148901554-0a82fbd2-8404-4589-82f3-af82c0a793bb.png">
<img width="400" alt="Screen Shot 2022-01-11 at 3 50 43 PM" src="https://user-images.githubusercontent.com/58488160/148902155-a1c2770f-3737-456b-893f-96b9da660342.png">


---

2022-01-07 Update:
1. Fixed mobile view of the homepage;
2. Made modifications to allow an all-theme homepage view.

---

# Obsidian-Homepage
A dashboard for your obsidian vault.


<img width="403" alt="IMG_7055" src="https://user-images.githubusercontent.com/58488160/147173306-3bdd2289-6dd1-4603-9ba7-24d8510dd29f.PNG">

## Features
Currently the homepage features 
1. A map of contents that leads to different parts in your vaults (such as your daily notes, weekly notes an other periodic notes);

<img width="403" alt="IMG_6675" src="https://user-images.githubusercontent.com/58488160/148902450-b1e55944-619b-471c-bf90-763f7f9725bc.GIF">


2. Three button tabs that allow you to switch between different parts you'd like to display. Currently there's a music of the month and automatic birthday countdown featured (this part is supported by React Components).  
3. A dynamic view of different sections in your daily note (in my case they are diaries, daily agendas, and my parrot logs)
<img width="400" alt="Screen Shot 2022-01-11 at 3 54 05 PM" src="https://user-images.githubusercontent.com/58488160/148902583-89cfc58f-4300-4495-ba6f-1eb93c915f20.png">

4. A project tracking for notes with the tag #project.
5. A Currently Reading section yet to be automatized
6. Obsidian activity.


## To use this homepage

1. Install Dataview, Banners, React Components, Admonition and Obsidian Activity;
2. The theme Blue Topaz is suggested;
3. Enable React Components; Create a components folder and put "music and birthday countdown.md" in it;
4. Add the two css files to your css snippets;
5. Dataview: enable dataviewjs and inline queries;
6. Admonition: create an "ad-col2" view with no background colors and no codeblock names;

<img width="400" alt="Screen Shot 2022-01-11 at 11 48 36 PM" src="https://user-images.githubusercontent.com/58488160/148975172-0553c210-6b53-4f39-b00e-e8bfd28cabc9.png">


7. Open the 00.Homepage note in your vault and get all sections personalized. 

## Extra notes
1. To use birthday countdown function, you'll need to create a page with the name of the persons/pets you'd like to have a countdown for and add "birthday: YYYY-MM-DD" in the YAML.
2. To use project tracking you'll need to have a
```
target: 10000
status: in progress
tags: project
```
in the YAML section of your single note project. It's based on https://gist.github.com/chrisgrieser/ac16a80cdd9e8e0e84606cc24e35ad99 so you can check there for more info. 

## Tricks
### Customizable Page Header
With this plugin you can quickly access your homepage (Homepage plugin required) from anywhere, both on PC and your phone. 

<img width="400" alt="Screen Shot 2022-01-11 at 11 27 19 PM" src="https://user-images.githubusercontent.com/58488160/148972407-0d7b57c5-39bf-4f90-9d1a-e77ff380d163.png">

Settings:

<img width="400" alt="Screen Shot 2022-01-11 at 11 45 03 PM" src="https://user-images.githubusercontent.com/58488160/148974533-0a0386c6-368d-4c51-b957-3b3c1b0a54f5.png">

### Advanced URI

With the plugin Advanced URI you can create a url for literally anything. Currently I am only using this for running two commands:
1. open big calendar
2. open memos
<img width="400" alt="Screen Shot 2022-01-11 at 11 37 18 PM" src="https://user-images.githubusercontent.com/58488160/148973246-454388c4-e1cf-4e2e-8a59-d737c49f03bf.png">

### Dynamic Buttons
There are several kinds of dynamic buttons in the MOC part.

1. Periodic Notes

Supposing you have a daily note formatted YYYY-MM-DD, you should write the md link as followed:
```
- `$= '[['+moment().format("YYYY-MM-DD")+'|Today]]'`
```
It'll create a button displaying "Today" and leads to your daily note.

2. URL scheme

If you are using Apple products, both MacOS and IOS have extensive URL schemes that allow you to open almost any app using URL, even perfoming some actions within the app (e.g. open a specific note; open a specific book in IBooks, etc.) I have installed a RSS reader called REEDER and am using this button to open it

```
	- [Reeder](reeder://)
```


# Obsidian 主页

<img width="400" alt="Screen Shot 2022-01-11 at 3 48 37 PM" src="https://user-images.githubusercontent.com/58488160/148901893-49b31f09-b23a-4d4c-853e-de8f42d09d76.png">

## 目前主页功能

1. 一个**导航**，可通向您的Obsidian库中的不同部分（例如您的每日笔记、每周笔记和其他定期笔记），
<img width="400" alt="Screen Shot 2022-01-11 at 3 54 05 PM" src="https://user-images.githubusercontent.com/58488160/148902583-89cfc58f-4300-4495-ba6f-1eb93c915f20.png">
2. 三个选项标签，可让您在要显示的不同部分之间切换。目前有**本月音乐**和自动**生日倒计时**功能。
3. **每日笔记**中不同部分的动态视图（在我的情况下，它们是日记、每日议程和我的鹦鹉日志）
4. 带有标签#project 的笔记**项目跟踪**。
5. **目前阅读**部分尚未自动化
6. Obsidian动态记录。


## 要使用此主页

1. 安装Dataview、Banners、React Components、Admonition和Obsidian Activity；
2. 建议使用 Blue Topaz 主题，因为它对 Admonition 的额外支持：安装主题后，下载插件 Style Settings 并在其中启用 Admonition Support（否则您可能没有包含日常笔记部分的分栏视图）
4. 启用React Components；创建一个components文件夹，把“音乐和生日倒计时.md”放进去；
5. 将这两个 css 文件添加到您的 css 片段中；
6. Dataview：启用dataviewjs和inline queries；
7. Admonition：创建一个没有背景颜色和代码块名称的“ad-col2”，配置如下图；
<img width="400" alt="Screen Shot 2022-01-11 at 11 48 36 PM" src="https://user-images.githubusercontent.com/58488160/148975172-0553c210-6b53-4f39-b00e-e8bfd28cabc9.png">
8. 在您的 Vault 中打开 00.Homepage，并让所有部分都个性化。

## 额外说明
1. 要使用生日倒计时功能，您需要创建一个页面，其中包含您想要倒计时的人/宠物的名称，并在 YAML 中添加“birthday：YYYY-MM-DD”。
2. 要使用项目跟踪，您需要有一个
```
target：10000
status：进行中
tags： project
```
在单笔记项目的 YAML 部分。它基于 https://gist.github.com/chrisgrieser/ac16a80cdd9e8e0e84606cc24e35ad99
因此您可以在此处查看更多信息。

## 技巧
### Customizable Page Header
使用此插件，您可以在 PC 和手机上的任何地方快速访问您的主页（需要Homepage插件）。


<img width="400" alt="Screen Shot 2022-01-11 at 11 27 19 PM" src="https://user-images.githubusercontent.com/58488160/148972407-0d7b57c5-39bf-4f90-9d1a-e77ff380d163.png">


设置：

<img width="400" alt="Screen Shot 2022-01-11 at 11 45 03 PM" src="https://user-images.githubusercontent.com/58488160/148974533-0a0386c6-368d-4c51-b957-3b3c1b0a54f5.png">


### Advanced URI

使用插件 Advanced URI，您可以为几乎任何内容和操作创建一个 url。目前我只使用它来运行两个命令：

1.打开Big Calendar
2.打开Memos

<img width="400" alt="Screen Shot 2022-01-11 at 11 37 18 PM" src="https://user-images.githubusercontent.com/58488160/148973246-454388c4-e1cf-4e2e-8a59-d737c49f03bf.png">


### 动态按钮
MOC部分有几种动态按钮。

1. 定期笔记

假设您有一个格式为 YYYY-MM-DD 的每日笔记，您应该如此编写 md 链接，如下所示：
```
- `$= '[['+moment().format("YYYY-MM-DD")+'|今天]]'`
```
它将创建一个显示“今天”的按钮并指向您的每日笔记。

2. URL方案

如果您使用的是 Apple 产品，MacOS 和 IOS 都有详尽的 URL 方案，允许您使用 URL 打开几乎任何应用程序，甚至可以在应用程序内执行某些操作（例如打开特定笔记；在 IBooks 中打开特定书籍等）我安装了一个名为 REEDER 的 RSS 阅读器，并使用此按钮打开它
```
	- [Reeder](reeder://)
```
