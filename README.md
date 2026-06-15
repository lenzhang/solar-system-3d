# 3D 太阳系演示

基于 Three.js 的交互式 3D 太阳系可视化，纯前端单文件项目，浏览器直接打开即可运行。

## 功能

- 八大行星真实比例轨道运动
- 行星高清贴图（太阳、水星、金星、地球、火星、木星、土星、天王星、海王星）
- 土星环、月球等卫星
- 小行星带和彗星模拟
- 星系漫游模式（自动巡游各星体）
- 轨道线、标签显示切换
- 速度控制、暂停/重置
- 点击星体查看信息

## 使用

直接在浏览器中打开 `index.html` 即可。

如果遇到跨域限制（贴图加载失败），可以用任意本地 HTTP 服务器：

```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve .
```

## 项目结构

```
├── index.html          # 主页面（含全部逻辑）
├── assets/
│   ├── three.min.js    # Three.js r152
│   ├── OrbitControls.js
│   ├── sun.jpg
│   ├── earth.jpg
│   ├── moon.jpg
│   └── ...             # 各行星贴图
└── README.md
```

## 技术栈

- [Three.js](https://threejs.org/) r152
- 原生 HTML/CSS/JavaScript，无构建工具依赖
