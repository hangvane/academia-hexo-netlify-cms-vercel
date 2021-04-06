---
title: Hello World
date: 2021-04-04T13:24:02.918Z
---

# hexo-netlify-cms-vercel

A templete to deploy a **Hexo** blog with **Netlify-CMS** on **Vercel**.

✔ Totally free of charge

✔ Static web pages, no rendering time

✔ Edit online, just as simple as using a dynamic CMS, supported by Netlify-CMS

✔ No local environment required, you can edit your pages on any devices, everywhere

✔ Zero coding

✔ Preview is supported by Netlify-CMS and Netlify

✔ Vercel CDN makes your pages to load quickly from anywhere in the world, including China Mainland

✔ Easy to bind to your domain, and enable SSL encrypt, supported by Vercel

# Additional improvements

- Customized 404 page

# Usage

1. Click `Use this template` to fork this repository. It can be private.

1. Modify `/source/admin/config.yml`. Change the value of `backend.repo` and `backend.base_url` to yours.

1. Go to [Github Developer applications](https://github.com/settings/developers) and create a new oauth app. The only important field is `Authorization callback URL`, input `https://<domain>/callback`, where `<domain>` is domain from step 2, also note that HTTPS is required. And then generate a new client secret.

1. Go to [**Vercel**](https://vercel.com/new) to import your repository and create a new project. Before clicking `Deploy` button, add the Environment Variables **`OAUTH_GITHUB_CLIENT_ID`** and **`OAUTH_GITHUB_CLIENT_SECRET`** and set the values as generated in the previous step.

1. Click `Deploy` button and waiting for the deployment finished.

1. Maybe you need to change the **Vercel** provided domain in *Settings > Domains*.

1. Open **`https://<domain>/admin/`** and login to the **Netlify-CMS** back-end. Note that the last character `/` in the URL can not be omitted.

1. Test whether **Netlify-CMS** is working properly.

1. If you need the preview feature provided by **Netlify-CMS**, that is, provides you a preview link on the article writing page once you click `save` button, you also need to link your blog repository to [**Netlify**](https://app.netlify.com/start). This is similar to link to **Vercel**, but you do not need to add Environment Variables since you do not use **Netlify-CMS** on the **Netlify** provided domain.

1. Congratulations! You have successfully deployed a **Hexo** blog with **Netlify-CMS** on **Vercel**.


# Thanks

The oauth gateway for Netlify CMS is implemented by [ublabs/netlify-cms-oauth](https://github.com/ublabs/netlify-cms-oauth).
