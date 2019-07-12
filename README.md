# ts-for-node
安装

    npm i -g typescript

编译
    
    tsc app.ts

初始化：

    tsc --init

生成了tsconfig.json文件，

解开以下配置：

    "outDir": "./dist", <br>
    "rootDir": "./src", <br>
    "moduleResolution": "node",  <br>

创建src文件夹

    ./src/

直接运行tsc，则自动编译成/dist/app.js文件

    npm init -y
    npm i express

在现有项目安装ts

    npm i -D typescript ts-node nodemon @types/node @types/express<br>

package.json中的script 添加以下命令：

    "scripts": {
    "start": "node dist/app.js",
    "dev": "nodemon src/app.ts",
    "build": "tsc -p ."
     },
 
 开发时，
        
    npm run dev
 
 开发后，
    
    npm run build
