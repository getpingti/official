# getpingti.com 新官网 · 企业官网改版服务

getpingti.com 转型后的主站：小企业官网改版服务（品牌主张「官网平替」——600 元/站，先做演示站，满意再付款）。

纯静态站：`index.html`（首页）、`service.html`（服务与价格）、`cases.html`（改版案例）、`faq.html`（常见问题）、`contact.html`（联系我们），共用 `style.css`，无框架、无 CDN、无后端。联系表单通过 mailto 拼装，不接任何接口。

## 部署映射

| 路径 | 内容 | 说明 |
|---|---|---|
| 本仓库（`getpingti/official`） | getpingti.com 主站 | 部署到 Cloudflare Pages，绑定主域名 **getpingti.com** |
| `/demo/<客户>/` | 客户改版演示站 | 现内置 `demo/case-wood/`（青岛龙山木工机械，16 页）与 `demo/case-dust/`（泊头市科惠除尘，18 页）；演示页全部带 `noindex` meta，确认期 10–15 天，到期下线对应目录即可 |
| https://software.getpingti.com | 原「开源软件平替」资源站 | 独立仓库 **getpingti/site**，在本站作为「软件平替」栏目外链存在；本站页脚已注明两站同属一个团队运营 |

## 素材来源

- 首页 Hero 与内页横幅背景图 `assets/img_hero.jpg`：案例企业泊头市科惠除尘原站自有实拍（除尘工程现场全景图，2 倍放大锐化版），随其演示站（`demo/case-dust/`）一并采集，特此注明来源为案例站实拍。
- `assets/longshan-machine.jpg`：青岛龙山木工机械原站实拍（气动拼板机），随其演示站一并采集。
- 案例页的全部问题数据（龙山 19 张产品图失效、新闻停在 2013 年；科惠 viewport 实测 0 处、首页 44 处强制新开窗口、新闻停在 2020 年、改版 18 页 51 个产品）来自两家演示站的改版说明 NOTES，与演示站内容一致。

## 待办

- 联系邮箱 `hello@getpingti.com` 目前为占位，域名邮箱开通后即可收信；开通前请勿对外发送本站链接邀约。
- 正式部署时在 Cloudflare Pages 将本仓库设为生产分支直连，演示目录随主站一同发布。
