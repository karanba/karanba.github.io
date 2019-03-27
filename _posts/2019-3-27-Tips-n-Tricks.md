---
layout: post
title: Hızlı Bilgiler, İpuçları ve Kullanım örnekleri
categories: [General]
tags: [node, vscode]
level: Başlangıç
lang: tr
blog: yes
--- 

Çeşitli araçlar ve ortamlar için hızlı başvuru kaynağı oluşturabilecek bilgiler.

## Node & Npm

### npm run komutuna ek argüman geçmek için _--_
~~~ bash
npm run build -- --watch
~~~

### npm paketinin anasayfasını ve repository sayfasını açmak için
~~~ bash
# goes to https://angularjs.org/
npm home angular

# goes to https://github.com/angular/angular.js
npm repo angular
~~~

## VS Code

### Open with VS Code from command line

~~~

# open current directory or given path
code . or path

# open with last active instance
code <file_name> -r 

# open a file at a line number
code -g <file_name>:<line>:<column?>
    
~~~
