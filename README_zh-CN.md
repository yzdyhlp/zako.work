# zako.work

简体中文 | [English](./README.md)

## 子域名申请

为了申请你的 `zako.work` 子域名，请跟随以下步骤：

1. 在 `zako/` 目录下创建一个文件，命名为 `<维护者名称>-ZAKO`。
    - 写入如下内容：

      ```plaintext
      zako:   <维护者名称>
      site:   <你的网站链接> # 可选的
      remark: <注释>        # 如果你希望添加多个注释，只需要换行并以 `remark:` 开头即可。
      ```

2. 在 `subdomain/` 目录下创建一个文件，命名为 `<子域名>.zako.work`。
    - 写入如下内容：

      ```plaintext
      domain: <子域名>.zako.work
      zako:   <维护者>
      a:      <IP>               # DNS records that conform to the specification. You can create records such as `a` `cname` `ns`, please open a pull request for updates and we will help you sync.
      ```

3. 创建一个拉取请求到我们的仓库。

这个时候目录应该是这样的：

```plaintext
subdomain/
  <子域名>.zako.work
zako/
  <维护者名称>-ZAKO
......
```
