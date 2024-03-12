# vue-admin-template

English | [简体中文](./README-zh.md)

> A minimal vue admin template with Element UI & axios & iconfont & permission control & lint

**Live demo:** http://panjiachen.github.io/vue-admin-template


**The current version is `v4.0+` build on `vue-cli`. If you want to use the old version , you can switch branch to [tag/3.11.0](https://github.com/PanJiaChen/vue-admin-template/tree/tag/3.11.0), it does not rely on `vue-cli`**

<p align="center">
  <b>SPONSORED BY</b>
</p>
<p align="center">
   <a href="https://finclip.com?from=vue_element" title="FinClip" target="_blank">
      <img height="200px" src="https://gitee.com/panjiachen/gitee-cdn/raw/master/vue%E8%B5%9E%E5%8A%A9.png" title="FinClip">
   </a>
</p>

## Build Setup

```bash
# clone the project
git clone https://github.com/PanJiaChen/vue-admin-template.git

# enter the project directory
cd vue-admin-template

# install dependency
npm install

# develop
npm run dev
```

This will automatically open http://localhost:9528

## Build

```bash
# build for test environment
npm run build:stage

# build for production environment
npm run build:prod
```

## Advanced

```bash
# preview the release environment effect
npm run preview

# preview the release environment effect + static resource analysis
npm run preview -- --report

# code format check
npm run lint

# code format check and auto fix
npm run lint -- --fix
```

Refer to [Documentation](https://panjiachen.github.io/vue-element-admin-site/guide/essentials/deploy.html) for more information

## Demo

![demo](https://github.com/PanJiaChen/PanJiaChen.github.io/blob/master/images/demo.gif)

## Extra

If you want router permission && generate menu by user roles , you can use this branch [permission-control](https://github.com/PanJiaChen/vue-admin-template/tree/permission-control)

For `typescript` version, you can use [vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template) (Credits: [@Armour](https://github.com/Armour))

## Related Project

- [vue-element-admin](https://github.com/PanJiaChen/vue-element-admin)

- [electron-vue-admin](https://github.com/PanJiaChen/electron-vue-admin)

- [vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template)

- [awesome-project](https://github.com/PanJiaChen/vue-element-admin/issues/2312)

## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

## License

[MIT](https://github.com/PanJiaChen/vue-admin-template/blob/master/LICENSE) license.

Copyright (c) 2017-present PanJiaChen



这是我们的git操作流程 ，你看看是否理解，有觉得不对的地方可以提出来：

如果某个需求是几个人合作开发，一般有个领头人，由领头人从dev新建一个此次开发用的中心分支，比如haier2021_contactus_core_210513， 
（git checkout dev > git pull > git checkout -b haier2021_contactus_core_210513 > git push) 

然后参与这次开发的每个人从这个中心分支haier2021_contactus_core_210513新建自己的分支，然后进行页面制作。 
（git checkout haier2021_contactus_core_210513 > git pull > git checkout -b sunyonghua_contactus_210513 > git push） 

当在本地开发完要更测试环境时，切到test分支，先拉取test最新代码，再将自己的分支合到test分支，如果有冲突，先在test分支解决完冲突再push。 
(git checkout test > git pull > git merge sunyonghua_contactus_210513 > git push) 

当测试环境没问题，可以更到中心分支上时，切换到中心分支haier2021_contactus_core_210513，拉取最新的代码，再切回自己的分支，将中心分支haier2021_contactus_core_210513合到自己的分支 ，如果有冲突，在自己分支解决冲突，解决完之后，再切回中心分支，将自己分支代码合到中心分支haier2021_contactus_core_210513。 
(git checkout haier2021_contactus_core_210513 > git pull > git checkout sunyonghua_contactus_210513 > git merge haier2021_contactus_core_210513 > git push > git checkout haier2021_contactus_core_210513 > git merge sunyonghua_contactus_210513 > git push) 

当项目经理说可以更到生产环境时，由领头人将dev分支最新代码合到中心分支haier2021_contactus_core_210513，如果有冲突，先在中心分支解决冲突，再push。 
(git checkout dev > git pull > git checkout haier2021_contactus_core_210513 > git pull > git merge dev > git push) 

然后领头人在gitlab上将中心分支haier2021_contactus_core_210513提合并请求，提到dev分支，由项目经理进行合并，合到dev后，项目经理再将dev合到master，更到生产环境。 



如果某个需求只有自己一个人开发，和上面类似，可以直接从dev分支新建自己的分支。 
(git checkout dev > git pull > git checkout -b sunyonghua_contactus_210513 > git push) 

当在本地开发完要更测试环境时，切到test分支，先拉取test最新代码，再将自己的分支合到test分支，如果有冲突，先在test分支解决完冲突再push。 
(git checkout test > git pull > git merge sunyonghua_contactus_210513 > git push) 

当测试环境没问题，项目经理说可以更到生产环境时，先将dev分支最新代码合到自己的分支，如果有冲突，先在自己的分支解决冲突，再push。 
(git checkout dev > git pull > git checkout sunyonghua_contactus_210513 > git merge dev > git push) 

然后在gitlab上将自己的分支sunyonghua_contactus_210513提合并请求，提到dev分支，由项目经理进行合并，合到dev后，项目经理再将dev合到master，更到生产环境。


注意：新切完一个分支时，先push到远程再改代码，这样方便改完提交代码的时候，看看都改了什么内容。每次提交之前都要看下提交的内容是否都是自己改的，不是自己改的不要提交。
重要提醒：
1、一定不要将test分支代码合到自己的开发分支上。
2、不要随便格式化代码，一定不能格式化模板里的代码，否则模板没法正常解析。