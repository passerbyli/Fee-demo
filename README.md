## 目录结构
sass目录
├── 404.scss (使用率非常低的可以独立出来，页面单独引用，不合并)
├── auth.scss
├── components 基础模块样式（能提取出公共组件的放到components里。）
│   ├── actionsheet.scss
│   ├── badge.scss
│   ├── button.scss
│   ├── cell.scss
│   ├── dialog.scss
│   ├── footer.scss
│   ├── form.scss
│   ├── grids.scss
│   ├── header.scss
│   ├── icon.scss
│   ├── list.scss
│   ├── navbar.scss
│   ├── tab.scss
│   ├── tabbar.scss
│   └── table.scss
├── main.scss
├── pages （独立页面的样式放到pages里。）
│   └── home.scss
└── utils 基础样式
    ├── functions.scss
    ├── iconfont.scss
    ├── mixins.scss
    ├── public.scss
    ├── reset.scss
    └── variables.scss  设置变量。包括颜色边距大小

同理Js文件也如此。
对于angular
├── app.js  入口文件
├── base.js
├── common 所有公共组件及模版文件
│   ├── common.module.js
│   ├── components
│   │   └── toastr
│   │       ├── toastr.html
│   │       └── toastr.js
│   ├── directives
│   │   ├── errSrc.directive.js
│   │   ├── ngBack.directive.js
│   │   └── other.directive.js
│   ├── message
│   │   ├── message.ctrl.js
│   │   └── message.directive.js
│   └── views
│       └── tabs.html
└── pages  以模块功能建立目录并且可以继续拆分模块文件夹
    ├── cart
    │   ├── addCartArea.html
    │   ├── cart.ctrl.js
    │   ├── cart.directive.js
    │   ├── cart.html
    │   ├── cart.module.js
    │   ├── cart.service.js
    │   ├── changeCartCount.html
    │   └── history_tpl.html
    ├── order
    │   ├── order.ctrl.js
    │   ├── order.directive.js
    │   ├── order.module.js
    │   ├── order.service.js
    │   └── views
    │       ├── alert-pakg.html
    │       ├── order-address.html
    │       ├── order-cancel.html
    │       ├── order-consignee-edit.html
    │       ├── order-edit.html
    │       ├── order-error.html
    │       ├── order-goods.html
    │       ├── order-invoice.html
    │       ├── order-jump.html
    │       ├── order-ok.html
    │       ├── order-payment.html
    │       └── ordermain.html
    └── page.module.js


所有的css和js文件路径是通过gulp来替换到html的。