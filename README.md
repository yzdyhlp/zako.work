# zako.work

English | [简体中文](./README_zh-CN.md)

## Subdomain(s) Request

To request your subdomain(s) on `zako.work`, please following this step:

1. Create a file on `zako/`, named as `<MAINTAINER>-ZAKO`.
    - write this content:

      ```plaintext
      zako:   <MAINTANER_NAME>
      site:   <YOUR_WEBSITE_URL> # This field is optional
      remark: <REMARK>           # If you wish add more than one remarks, just create a new line and write `remark:` on head.
      ```

2. Create a file on `subdomain/`, named as `<SUBDOMAIN>.zako.work`.
    - write this content:

      ```plaintext
      domain: <SUBDOMAIN>.zako.work
      zako:   <MNT_ZAKO>
      a:      <IP>                  #
      ```

3. Create a pull request to our repo.

这个时候目录应该是这样的：

```plaintext
subdomain/
  <SUBDOMAIN>.zako.work
zako/
  <MAINTAINER>-ZAKO
...
```
