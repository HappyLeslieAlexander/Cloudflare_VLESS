# Cloudflare_VLESS

在 CloudFlare Workers 或 Pages 部署 VLESS 节点

## 部署教程

进入Cloudflare官网，注册一个新账户（如果你有请跳过）

进入Workers & Pages，创建一个新Worker或Pages

进入代码后台，把原来的js全部删掉，复制本项目_worker.js中的所有代码，粘贴进js里

用V2RayN生成一个UUID，替换第八行的UUID，保存

绑定你自己的Cloudflare的域名，必须解析到Cloudflare的名称服务器并添加至Cloudflare（可跳过）

访问 https://DOMAIN.workers.dev/UUID ，即可查看节点明文配置信息

访问 https://DOMAIN.workers.dev/UUID/base64 ，即可使用 Base64 通用客户端订阅

访问 https://DOMAIN.workers.dev/UUID/clash ，即可使用 Clash 节点订阅

访问 https://DOMAIN.workers.dev/UUID/sb ，即可使用 Sing-box 节点订阅

拷贝节点订阅，如果没有域名，需要搭配IP优选（因为worker.dev域名被墙了，非TLS也可优选），且不可用非TLS端口（因为worker.dev域名默认使用https）

将节点订阅导入V2RayN或V2RayNG，即可使用，或搭配Cloudflare的IP优选使用，替换原本的地址（其他的不要动）

## 鸣谢

项目大部分代码来自 https://github.com/Misaka-blog/cf-wkrs-pages-vless/tree/main 为了避免原作者删库跑路Clone了此仓库
