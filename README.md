# Vite + vue3 + electron 模板项目

快速开始一个electron + vue3项目，参考知乎文章 [Vite+Electron快速构建一个VUE3桌面应用 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/421460116)

### 1.克隆 & 安装依赖

```shell
git clone https://github.com/XiaoXianThis/electron-vue3-quickstart.git
```

```shell
cnpm install
```

---

### 2.运行项目

先修改 `electron/main.js`

```javascript
//是否开发模式（为了热更新）
const IS_DEV = true
```

然后

```shell
npm run electron:serve
```

---

### 3.打包

先修改 `electron/main.js`

```js
//打包前改成false
const IS_DEV = false
```

然后

```shell
npm run electron:build
```

---

### 修改软件信息

修改 `package.json`

```json
{
    "name": "electron-vue3-quickstart", //名称
  	"version": "0.0.1", //版本号
    
    "build": { //打包信息
        "appId": "com.appid", //包名
        "productName": "electron-vue3-quickstart", //软件名
        "copyright": "Copyright © 2022 APP", //版权信息
    }
}
```



