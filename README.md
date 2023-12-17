## Deployment

该项目修改自 [markdown-resume](https://github.com/mdnice/markdown-resume/)，在此基础上突破了一百行限制、优化了字体文件。以下为部署方案：

```powershell
set NODE_OPTIONS=--openssl-legacy-provider
yarn install
yarn start
```

由于 node.js 版本更新，导致部分软件加密算法失效，需设置改行后解决，详情参考 [StackOverflow](https://stackoverflow.com/questions/74726224/opensslerrorstack-error03000086digital-envelope-routinesinitialization-e)