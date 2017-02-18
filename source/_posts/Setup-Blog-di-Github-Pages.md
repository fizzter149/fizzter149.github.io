---
title: Setup Blog di Github Pages
date: 2017-02-18 01:09:31
tags: [blog, github]
categories: uncategorized
---

Langkah mudah setup blog pribadi di github pages. Blog engine yang digunakan adalah [Hexo](https://hexo.io), walaupun pada dasarnya github pages bisa digunakan untuk serve static website.

<!-- more -->

# Yang dibutuhkan
1. Git
2. Node

# Langkah-langkah

## di [github](https://github.com):
1. buat repo `<nama-blog>.github.io`
2. catat url repo

## di console:

1. Install cli untuk blog engine [Hexo](https://hexo.io)
```sh
npm install -g hexo-cli
```

2. Buat project blog baru
```
hexo init new-blog
cd new-blog
```

3. Sesuaikan pengaturan
```
vi _config.yml
```
    contoh, untuk deploy:
```yaml
deploy:
 type: git
 repo: <url repo github yang sudah dicatat sebelumnya>
```

4. Untuk deploy:
```sh
hexo deploy
```

# selesai

`https://<nama-blog>.github.io` is up!

Selain [Hexo](https://hexo.io), ada banyak alternatif blogging engine, contohnya jekyll.
