---
title: Contributing
---

We welcome you to join the development of Hexo. ๐ค

## ๊ฐ๋ฐ

์ฐ๋ฆฌ๋ ๋น์ ์ด Hexo์ ๊ฐ๋ฐ์ ์ฐธ์ฌํ๋ ๊ฒ์ ํ์ํฉ๋๋ค. ์ด ๋ฌธ์๋ ๋น์ ์ ๊ฐ๋ฐ ํ๋ก์ธ์ค์ ๋์์ ์ค ๊ฒ๋๋ค.

### ์์ํ๊ธฐ ์ ์...

Please read [Contributor Covenant Code of Conduct](https://github.com/hexojs/hexo/blob/master/CODE_OF_CONDUCT.md) first.

์๋์ ์ฝ๋ฉ ์คํ์ผ์ ์ง์ผ์ฃผ์ธ์.

- [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)๋ฅผ ๋ฐ๋ฆ๋๋ค.
- ๋ ๊ฐ์ ๊ณต๋ฐฑ์ ์ฌ์ฉํ soft-tab์ ์ฌ์ฉํฉ๋๋ค.
- ์ฝค๋ง๋ก ์์ํ์ง ๋ง์ธ์.

Also, Hexo has its own [ESLint config](https://github.com/hexojs/eslint-config-hexo), so please make sure your contribution will make ESLint happy.

### ์ํฌํ๋ก์ฐ

1. Fork [hexojs/hexo].
2. ์ ์ฅ์๋ฅผ ๋น์ ์ ์ปดํจํฐ์ cloneํ๊ณ  ์์กด ์ฌํญ๋ค์ ์ค์นํฉ๋๋ค.

``` bash
$ git clone https://github.com/<username>/hexo.git
$ cd hexo
$ npm install
$ git submodule update --init
```

3. ๊ธฐ๋ฅ branch๋ฅผ ์์ฑํฉ๋๋ค.

``` bash
$ git checkout -b new_feature
```

4. ๊ฐ๋ฐํฉ๋๋ค.
5. Branch๋ฅผ pushํฉ๋๋ค.

```
$ git push origin new_feature
```

6. ๋ณ๊ฒฝ์ฌํญ์ ๋ํ ์ค๋ช์ ํฌํจํ์ฌ Pull request๋ฅผ ์์ฑํฉ๋๋ค.

### ๊ณต์ง์ฌํญ

- `package.json`์ version number๋ ์์ ํ์ง ๋ง์ธ์.
- ๋น์ ์ Pull request๋ ํ์คํธ๋ฅผ ํต๊ณผํ์ ๋์๋ง merge๋ฉ๋๋ค. ๋ฐ์ํ๊ธฐ ์ ์ test๋ฅผ ๋๋ ค๋ณด์ธ์.

``` bash
$ npm test
```

## Updating official-plugins

Also, we welcome PR or issue to [official-plugins](https://github.com/hexojs). ๐ค

## ๋ฌธ์์ ๊ฐฑ์ 

Hexo ๋ฌธ์๋ opensource์ด๋ฉฐ [hexojs/site]์์ ์์ค ์ฝ๋๋ฅผ ๊ฒ์ํ  ์ ์์ต๋๋ค.

### Workflow

1. Fork [hexojs/site]
2. ์ ์ฅ์๋ฅผ ๋น์ ์ ์ปดํจํฐ์ cloneํ๊ณ  ์์กด ์ฌํญ๋ค์ ์ค์นํฉ๋๋ค.

``` bash
$ npm install hexo-cli -g # If you don't have hexo-cli installed
$ git clone https://github.com/<username>/site.git
$ cd site
$ npm install
```

3. ๋ฌธ์๋ฅผ ์์ ํ์ธ์. Server๋ฅผ ๋๋ ค์ ์ค์๊ฐ์ผ๋ก ํ์ธํ  ์ ์์ต๋๋ค.

``` bash
$ hexo server
```

4. Branch๋ฅผ pushํฉ๋๋ค.
5. ๋น์ ์ ๋ณ๊ฒฝ์ฌํญ์ ๋ํ ์ค๋ช์ ํฌํจํ์ฌ Pull request๋ฅผ ์์ฑํฉ๋๋ค.

### ๋ฒ์ญ

1. `source` ํด๋ ์์ ์ ์ธ์ด์ ๋ํ ํด๋๋ฅผ ์์ฑํ์ธ์. (์๋ฌธ์๋ก ์์ฑํ์ธ์.)
2. `source` ํด๋์ Markdown ๋ฐ ํํ๋ฆฟ ํ์ผ๋ค์ ์ ์ธ์ด ํด๋์ ๋ณต์ฌํ์ธ์.
3. `source/_data/language.yml`์ ์ ์ธ์ด๋ฅผ ์ถ๊ฐํ์ธ์.
4. `themes/navy/languages`์ `en.yml` ํ์ผ์ ๋ณต์ฌํ๊ณ  ์ ์ธ์ด๋ก ์ด๋ฆ์ ๋ณ๊ฒฝํ์ธ์. (์๋ฌธ์๋ก ๋ณ๊ฒฝํ์ธ์.)

## ์ด์ ๋ณด๊ณ 

Hexo๋ฅผ ์ฌ์ฉํ๋ค๊ฐ ๋ฌธ์ ๋ฅผ ๋ฐ๊ฒฌํ๋ฉด, [Troubleshooting](troubleshooting.html), [GitHub](https://github.com/hexojs/hexo/issues), [Google Group](https://groups.google.com/group/hexo)์์ ์ด์์ ๋ํด ๋ต์ ์ฐพ์๋ณด์ธ์. ๋ง์ฝ ๋ต์ด ์๋ค๋ฉด Github์ ๋ฌธ์ ๋ฅผ ๋ณด๊ณ ํด ์ฃผ์ธ์.

1. ๋ฌธ์  ์ฌํ์ [debug mode](commands.html#Debug_mode)์์ ํด์ฃผ์ธ์.
2. Follow the steps from issue template to provide debug message and version when submitting a new issue at GitHub.

[hexojs/hexo]: https://github.com/hexojs/hexo
[hexojs/site]: https://github.com/hexojs/site
