# Cloudflare_VLESS

在 CloudFlare Workers 或 Pages 部署 VLESS 节点

## 部署教程

Workers 教程地址：https://blog.misaka.rest/2023/07/29/cf-wkrs-vless/

Pages 教程地址：https://blog.misaka.rest/2023/07/29/cf-pages-vless/

进入Cloudflare官网

进入Workers & Pages，创建一个新Worker或Pages

进入代码后台，把原来的js全部删掉，复制本项目_worker.js中的所有代码，粘贴进js里

用V2RayN生成一个UUID，替换第八行的UUID，保存


访问 https://DOMAIN.workers.dev/UUID ，即可查看节点明文配置信息

访问 https://DOMAIN.workers.dev/UUID/base64 ，即可使用 Base64 通用客户端订阅

访问 https://DOMAIN.workers.dev/UUID/clash ，即可使用 Clash 节点订阅

访问 https://DOMAIN.workers.dev/UUID/sb ，即可使用 Sing-box 节点订阅

将节点订阅导入V2RayN或V2RayNG，即可使用，或搭配Cloudflare的IP优选使用，替换原本的地址（其他的不要动）

默认域名为 www.gov.se ，可以替换成任意套了Cloudflare CDN的域名（如www.visa.com speed.cloudflare.com leslieblog.top），也可以搭配IP优选将地址改为Cloudflare EndPoint 边缘IP

## 鸣谢

项目大部分代码来自 https://github.com/Misaka-blog/cf-wkrs-pages-vless/tree/main 为了避免原作者删库跑路Clone了此仓库

鸣谢项目
zizifn：https://github.com/zizifn/edgetunnel
3Kmfi6HP：https://github.com/3Kmfi6HP/EDtunnel
cmliu：https://github.com/cmliu/edgetunnel

### 捐赠

加密货币

TRC20

TY7n1xwiHCBqcQqGH1cxjTQqZTuTXbzB4S

ERC20

0xed57E7237E88ceC19d3Fd12A0D26bACb1DCc247b

TON

UQC4r4gxAIbOTEEZGG-C1Ffn9inRo24J7qw3U0dFfaIfKyFr

## 注意事项

由于 Workers 节点的 IP 变动频繁，因此请勿在此节点登录重要账号

## 遇到问题？

有问题请看 [Issues&Solutions](https://github.com/HappyLeslieAlexander/Cloudflare_VLESS/blob/main/Issues%26Solutions.md) ，看看是否已有解决方案，如无请开Issue，欢迎提交Pull Request

## 联系
Telegram: https://t.me/Depressed_LeslieAlexander/

E-mail: https://github.com/HappyLeslieAlexander/

项目地址: https://github.com/HappyLeslieAlexander/Cloudflare_VLESS/

By Leslie Alexander
