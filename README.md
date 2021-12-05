# ni-demo
:art: use antfn/ni

### install dep
pnpm

### use
1. ni相关会根据当前项目的锁文件，去判断应该使用什么包管理功能，若没有任意包管理器的锁文件则交互式询问
```
package.lock.json => npm
yaen.lock => yarn
pnpm-lock.yaml => pnpm
```
2. ni - install
3. nr - run
4. nx - execute
5. nu - upgrade
6. nci - clean install

### debugger mode
在命令最后加上`?`，会进入debugger模式，此时不会去执行相应命令，而是打印出该命令“解析”出来的结果
eg:
```
ni ? => pnpm install
```