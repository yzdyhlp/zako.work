# zako.work

[![PRs](https://img.shields.io/github/issues-pr-closed-raw/MuskaNet/zako.work.svg?style=flat-square&colorB=FF69B4&label=pull%20requests)](https://github.com/MuskaNet/zako.work/pulls?q=is%3Apr+is%3Aclosed+label%3Aadd)
[![Contributors](https://img.shields.io/github/contributors-anon/MuskaNet/zako.work.svg?color=228B22&style=flat-square)](https://github.com/MuskaNet/zako.work/graphs/contributors)

English | [简体中文](./README_zh-CN.md)

## Subdomain(s) Request

To request your subdomain(s) on `zako.work`, please following this step:

1. Create a file on `zako/`, named as `<MAINTAINER>-ZAKO`. Please use **ALL CAPITAL CAPTIONS** when naming your files.
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
      a:      <IP>                  # DNS records that conform to the specification. You can create records such as `a` `cname` `ns`, please open a pull request for updates and we will help you sync.
      ```

> [!IMPORTANT]  
> If possible, please add NS records, otherwise you need open a new PR to this repository, this is cumbersome and time-consuming.

4. Create a pull request to our repo.

At this time the directory should look like this:

```plaintext
subdomain/
  <SUBDOMAIN>.zako.work
zako/
  <MAINTAINER>-ZAKO
...
```
