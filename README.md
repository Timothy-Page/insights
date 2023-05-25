# rtd.ditatompel.com Site

Based from starter theme template of [HB Framework](https://hbstack.dev/). live demo: https://theme.hbstack.dev/.
I install this by just following [https://hbstack.dev/en/docs/getting-started/installation/](https://hbstack.dev/en/docs/getting-started/installation/) process.

```bash
# Clone the repository
git clone --depth 1 https://github.com/hbstack/theme rtd-ditatompel-com
cd rtd-ditatompel-com
# change the module path located in go.mod, replace the module github.com/hbstack/theme with this repo : github.com/ditatompel/rtd-ditatompel-com.
sed -i -e 's/module\ github.com\/hbstack\/theme/module\ github.com\/ditatompel\/rtd-ditatompel-com/' go.mod
# push to remote repo
git add .
git commit --amend
git remote set-url origin git@github.com:ditatompel/rtd-ditatompel-com.git
git push origin main
# install build tools
npm ci
# start hugo server
npm run dev
# or 
npm run prod
```

## Documentations

| English | 简体中文 |
| ------- | -------- |
| [Prerequisites](https://hbstack.dev/en/docs/getting-started/prerequisites/) | [先决条件](https://hbstack.dev/zh-hans/docs/getting-started/prerequisites/) |
| [Installation](https://hbstack.dev/en/docs/getting-started/installation/) | [安裝](https://hbstack.dev/zh-hans/docs/getting-started/installation/) |
| [Configuration](https://hbstack.dev/en/docs/configuration/) | [配置](https://hbstack.dev/zh-hans/docs/configuration/) |
| [Content](https://hbstack.dev/en/docs/content/) | [内容](https://hbstack.dev/zh-hans/docs/content/) |
| [Deployment](https://hbstack.dev/en/docs/deployment/) | [部署](https://hbstack.dev/zh-hans/docs/deployment/) |
| [Modules](https://hbstack.dev/en/docs/modules/) | [模块](https://hbstack.dev/zh-hans/docs/modules/) |

## Features

- **Fast** and **SEO** friendly: [PageSpeed Insight](https://pagespeed.web.dev/analysis?url=https://theme.hbstack.dev/en/) scored perfect :100: in all four metrics on mobile and desktop.
- **Multi-purpose**: blog, project documentations, digital garden, gallery, landing pages and so on.
- **Responsive**: mobile first, built on top of Bootstrap v5.3.
- :ice_cube: **Modular** and **flexible**: extend features via various modules.
- :first_quarter_moon: **Dark mode**: light, dark or auto (follow system).
- :mag: **Search**: powerful client side *fuzzy* search that allows *filtering* and *sorting* of results, as well as searching from all multilingual sites.
- **PurgeCSS**: remove unused CSS.
- :rocket: **PWA**:
  - Installable: add site to home screen.
  - Offline available: offline page and offline image.
  - Allow precaching resources, such as CSS, JS and fonts.
- **Advanced**:
  - Custom SCSS [variables](https://github.com/hbstack/theme/blob/main/assets/hb/modules/custom/scss/variables.tmpl.scss) and [style](https://github.com/hbstack/theme/blob/main/assets/hb/modules/custom/scss/index.scss).
  - Custom [JavaScript](https://github.com/hbstack/theme/blob/main/assets/hb/modules/custom/js/index.ts).
  - Custom HTML markup:
    - [Before the end of `<head>`](https://github.com/hbstack/theme/blob/main/layouts/partials/hugopress/modules/hb-custom/hooks/head-end.html)
    - [Before the end of `<body>`](https://github.com/hbstack/theme/blob/main/layouts/partials/hugopress/modules/hb-custom/hooks/body-end.html)
- :framed_picture: **Images Processing**: process images via URL query string and fragment, such as alignment, resizing, cropping and so on, friendly to Markdown.
- :computer: **Code block panel**: expand toggle, code copy button, line number toggle and wrap toggle.
- **Menus**: supports header menus and footer menus.
- Related posts slide.
- :framed_picture: Image viewer: zoom in/out image.
- :card_index_dividers:	**Archives**: group by year and month.
- :memo: **Multiple authors**: articles can be co-authored.
- :globe_with_meridians: **Multilingual**.
- :arrow_left: **RTL**: supports Right-to-Left languages.
- :arrow_up: Back/Return to top button.
- Social links: supports header and footer social links.
- Content: supports KaTex (math), Mermaid (diagrams) and Bootstrap shortcodes.
- ...

## Screenshot

![Screenshot](https://raw.githubusercontent.com/hbstack/theme/main/images/screenshot.png)
