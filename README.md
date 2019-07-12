# ts-for-node
安装

  npm i -g typescript
  
编译

  tsc app.ts

初始化：

tsc --init<br>

后生成tsconfig.json文件，

解开

"outDir": "./dist", <br>
"rootDir": "./src", <br>
"moduleResolution": "node",  <br>

创建src文件夹

./src/

直接运行tsc，则自动编译成/dist/app.js文件

npm init -y

npm i express<br>

在现有项目安装ts

npm i -D typescript ts-node nodemon @types/node @types/express<br>

package.json中的script 添加start命令：

  "scripts": {
  
    "start": "node dist/app.js",
  
    "dev": "nodemon src/app.ts",
    
    "build": "tsc -p ."
    
  },
