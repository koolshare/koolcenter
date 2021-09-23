# KoolCenter

此项目存储所有 [KoolCenter](https://www.koolcenter.com) 的文章，并且能独立运行。

## 准备

安装好 nodejs  hugo

### 更新最新代码

```bash
git submodule update --init --recursive
```

## 运行    

```bash
npm install
npm install hugo-extended --save-dev
npm run dev
```

使用Hugo作为内容生成和管理

### 主题

`./themems/docsy`

主题是另外一个仓库，最好别改主题代码

### 内容

`./content`

### 其他

很多重要配置信息在：

```
./config/_default/config.toml
```


