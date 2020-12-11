# TS入门

## Hello TypeScript

1. 新建一个`hello.ts`文件，代码如下：

   ```typescript
   function sayHello(person: string) {
       return 'Hello, ' + person;
   }
   let user = 'Tom';
   console.log(sayHello(user));
   ```

2. 运行时执行 `tsc hello.ts`会生成一个同名的`js`文件(即`hello.js`)，代码如下

   ```typescript
   function sayHello(person) {
       return 'Hello, ' + person;
   }
   var user = 'Tom';
   console.log(sayHello(user));
   ```

   注意：

   1. es6 语法转为es5，示例中的 let -> var
   2. **TypeScript 只会在编译时对类型进行静态检查，如果发现有错误，编译的时候就会报错**。而在运行时，与普通的 JavaScript 文件一样，不会对类型进行检查

## 安装typescript

`TypeScript`的安装命令如下

```shell
npm install typescript -g
```

以上是在全局安装了`tsc`命令，执行此命令就可以编译.ts文件

## 对TypeScript的理解

**理解：**

`TypeScript`是`JavaScript`的一个超集，主要提供**类系统**以及对**ES6**的支持

**TypeScript的优势**

1. 增强了代码的可读性以及可维护性
2. 包容性强
   - .js结尾的文件可以直接命名为.ts，即使不显示定义类型，也能够自动做出类型推论
3. 社区活跃