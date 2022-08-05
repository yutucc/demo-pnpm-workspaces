# Demo 演示 pnpm workspaces 的用法


## 环境
node 版本要大于等于 14

pnpm 版本要大于等于 7

## 命令
根目录执行：

```
pnpm add @pn/components @pn/models -r --filter @pn/web

pnpm start
```

然后就可以看见一下执行效果：

![](https://tva1.sinaimg.cn/large/b3cc33a0gy1h4vznzkrvhj20gb03e3z1.jpg)

## 补充
另外，如果想把项目放在 apps 目录下，把公共库放在 packages 目录下，可以直接在 `pnpm-workspace.yaml` 增加一行 `- 'apps/*'`

然后在根目录执行：

```
pnpm add @pn/components @pn/models -r --filter @pn/exam

pnpm run start:exam
```

即可看到以下效果：

![](https://tva1.sinaimg.cn/large/b3cc33a0gy1h4w0fgaefoj20hm03odgf.jpg)
