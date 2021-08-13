# Nodejs 16 for replit.com
How to use nodejs 16 on replit.

## Instruction
#### 1. Open shell mode
#### 2. Execute this command
```sh
npm init -y && npm i --save-dev node@16 && npm config set prefix=$(pwd)/node_modules/node && export PATH=$(pwd)/node_modules/node/bin:$PATH
```
##### Note you can change the node version to any version you want just replace 16 with the version you want.
#### 3. Create [.replit](https://docs.repl.it/repls/dot-replit) file to make the commands run from the shell not console.
```
run = "npm start"
```
#### 4. In your package.json file add this code.
```json
"scripts": {
    "start": "node ."
}
```
#### Optional. If you have an installed package before re-install the package Ex:
```
npm uninstall pkg-name && npm i pkg-name
```

## الخطوات
#### 1. افتح وضع الـ Shell
#### 2. حط الامر ذا
```sh
npm init -y && npm i --save-dev node@16 && npm config set prefix=$(pwd)/node_modules/node && export PATH=$(pwd)/node_modules/node/bin:$PATH
```
##### ملحوظة تقدر تغير اصدار النود عن طريق تغيير رقم 16 الموجود بالامر
#### 3. سوي ملف [.replit](https://docs.repl.it/repls/dot-replit) عشان نخلي ريبل ات يشغل المشروع من الShell وليس الكونسول
```
run = "npm start"
```
#### 4. في ملف الpackage.json حط ذا الكود
```json
"scripts": {
    "start": "node ."
}
```
#### اختياري. لو عندك بكج مثبت قبل كذا امسحه وارجع نزله
```
npm uninstall pkg-name && npm i pkg-name
```
