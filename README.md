This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.



# 安装nvm、nodejs 
https://help.aliyun.com/zh/ecs/use-cases/deploy-a-node-js-environment-on-a-centos-7-instance

解决nvm ls-remote 列表只出现iojs版本
https://blog.csdn.net/Guzarish/article/details/141372073

nvm install v20.18.0

default.conf
server {
  listen 80;
  server_name todokit.xyz aliyun.todokit.xyz;
  return 301 https://omb.todokit.xyz;
}

cat dokki.fans.conf
server{
  listen 80;
  server_name  dokki.fans;

  location / {
    proxy_pass http://localhost:3000;
  }
}

npm install pm2 -g
在Linux阿里云服务器上部署Nextjs项目
https://juejin.cn/post/6993205190471974925
在自己服务器上部署nextjs项目
https://juejin.cn/post/7173498085958483998