## Alist白天/黑夜主题模板 | Alist Day/Night Theme Template

说明：本主题为带有**日夜切换**的主题模板，适用于**Alist>=3.31**。

Info: This is an Alist Nay/Night Theme Template for **Alist>=3.31** .

## 使用方法 | Usage

打开alist-header.html,编辑以下内容，将四个引号内的.png换成你的图片连接。

Open alist-header.html and edit it, make sure .png links in thr quote replaced with your own link to the image.

```html
.hope-ui-light {
    background-image:url("白天图片横屏|Daythemehorizontal.png") !important;
    @media (max-aspect-ratio:1) {
        background-image:url("白天图片竖屏|Daythemevertical.png") !important;
    }
    background-repeat:no-repeat;
    background-size:cover;
    background-attachment:fixed;
    background-position-x:center
}
.hope-ui-dark {
     background-image:url("黑夜图片横屏|Nightthemehorizontal.png") !important;
    @media (max-aspect-ratio:1) {
        background-image:url("黑夜图片竖屏|Nightthemevertical.png") !important;
    }
    background-repeat:no-repeat;
    background-size:cover;
    background-attachment:fixed;
    background-position-x:center
}
```

然后打开Alist，登录管理员账号并进入管理页面。依次点击：` 三 > 设置 > 全局 ` 将修改后内容全选，复制粘贴到 **自定义头部** 中。

Then open Alist, enter manage page and click by the following order: `三 > Settings > Global` .Now select thr whole modified file content and copy and paste it into  **Customize head** .

点击 **保存** ，大功告成！

Click on the  **Save**  button and everything is done!

日夜切换按钮可以**单独引用** 。

Day/Night switch button is available for **standalone** usage.

```html
<!--日夜切换按钮单独使用 | Standalone usage for day/night switch button-->
<script>
    function daynightswitch() {
        if (document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-icHSmvX-css")[0]) {
            document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-icHSmvX-css")[0].$$click();

        } else {
            if (document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[1]) {
                if (document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[7]) {
                    document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[7].$$click();
                } else { document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[1].$$click(); }
                document.getElementsByClassName("hope-drawer__content-container hope-c-gLUHnt hope-c-fxrEBZ hope-c-fxrEBZ-llmmsr-placement-right hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].style.display = 'None';
                document.getElementsByClassName("hope-drawer__overlay hope-c-ctSAUo hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].style.display = 'None';
                document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-icHSmvX-css")[0].$$click();
                document.getElementsByClassName("hope-modal__close-button hope-c-gYVOHl hope-close-button hope-c-iNeqtt hope-c-iNeqtt-feqEsd-size-md hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].click();
            } else {
                document.getElementsByClassName("toolbar-toggle hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[0].$$click();
                if (document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[9]) {
                    document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[9].$$click();
                } else { document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[1].$$click(); }
                document.getElementsByClassName("hope-drawer__content-container hope-c-gLUHnt hope-c-fxrEBZ hope-c-fxrEBZ-llmmsr-placement-right hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].style.display = 'None';
                document.getElementsByClassName("hope-drawer__overlay hope-c-ctSAUo hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].style.display = 'None';
                document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-icHSmvX-css")[0].$$click();
                document.getElementsByClassName("hope-modal__close-button hope-c-gYVOHl hope-close-button hope-c-iNeqtt hope-c-iNeqtt-feqEsd-size-md hope-c-PJLV hope-c-PJLV-ijhzIfm-css")[0].click();
                if (document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[8]) {
                    document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[8].$$click();
                } else { document.getElementsByClassName("hope-icon hope-c-XNyZK hope-c-PJLV hope-c-PJLV-ifkxHPo-css")[2].$$click(); }
            }
        }
        location.reload();
    }
    document.write(`<button
    class="hope-menu__trigger hope-c-bvjbhC hope-c-PJLV hope-c-PJLV-ieTGfmR-css hope-icon-button hope-button hope-c-ivMHWx hope-c-ivMHWx-kcPQpq-variant-subtle hope-c-ivMHWx-cEknLI-size-lg hope-c-ivMHWx-dvmlqS-cv hope-c-ivMHWx-hZistB-cv hope-c-PJLV hope-c-PJLV-iikaotv-css"
    type="button" role="button" id="hope-menu-daynight-switch-trigger" aria-label="switch layout"><svg t="1733225100292"
        class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="4397"
        xmlns:xlink="http://www.w3.org/1999/xlink" width="1em" height="1em">
        <path
            d="M512 0c282.7776 0 512 229.2224 512 512s-229.2224 512-512 512S0 794.7776 0 512 229.2224 0 512 0z m0 51.2a460.8 460.8 0 0 0-13.568 921.3952L512 972.8v-256a204.8 204.8 0 1 0 0-409.6V51.2z m0 256v409.6a204.8 204.8 0 1 1 0-409.6z"
            fill="currentColor" p-id="4398"></path>
    </svg></button>`)
    document.getElementById("hope-menu-daynight-switch-trigger").addEventListener("click", daynightswitch);
</script>
```
