# DMIT 外贸建站怎么选：访客在海外该买 T1 还是 Pro？洛杉矶、香港、东京机房怎么挑？（附全套餐价格表与 3 个容易买错的点）

做外贸独立站，访客基本在海外、你自己也不常登后台的话，DMIT 的洛杉矶 T1 系列就够用：V2C2G 是 2 核 2GB / 40GB SSD / 5TB 月流量 / 10Gbps 带宽，**$14.90/月**。真想为 CN2 GIA 多付钱，先想清楚这笔钱买的是哪一段体验——人在国内、天天登后台改产品图调页面，Pro 和 EB 的回程线路让这些操作不卡；访客在海外，走的是国际段，T1 覆盖得住。

下面把三条产品线的差别、洛杉矶和香港的全套餐价格、机房怎么对应访客位置、三个最容易多花钱的地方、退款与流量限制，以及从下单到 WordPress 上线的卡点一次讲完。价格来自第三方在 2026 年 4 月对官网的整理，DMIT 调价和库存变动频繁，下单前以结算页显示为准。

## 选购速览

> - **纯海外访客、预算优先**：LAX T1 V2C2G，$14.90/月，2 核 2GB / 40GB / 5TB 流量 / 10Gbps
> - **国内要频繁登后台**：LAX EB Pocket，$159.98/年（约 $13.33/月），2 核 2GB / 40GB / 3TB 流量 / 4Gbps
> - **要最低延迟**：香港 Pro，$39.90/月起，但入门是 1 核 1GB，建站偏紧
>
> 👉 [查看 LAX T1 V2C2G 当前价格与库存](https://www.dmit.io/aff.php?aff=9081&pid=169)

## 三条产品线，一句话分清

**Pro（Premium）**：电信、联通、移动三网回程全走 CN2 GIA，晚高峰最稳，同配置里最贵。

**EB（Eyeball）**：联通走 AS9929、移动走 CMIN2，线路等级比 Pro 低一档，价格基本持平或略低。

**T1（Tier 1）**：国际优化线路，不做中国大陆方向的专项优化，价格最低，圣何塞的 T1 还带 20Gbps DDoS 防御。

全系 KVM 虚拟化，给完整 root 权限，能跑 Docker，原生 IP。DMIT 是自有机房资源的上游服务商，不是从别人那里批发线路再转卖。成立年份第三方资料说法不一（2017 与 2018 两种），官网没有公开确认，这一点对选套餐没有影响。

## 洛杉矶全套餐价格

### LAX Premium / Pro（AN4 平台，三网 CN2 GIA）

| 套餐 | CPU / 内存 / 硬盘 | 月流量 / 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- |
| TINY | 1核 / 2GB / 20GB SSD | 1000GB / 1Gbps | $88.88/年 | [选 TINY](https://www.dmit.io/aff.php?aff=9081&pid=237) |
| Pocket | 2核 / 2GB / 40GB SSD | 1500GB / 4Gbps | $159.98/年 | [选 Pocket](https://www.dmit.io/aff.php?aff=9081&pid=238) |
| STARTER | 2核 / 2GB / 80GB SSD | 3000GB / 10Gbps | $29.90/月 | [选 STARTER](https://www.dmit.io/aff.php?aff=9081&pid=239) |
| MINI | 4核 / 4GB / 80GB SSD | 5000GB / 10Gbps | $58.88/月 | [选 MINI](https://www.dmit.io/aff.php?aff=9081&pid=240) |
| MICRO | 4核 / 4GB / 160GB SSD | 7000GB / 10Gbps | $74.99/月 | [选 MICRO](https://www.dmit.io/aff.php?aff=9081&pid=241) |
| MEDIUM | 6核 / 8GB / 160GB SSD | 15000GB / 10Gbps | $168.88/月 | [选 MEDIUM](https://www.dmit.io/aff.php?aff=9081&pid=242) |
| LARGE | 8核 / 16GB / 320GB SSD | 25000GB / 10Gbps | $338.88/月 | [选 LARGE](https://www.dmit.io/aff.php?aff=9081&pid=243) |
| GIANT | 12核 / 24GB / 640GB SSD | 50000GB / 10Gbps | $619.99/月 | [选 GIANT](https://www.dmit.io/aff.php?aff=9081&pid=244) |

TINY 年付折算约 $7.41/月，是这条线里最便宜的入场方式；往上到 STARTER 换成月付后单月 $29.90，配置翻到 2 核 2GB / 80GB / 3TB / 10Gbps。

### LAX Eyeball（AS9929 + CMIN2）

| 套餐 | CPU / 内存 / 硬盘 | 月流量 / 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- |
| TINY | 1核 / 2GB / 20GB SSD | 1500GB / 2Gbps | $88.88/年 | [选 EB TINY](https://www.dmit.io/aff.php?aff=9081&pid=245) |
| Pocket | 2核 / 2GB / 40GB SSD | 3000GB / 4Gbps | $159.98/年 | [选 EB Pocket](https://www.dmit.io/aff.php?aff=9081&pid=246) |
| STARTER | 2核 / 2GB / 80GB SSD | 5000GB / 10Gbps | $29.90/月 | [选 EB STARTER](https://www.dmit.io/aff.php?aff=9081&pid=247) |
| MINI | 4核 / 4GB / 80GB SSD | 10000GB / 10Gbps | $58.88/月 | [选 EB MINI](https://www.dmit.io/aff.php?aff=9081&pid=248) |
| MICRO | 4核 / 4GB / 160GB SSD | 14000GB / 10Gbps | $74.99/月 | [选 EB MICRO](https://www.dmit.io/aff.php?aff=9081&pid=249) |
| MEDIUM | 6核 / 8GB / 160GB SSD | 30000GB / 10Gbps | $168.88/月 | [选 EB MEDIUM](https://www.dmit.io/aff.php?aff=9081&pid=250) |
| LARGE | 8核 / 16GB / 320GB SSD | 50000GB / 10Gbps | $338.88/月 | [选 EB LARGE](https://www.dmit.io/aff.php?aff=9081&pid=251) |
| GIANT | 12核 / 24GB / 640GB SSD | 100000GB / 10Gbps | $619.99/月 | [选 EB GIANT](https://www.dmit.io/aff.php?aff=9081&pid=252) |

从 Pocket 这一档往上，EB 的月流量是 Pro 的两倍，价格一模一样。

### LAX Tier 1（国际线路，外贸站重点）

| 套餐 | CPU / 内存 / 硬盘 | 月流量 / 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- |
| V2C2G | 2核 / 2GB / 40GB SSD | 5000GB / 10Gbps | $14.90/月 | [选 V2C2G](https://www.dmit.io/aff.php?aff=9081&pid=169) |
| V2C4G | 2核 / 4GB / 80GB SSD | 10000GB / 10Gbps | $23.90/月 | [选 V2C4G](https://www.dmit.io/aff.php?aff=9081&pid=170) |
| V4C4G | 4核 / 4GB / 120GB SSD | 20000GB / 10Gbps | $36.90/月 | [选 V4C4G](https://www.dmit.io/aff.php?aff=9081&pid=171) |
| V4C8G | 4核 / 8GB / 160GB SSD | 40000GB / 10Gbps | $52.90/月 | [选 V4C8G](https://www.dmit.io/aff.php?aff=9081&pid=180) |
| V8C16G | 8核 / 16GB / 240GB SSD | 80000GB / 10Gbps | $119.90/月 | [选 V8C16G](https://www.dmit.io/aff.php?aff=9081&pid=172) |
| V12C24G | 12核 / 24GB / 320GB SSD | 160000GB / 10Gbps | $199.90/月 | [选 V12C24G](https://www.dmit.io/aff.php?aff=9081&pid=173) |

T1 的入门配置（2 核 2GB）比 Pro 和 EB 的 TINY 还高，流量 5TB 是 Pro TINY 的五倍，价格 $14.90/月。资料没有给出 T1 的年付价，不能假设年付有折扣，$14.90 × 12 = $178.80/年 是按目前的月付价估算的结果。

## 新平台、香港与东京套餐

| 系列 / 套餐 | CPU / 内存 / 硬盘 | 月流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- |
| AN5 Pro TINY | 1核 / 2GB / 20GB | 1TB | $119.99/年 | [选 AN5 TINY](https://www.dmit.io/aff.php?aff=9081&pid=100) |
| AN5 Pro Pocket | 2核 / 2GB / 40GB | 1.5TB | $203.90/年 | [选 AN5 Pocket](https://www.dmit.io/aff.php?aff=9081&pid=137) |
| AN5 Pro STARTER | 2核 / 2GB / 80GB | 3TB | $38.90/月 | [选 AN5 STARTER](https://www.dmit.io/aff.php?aff=9081&pid=56) |
| HKG Pro TINY | 1核 / 1GB / 20GB | 500GB | $39.90/月 | [选 HKG Pro TINY](https://www.dmit.io/aff.php?aff=9081&pid=152) |
| HKG Pro TINYv2 | 1核 / 1GB / 20GB | 500GB | 年付 $233.91 | [选 HKG Pro TINYv2](https://www.dmit.io/aff.php?aff=9081&pid=181) |
| HKG EB TINYv2 | 1核 / 1GB / 20GB | 1TB | $29.90/月 | [选 HKG EB TINYv2](https://www.dmit.io/aff.php?aff=9081&pid=188) |
| HKG T1 WEE | 1核 / 1GB / 20GB | 1TB | $36.9/年 | [选 HKG T1 WEE](https://www.dmit.io/aff.php?aff=9081&pid=164) |
| TYO T1 TINY | 1核 / 1GB / 20GB | 1TB | $36.9/年 | [选 TYO T1 TINY](https://www.dmit.io/aff.php?aff=9081&pid=224) |

AN5 是 AMD EPYC 9005 平台，官网标价整体比 AN4 高一截。香港 Pro TINYv2 年付 $233.91 折算约 $19.49/月，比月付 TINY 的 $39.90 便宜一半，代价是带宽从 1Gbps 降到 500Mbps。

官网还有圣何塞 SJC 和洛杉矶 Premium Secure（LAX.sPro，去程走 Cloudflare Magic Transit，带 5Tbps+ 国际共享 DDoS 防御）两个系列，资料里没有可核验的完整价目，这里不列数字，需要的直接看官网当前页面。

## 机房怎么选：访客在哪，服务器就靠近哪

| 机房 | 线路 | 到大陆延迟（第三方参考） | 适合场景 |
| --- | --- | --- | --- |
| 香港 HKG | CN2 GIA / CMI | 约 20–50ms | 国内用户为主、延迟敏感 |
| 东京 TYO | CN2 GIA / CMI | 80–120ms | 日本 IP、亚太业务 |
| 洛杉矶 LAX | CN2 GIA / CMIN2 | 约 150–200ms | 中外兼顾、外贸站 |
| 圣何塞 SJC | Tier 1 + 20Gbps DDoS | 180–220ms | 海外用户、需要防御 |

这张表里的延迟数字，衡量的是**大陆到机房**这一段。外贸站的访客在欧美，这个数字对访客没有意义，只对你自己在国内登后台、传图、调页面的操作速度有意义。访客在美国，服务器放洛杉矶，走的是美西到美国各地的短路径；服务器放香港，美国访客要跨太平洋绕回来，反而更慢。

所以外贸站的机房判断只有一条：**主要客群在哪，机房就放哪。** 客群集中在美国和欧洲，洛杉矶是默认选项；客群在日本和东南亚，东京更近；客群有一半在国内，才需要把延迟表当回事。

有位第三方作者在测评里写过他自己的使用情况：洛杉矶 Premium 线路，国内白天访问基本在 150ms 以内，晚高峰偶尔到 180ms 左右。这是他个人体验，不是本文实测，只作为参考值看。

## 外贸站最容易买错的三个地方

### 一、Pro TINY 和 EB TINY 同价，配置相同，流量差一半

两个都是 $88.88/年，都是 1 核 2GB / 20GB SSD。EB TINY 给 1500GB 月流量和 2Gbps 带宽，Pro TINY 只有 1000GB 和 1Gbps。价差为零，差的是回程：Pro 三网全走 CN2 GIA，EB 是联通 AS9929 加移动 CMIN2。

访客在海外，这两条回程线路对访客都没有影响，那 EB TINY 就是更划算的那个，同样的钱多拿 50% 流量和翻倍带宽。你自己在国内天天登后台，Pro 的回程更稳，这笔钱才算花到了地方。

Pocket 档同理：Pro Pocket 和 EB Pocket 都是 $159.98/年，配置都是 2 核 2GB / 40GB / 4Gbps，EB 的流量是 3000GB，Pro 是 1500GB。

👉 [对比 EB Pocket 与 Pro Pocket 的实时报价](https://www.dmit.io/aff.php?aff=9081&pid=246)

### 二、AN5 比 AN4 贵 35%，买到的只是 CPU 代际

AN5 的 TINY 是 1 核 2GB / 20GB / 1TB / 1Gbps，和 AN4 的 TINY 一模一样，价格从 $88.88/年 涨到 $119.99/年，一年**多付 $31.11**，涨幅约 35%。

这 $31.11 买的是 AMD EPYC 9005 平台相对上一代的算力提升，内存、硬盘、流量、带宽一项没变。WordPress 建站在正常访问量下，瓶颈通常在 PHP 和数据库查询，换一代 CPU 感知不到。除非你跑计算密集型的任务（批量图片处理、爬虫、数据处理脚本），AN4 的 TINY 就够，把差价省下来加流量更实在。

### 三、香港入门是 1 核 1GB，不等于能直接建站

香港 Pro TINY $39.90/月、HKG EB TINYv2 $29.90/月，配置都是 1 核 1GB / 20GB。第三方给出的 WordPress 建站配置底线是 **1 核 2GB 内存 + 20GB SSD 起步**，1GB 内存跑 WordPress 加 MySQL，再挂几个插件和缓存，余量很小。

香港的低价档适合做落地节点、轻量代理、静态页面，正经跑 WooCommerce 或带插件的 WordPress，要往 2GB 内存的档位走，价格也就不是 $29.90 这个数了。想要低延迟又要 2GB 内存，先算清预算再决定。

## 会影响下单决定的几条硬规则

**退款**：购买后 3 天内、流量使用不超过 30GB，可以申请全额退款，扣除支付网关手续费；购买后 30 天内可以按剩余服务价值申请部分退款。续费订单和余额支付不在退款范围内。条款里写的是"部分退款"，不是 30 天内全额退，别记错。

**流量超限**：不停机，降速继续跑。第三方资料对降速幅度的说法不一致，有说 4Mbps 的，也有说 8Mbps 的，具体看套餐页的说明。降速后网站还能打开，但体验会明显变差，图片多的站建议选流量富余一档。

**T1 不保证中国大陆可用性**：这条写在换 IP 政策里。T1 是国际线路，不承诺大陆方向的连通质量，如果你的站有一半访客在国内，T1 不是合适的选择。

**免费换 IP**：LAX Pro 和 EB 系列支持，条件是实例购买满 7 天、距上次换 IP 满 15 天。第三方整理称超出频率收费 $5/次，2026 年初部分系列开放了后台自助换 IP，不用开工单。

**计费口径**：第三方资料对流量是单向还是双向计费说法不一致，有资料写 T1 系列单向计费（取入站和出站的最大值），也有资料写双向计费。下单前在套餐页确认一次，图片站和视频站尤其要看清。

**其他**：支持 Ubuntu、Debian、CentOS，不支持 Windows；默认 SSH 密钥登录，密钥只能下载一次；防火墙默认只开 SSH 端口，装完 Nginx 发现 80/443 不通要去后台放行；洛杉矶、香港、东京三个机房都不需要 ICP 备案；支持支付宝、微信、PayPal、信用卡。

关注缺货问题：LAX Pro 的 TINY 和 Pocket、香港 Pro 系列经常没货，看到有货再谈选哪个。

👉 [查看 DMIT 全部套餐的实时库存与价格](https://www.dmit.io/aff.php?aff=9081)

## 从下单到 WordPress 上线，会卡住的几步

1. **选套餐进结算页**，确认当前价格和库存，年付、季付、月付在同一页选。
2. **系统选 Ubuntu 22.04 LTS**，兼容性和文档最全，别选太新的版本。
3. **下载 SSH 密钥**，控制台只弹一次，丢了要重新生成。
4. **连上后装宝塔面板**，LNMP 环境一键安装约 30 分钟，PHP 选 8.0 或 8.1。
5. **后台防火墙放行 80 和 443**，这一步不做，域名解析对了也打不开。
6. **域名 A 记录指向服务器 IP**，宝塔里新建站点、绑定域名、建数据库，一键部署 WordPress。
7. **申请 Let's Encrypt 免费证书**，开启 HTTPS。
8. **装缓存和备份插件**，缓存用 W3 Total Cache 或 LiteSpeed Cache，备份用 UpdraftPlus，顺手把 BBR 开了。

## 常见问题

**外贸站用 DMIT 需要备案吗？**
不需要。洛杉矶、香港、东京三个机房都在境外，不走 ICP 备案流程。

**IP 被墙了怎么办？**
LAX Pro 和 EB 系列可以免费换 IP，条件是购买满 7 天、距上次换 IP 满 15 天。T1 系列不保证大陆可用性，也就不在这个政策覆盖范围内。

**流量用完了会直接停机吗？**
不会，降速处理，网站还能访问。降速后的具体速率各套餐不同，以套餐页为准。

**能装 Windows 吗？**
不能。只支持主流 Linux 发行版。

**T1 和 Pro 的流量计费方式一样吗？**
第三方资料说法不一致，有的写 T1 单向计费，有的写全系双向。这个差别对流量消耗影响很大，下单前在套餐页确认。

## 最后怎么定

访客只在海外、你自己也不常登后台，DMIT 不是必须的，同价位有更便宜的普通国际线路可选；一定要用，就选 LAX T1 V2C2G，$14.90/月，2 核 2GB / 5TB 流量，配置和流量都给得比同价位的 Pro TINY 多。

访客里有一部分在国内，或者你要天天登后台改东西，选 LAX EB Pocket，$159.98/年，约 $13.33/月，2 核 2GB / 3TB 流量 / 4Gbps，CMIN2 加 AS9929 的回程够用，比 Pro Pocket 同价多一倍流量。

要最低延迟、预算不设限，看香港 Pro，但记住入门是 1 核 1GB，建站要往上选档。

下单前确认两件事：目标套餐当前有没有货，结算页显示的价格和计费周期是不是你看到的那个。

👉 [按上面的规则挑一个套餐，进 DMIT 结算页确认最终价格](https://www.dmit.io/aff.php?aff=9081)
