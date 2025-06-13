# zako.work

[![PRs](https://img.shields.io/github/issues-pr-closed-raw/MuskaNet/zako.work.svg?style=flat-square&colorB=FF69B4&label=pull%20requests)](https://github.com/MuskaNet/zako.work/pulls?q=is%3Apr+is%3Aclosed+label%3Aadd)
[![Contributors](https://img.shields.io/github/contributors-anon/MuskaNet/zako.work.svg?color=228B22&style=flat-square)](https://github.com/MuskaNet/zako.work/graphs/contributors)

简体中文 | [English](./README.md)

## 子域名申请

为了申请你的 `zako.work` 子域名，请跟随以下步骤：

1. 在 `zako/` 目录下创建一个文件，命名为 `<维护者名称>-ZAKO`。请注意，请使用对文件使用**英文全大写**命名。
    - 写入如下内容：

      ```plaintext
      zako:   <维护者名称>
      site:   <你的网站链接> # 可选的
      remark: <注释>        # 如果你希望添加多个注释，只需要换行并以 `remark:` 开头即可。
      ```

2. 在 `subdomain/` 目录下创建一个文件，命名为 `<子域名>.zako.work`。

> [!IMPORTANT]  
> 如果可以，请添加 NS 记录而不是其他记录，否则在更新时，您需要重新开一个 PR 到本仓库，将会很麻烦且费时。

    - 写入如下内容：

      ```plaintext
      domain: <子域名>.zako.work
      zako:   <维护者>
      a:      <IP>               # 符合规范的 DNS 记录。您可以创建诸如 `a` `cname` `ns` 之类的记录，请创建拉取请求以获取更新，我们将帮助您同步。
      ```

4. 创建一个拉取请求到我们的仓库。

这个时候目录应该是这样的：

```plaintext
subdomain/
  <子域名>.zako.work
zako/
  <维护者名称>-ZAKO
......
```
