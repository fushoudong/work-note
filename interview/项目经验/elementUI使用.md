# element-ui

## 1. 现有组件

### 1. el-backtop

> el-backtop官网上存在一些问题，在使用时需要注意以下几点
>
> 1. el-backtop的直接父元素需要设置css属性中的overflow与height，设置如下：
> 2. 在使用时使用target属性指向父类的选择器(class注意.)

1. 样式

   ```css
   // 设置的css
   .scroll-backtop {
   	overflow: hidden;
       height: '100px'/*  固定高度 */
   }
   ```

2. 使用

   ```vue
   <div class="scroll-backtop">
       <el-backtop target=".scroll-backtop"></el-backtop>
   </div>
   ```

   

