<div align="right">
  è¯­è¨:
  <a title="è±è¯­" href="../../README.md">ðºð¸</a>
  ð¨ð³
  <a title="ä¿è¯­" href="../ru/README.md">ð·ðº</a>
</div>

![NexT preview](https://user-images.githubusercontent.com/16272760/99784261-872d3200-2b56-11eb-807c-869042d1f6e8.png)

<a title="NexT ç½ç«" href="https://theme-next.js.org"><img align="right" alt="NexT logo" width="100" height="100" src="https://raw.githubusercontent.com/next-theme/hexo-theme-next/master/source/images/logo.svg"></a>

# NexT

> Â«NexTÂ» æ¯ä¸æ¬¾é£æ ¼ä¼éçé«è´¨é [Hexo](https://hexo.io) ä¸»é¢ï¼èªç¹ç¹æ»´æ»´ä¸­ç¨ç±éç¢èæã

[![NPM version](https://img.shields.io/npm/v/hexo-theme-next?color=red&logo=npm&style=flat-square)](https://www.npmjs.com/package/hexo-theme-next)
[![Required Hexo version](https://img.shields.io/badge/hexo-%3E=5.3.0-blue?style=flat-square&logo=hexo)](https://hexo.io)
[![License](https://img.shields.io/badge/license-%20AGPL-orange?style=flat-square&logo=gnu)](https://github.com/next-theme/hexo-theme-next/blob/master/LICENSE.md)
[![Build Status](https://img.shields.io/github/workflow/status/next-theme/hexo-theme-next/Linter?label=test&logo=github&style=flat-square)](https://github.com/next-theme/hexo-theme-next/actions?query=workflow%3ALinter)
[![Build Status](https://img.shields.io/github/workflow/status/next-theme/hexo-theme-next/Tester?logo=github&style=flat-square)](https://github.com/next-theme/hexo-theme-next/actions?query=workflow%3ATester)
[![Coverage Status](https://img.shields.io/coveralls/github/next-theme/hexo-theme-next?logo=coveralls&style=flat-square)](https://coveralls.io/github/next-theme/hexo-theme-next)
[![jsDelivr hits](https://img.shields.io/jsdelivr/npm/hm/hexo-theme-next?logo=jsdelivr&logoColor=white&style=flat-square)](https://www.jsdelivr.com/package/npm/hexo-theme-next)

## å³æ¶é¢è§

<p align="center">
  ð <a href="https://theme-next.js.org/muse/">Muse</a> | ð¯ <a href="https://theme-next.js.org/mist/">Mist</a> | âï¸ <a href="https://theme-next.js.org/pisces/">Pisces</a> | âï¸ <a href="https://theme-next.js.org">Gemini</a>
<br>
<br>
  æ´å¤ Â«NexTÂ» çä¾å­åè§<a href="https://github.com/next-theme/awesome-next#live-preview">è¿é</a>ã
</p>

## å®è£

å¦æä½ å¨ä½¿ç¨ Hexo 5.0 ææ´æ°çæ¬ï¼æç®åçå®è£æ¹å¼æ¯éè¿ npmï¼

```sh
$ cd hexo-site
$ npm install hexo-theme-next
```

ä½ ä¹å¯ä»¥ç´æ¥åéæ´ä¸ªä»åºï¼

```sh
$ cd hexo-site
$ git clone https://github.com/next-theme/hexo-theme-next themes/next
```

æ­¤å¤ï¼å¦æä½ æ³è¦ä½¿ç¨å¶ä»æ¹å¼ï¼è¯·åè§[è¯¦ç»å®è£æ­¥éª¤][docs-installation-url]ã

å®è£å®æåï¼å¨ Hexo éç½®æä»¶ä¸­å° `theme` è®¾ç½®ä¸º `next`ã

```yml
theme: next
```

## éç½®

ç®å NexT é¼å±ç¨æ·ä½¿ç¨ [Alternate Theme Config][docs-configuration-url] è¿è¡éç½®ãå¹¶ä¸å¯ä»¥è½»æ¾å°éè¿ [Custom Files][docs-custom-files-url] èªå®ä¹ä¸»é¢çå¸å±åæ ·å¼ã

ä¸æ¨èç´æ¥ä¿®æ¹ NexT ä¸»é¢çæä»¶ãå ä¸ºè¿å¯è½å¯¼è´éè¯¯ï¼ä¾å¦ git merge å²çªï¼ï¼å¹¶ä¸å¨åçº§ä¸»é¢æ¶ä¿®æ¹çæä»¶å¯è½ä¸¢å¤±ã

ç¶èä½ ä¹å¯ä»¥éè¿æäº¤ï¼`Commit`ï¼ãè´®èï¼`Stash`ï¼æå¿½è§ï¼`Discard`ï¼æ¬å°æ´æ¹ä»¥ç»è¿è¿ç§æ´æ°éè¯¯ï¼ä¾å¦ **Â«Commit your changes or stash them before you can mergeÂ»**ï¼ãå·ä½æ¹æ³è¯·åè[è¿é](https://stackoverflow.com/a/15745424/5861495)ã

## æä»¶

æä»¶ä¸°å¯åæå±äº NexT çåè½ãè¿äºæä»¶åä¸ºä¸¤ç§ï¼æ ¸å¿æä»¶åç¬¬ä¸æ¹æä»¶ãæ ¸å¿æä»¶è¢« NexT çåºç¡åè½æä¾èµãç¬¬ä¸æ¹æä»¶æä¾äºå¤§éçå¯éåè½ã

éç½®è¿äºæä»¶éå¸¸ç®åãä¾å¦ï¼ä½ æ³è¦å¨ä½ çç«ç¹ä¸­ä½¿ç¨ `pjax` æä»¶ï¼è¯·è¿å¥ NexT éç½®æä»¶ï¼å¯ç¨ `pjax` éç½®é¡¹ï¼

```yml
# Easily enable fast Ajax navigation on your website.
# For more information: https://github.com/next-theme/pjax
pjax: true
```

### è®¾ç½® CDN

ç¬¬ä¸æ¹æä»¶é»è®¤éè¿ [jsDelivr](https://www.jsdelivr.com) CDN æå¡å è½½ãæä»¬ä¹æä¾äºå¶å®ç CDN æå¡ä¾éæ©ï¼åæ¬èåç [UNPKG](https://unpkg.com) å [CDNJS](https://cdnjs.com)ã

ä¾å¦ï¼ä½ æ³è¦ä½¿ç¨ `unpkg` ä»£æ¿ `jsdelivr` ä½ä¸ºé»è®¤ç CDN æä¾åï¼ä½ éè¦å¨ NexT éç½®æä»¶ä¸­è¿è¡å¦ä¸è®¾ç½®ï¼

```yml
vendors:
  # ...
  # Some contents...
  # ...
  plugins: unpkg
```

## æ´æ°

NexT æ¯ä¸ªæé½ä¼åå¸æ°çæ¬ãè¯·å¨æ´æ°åéè¯»[æ´æ°è¯´æ][docs-release-url]ãä½ å¯ä»¥éè¿å¦ä¸å½ä»¤æ´æ° NexTã

éè¿ npm å®è£ææ°çæ¬ï¼

```sh
$ cd hexo-site
$ npm install hexo-theme-next@latest
```

æèéè¿ git æ´æ°å°ææ°ç master åæ¯ï¼

```sh
$ cd themes/next
$ git pull
```

**å¦æä½ æ³è¦ä» v5.x / v7.x æ´æ°å°ææ°çæ¬ï¼éè¯»[è¿ç¯ææ¡£][docs-upgrade-url]ã**

## åé¦

* æµè§ [Awesome NexT][awesome-next-url] åè¡¨ï¼ä¸å¶å®ç¨æ·åäº«æä»¶åæç¨ã
* å å¥æä»¬ç [GitHub discussions][discussions-url] / [Gitter][gitter-url] èå¤©ã
* è¯·è±å ç§éæ¥[æ·»å æä¿®æ­£ç¿»è¯][i18n-url]ã
* å¨ [GitHub Issues][issues-bug-url] æ¥åBugã
* å¨ [GitHub][issues-feat-url] è¯·æ±æ°çåè½ã
* ä¸º [åæ¬¢è¿ç Feature request][feat-req-vote-url] æç¥¨ã

## è´¡ç®ä½ çä»£ç 

æä»¬æ¬¢è¿ä½ å å¥ NexT çå¼åï¼è´¡ç®åºä½ çä¸ä»½åéãè¯·ç[å¼æºè´¡ç®æå][contributing-document-url]ã ð¤

ä½ ä¹å¯ä»¥éæ¶åæä»¬ç[å®æ¹æä»¶][official-plugins-url]æäº¤ Issue æ Pull Requestã

## è´¡ç®è

[![Contributors][contributors-image]][contributors-url]

## é¸£è°¢

Â«NexTÂ» ç¹å«æè°¢è¿äºæ¯ææä»¬æ ¸å¿åºç¡è®¾æ½çä¼è´¨æå¡ï¼

<a href="https://github.com"><img height="40" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png"></a>

> GitHub å®¹è®¸æä»¬æç®¡ Git ä»åºåè¿è¡æµè¯ã

<a href="https://www.netlify.com"><img height="40" src="https://www.netlify.com/img/press/logos/full-logo-light.svg"></a>

> Netlify å®¹è®¸æä»¬åå¸ææ¡£ã

<a href="https://crowdin.com"><img height="40" src="https://support.crowdin.com/assets/logos/crowdin-logo-small-black.svg"></a>

> Crowdin å®¹è®¸æä»¬æ¹ä¾¿å°ç¿»è¯ææ¡£ã

<a href="https://www.jsdelivr.com"><img height="40" src="https://raw.githubusercontent.com/jsdelivr/jsdelivr-media/master/default/svg/jsdelivr-logo-horizontal.svg"></a>

> jsDelivr æä¾äº CDN æå¡ã

[docs-installation-url]: https://theme-next.js.org/docs/getting-started/installation.html
[docs-configuration-url]: https://theme-next.js.org/docs/getting-started/configuration.html
[docs-custom-files-url]: https://theme-next.js.org/docs/advanced-settings/custom-files.html
[docs-release-url]: https://github.com/next-theme/hexo-theme-next/releases
[docs-upgrade-url]: https://theme-next.js.org/docs/getting-started/upgrade.html

[awesome-next-url]: https://github.com/next-theme/awesome-next
[discussions-url]: https://github.com/next-theme/hexo-theme-next/discussions
[gitter-url]: https://gitter.im/hexo-next
[i18n-url]: https://crowdin.com/project/hexo-theme-next

[issues-bug-url]: https://github.com/next-theme/hexo-theme-next/issues/new?assignees=&labels=Bug&template=bug-report.md
[issues-feat-url]: https://github.com/next-theme/hexo-theme-next/issues/new?assignees=&labels=Feature+Request&template=feature-request.md
[feat-req-vote-url]: https://github.com/next-theme/hexo-theme-next/issues?q=is%3Aopen+is%3Aissue+label%3A%22Feature+Request%22

[contributing-document-url]: https://github.com/next-theme/hexo-theme-next/blob/master/docs/zh-CN/CONTRIBUTING.md
[official-plugins-url]: https://github.com/next-theme
[contributors-image]: https://raw.githubusercontent.com/next-theme/contributors/master/contributors.svg
[contributors-url]: https://github.com/next-theme/hexo-theme-next/blob/master/docs/AUTHORS.md
