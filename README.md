# zako.work

To request your subdomain(s) on `zako.work`, please following this step:

1. Create a file on `zako/`, named as `<YOURNAME>-ZAKO`.
  - write this content:
    ```
    zako: <MAINTANER_NAME>
    site: <YOUR_WEBSITE> # This field is optional
    remark: <REMARK> # If you wish add more than one remarks, just create a new line and write `remark:` on head.
    ```
2. Create a file on `subdomain`, named as `<SUBDOMAIN>.zako.work`.
  - write this content:
    ```
    domain: <SUBDOMAIN>.zako.work
    zako: <MNT_ZAKO>
    ```
3. Create a pull request to our repo.
