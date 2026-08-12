# San 论文毕设 - 官网

## 文件结构

```
论文业务官网/
├── index.html              ← 主页面
├── images/
│   ├── cases/              ← 案例截图（6个位置）
│   │   ├── case1.png       ← 金融学本科论文
│   │   ├── case2.png       ← 工商管理硕士论文
│   │   ├── case3.png       ← 会计学降重案例
│   │   ├── case4.png       ← 计算机本科论文
│   │   ├── case5.png       ← 客户好评截图1
│   │   └── case6.png       ← 客户好评截图2
│   └── wechat-qr.png       ← 微信二维码
└── README.md
```

## 如何添加案例截图

1. 将截图放到 `images/cases/` 文件夹
2. 按顺序命名：`case1.png`, `case2.png`, ... `case6.png`
3. 图片建议尺寸：宽 800px+，高度自适应
4. 如果图片加载失败，会显示"📄 案例截图"占位文字

## 如何添加微信二维码

1. 将微信二维码图片放到 `images/wechat-qr.png`
2. 建议尺寸：300x300px 以上

## 部署到服务器

### 方式一：直接上传
将整个 `论文业务官网/` 文件夹上传到服务器 web 目录即可。

### 方式二：GitHub Pages
```bash
cd 论文业务官网
git init
git add .
git commit -m "初始版本"
git remote add origin https://github.com/你的用户名/论文业务官网.git
git push -u origin main
```
然后在 Settings → Pages → Source 选择 main 分支。

### 方式三：Vercel / Netlify
直接拖拽文件夹到 vercel.com 或 netlify.com 即可部署。

## 后期维护

| 操作 | 怎么做 |
|------|--------|
| 新增案例 | 往 `images/cases/` 放截图，告诉我更新HTML |
| 删除案例 | 删图片即可，告诉我清理HTML引用 |
| 改价格/文案 | 告诉我改什么，我直接改HTML |
| 换服务器 | 整个文件夹搬过去就行，零配置 |

## 导航结构

1. **首页** - Hero大图 + 核心卖点 + CTA按钮
2. **服务项目** - 论文写作/降重/辅导/答辩PPT
3. **案例展示** - 过往作品截图、好评截图
4. **价格** - 透明报价，按类型/字数分级
5. **流程** - 下单→沟通→初稿→修改→交付
6. **联系我们** - 微信扫码 + 悬浮CTA按钮
