# Grok3 PlayGround 
# Grok3 2.0 游乐场

### 作者：技术爬爬虾
[B站](https://space.bilibili.com/316183842)，[Youtube](https://www.youtube.com/@Tech_Shrimp)，抖音，公众号 全网同名。转载请注明作者。

## 项目简介
#### Demo: [https://ubiquitous-lolly-397934.netlify.app/](https://ubiquitous-lolly-397934.netlify.app/)
10秒部署一个Grok3国内镜像网站，支持多账户聚合，单账户额度不够可秒换账号。
不限地区/网络环境，打开即用，<b>适配了手机端</b>。
使用Netlify/Deno/Cloudflare Worker无服务器免费部署。


## Netlify部署 [推荐]
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/tech-shrimp/grok-playground)
点击部署按钮，登录Github账户即可

## Deno部署

1. [fork](https://github.com/tech-shrimp/grok-playground/fork)本项目
2. 登录/注册 https://dash.deno.com/
3. 创建项目 https://dash.deno.com/new_project
4. 选择此项目，填写项目名字（请仔细填写项目名字，关系到自动分配的域名）
5. Entrypoint 填写 `src/deno_index.ts` 其他字段留空 
   <details>
   <summary>如图</summary>
   ![image](/docs/images/1.png)
   </details>
6. 点击 <b>Deploy Project</b>
7. 部署成功后获得域名，点开即用。

## Cloudflare Worker 部署
[![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/tech-shrimp/grok-playground)

1. 点击部署按钮
2. 登录Cloudflare账号
3. 填入Account ID，与API Token
4. Fork本项目，开启Github Action功能
5. 部署，打开dash.cloudflare.com，查看部署后的worker
6. 需要开梯子使用


#### 有用的话帮忙B站或者Youtube点个关注~
[https://space.bilibili.com/316183842](https://space.bilibili.com/316183842)<br>
[https://www.youtube.com/@Tech_Shrimp](https://www.youtube.com/@Tech_Shrimp)

## 本地调试（Deno）

Windows 安装Deno:
> irm https://deno.land/install.ps1 | iex

Mac/Linux 安装Deno:
> curl -fsSL https://deno.land/install.sh | sh

启动项目：

>cd 项目目录 <br>
>deno run start


## 本地调试（Netlify）

1. 安装NodeJs
2. npm install -g netlify-cli
3. cd 项目根目录
4. netlify login
5. netlify dev
