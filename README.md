# Three.js STL模型动画展示

这是一个使用Three.js创建的简单网页应用，用于展示STL模型的跳跃和旋转动画效果。

## 项目文件

- `index.html` - 基本的HTML页面结构
- `main.js` - Three.js的主要代码，负责加载STL模型和创建动画
- `cookie.stl` - 3D模型文件
- `server.js` - 用于本地开发的简单Node.js服务器

## 如何运行

### 前提条件

- 安装Node.js (https://nodejs.org/)

### 运行步骤

1. 打开命令行终端，进入项目所在文件夹
2. 运行以下命令启动本地服务器：
   ```
   node server.js
   ```
3. 在浏览器中访问：`http://localhost:3000`

## 功能说明

### 动画控制
界面底部有一排控制按钮，可以切换不同的动画效果：

- **蹦蹦跳跳**：模型只进行上下跳跃运动
- **转圈圈**：模型只进行旋转运动
- **一起动**：模型同时进行跳跃和旋转运动
- **暂停**：暂停所有动画
- **切换背景**：循环切换不同的背景效果

### 背景效果
应用提供多种背景效果：

1. 默认浅灰色背景
2. 天蓝色背景
3. 浅粉色背景
4. 蓝粉渐变背景
5. 星空背景

### 交互控制
- 使用鼠标拖拽来旋转视角
- 滚轮缩放视图

## 自定义设置

如果要调整动画效果，可以修改`main.js`文件中的以下参数：

- `jumpHeight` - 控制跳跃的高度
- `jumpSpeed` - 控制跳跃的速度
- `rotationSpeed` - 控制旋转的速度

如果要添加或修改背景，可以编辑`backgrounds`数组。 