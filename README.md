## yidash（易大师）一万个JavaScript实用方法库

`警告⚠️`：未发布 **v2.0.0** 之前，均为不稳定版本，慎用！！！

![logo](https://static.yicode.tech/logo/yidash-logo.png)

## 🏠 官网

[文档官网 https://yidash.dev](https://yidash.dev)

## 🛖 仓库

[github https://github.com/chenbimo/yidash](https://github.com/chenbimo/yidash)

## 🧊 安装

```bash
npm install yidash
# 或
pnpm add yidash
```

## 🍼 使用

`注意⚠️`：本项目暂时只提供 `ESM` 包。

```javascript
import { yd_tree_array2Tree, yd_regexp_trainNumber, yd_number_validNumber } from 'yidash';
console.dir(
    yd_tree_array2Tree([
        { id: 1, pid: 0 },
        { id: 2, pid: 1 },
        { id: 3, pid: 2 }
    ])
);
console.dir(yd_regexp_trainNumber);
const validNumber = yd_number_validNumber();
console.log(validNumber(1.111)); // 1.11
console.log(validNumber(1.571333)); // 1.57
console.log(validNumber('1..221333')); // 1.57
console.log(validNumber('1.2213.33')); // 1.57
console.log(validNumber('1.')); // 1.
console.log(validNumber('1.2')); // 1.20
console.log(validNumber('1.2.')); // 1.20
```

## 🎁 贡献和福利

### **贡献者交流群**

加笔者微信 `chensuiyime`，注明 `yidash` ，拉你进微信交流群。

群内将解答关于代码贡献相关的问题。

### **代码贡献步骤**

1. 访问本仓库。
2. fork本仓库。
3. 拉取fork后的仓库。
4. 修改代码。
5. push代码。
6. 发起pull request。
7. 等待笔者验证与合并。

**注意**：只提交lib中的函数到本仓库合并即可，其他文件不要提交。

### **不能这样做**

1. 不能引入很多包，需要导包的函数要与我沟通确认，尽量不依赖第三方包。
2. 不能写很复杂的函数，不能超过500行，要小而美。
3. 每个文件的作者，一经提交，其他人后续修改也不能改其原作者。

### **必须这么做**

1. 必须写JSDoc注释和使用案例，不然别人看不懂，不知道怎么用。
2. 必须写明函数作者，具体参考JSDoc文档。
3. 必须4格缩进，不喜欢的请不要参与本项目。
4. 必须按照如下格式写清楚提交信息。
5. 必须一个函数一个文件。

### **没有这些玩意**

1. 没有 `TypeScript`。
2. 没有 `Eslint`。

### **函数开发规则**

文件名必须是 `yd_[类型]_函数名`，`yd` 是 `yidash` 的缩写。

比如`yd_is_number`，`is` 表示判断，`number` 表示数字，这是一个判断数字的函数。

函数名必须具名导出，不能使用 `default` 默认导出，而且要跟文件名一致。

能用 `const` 的地方，必须用 `const`。

### **代码提交格式**

`提交主题: 提交具体内容`

举例：

-   `完善功能: yd_is_number函数增加判断机制`
-   `代码重构: yd_number_thousands重新设计`
-   `新增函数: 增加yd_is_array函数`

### **贡献者福利**

1. 增加开源参与度。
2. 体会开源的乐趣。
3. 为自己的职业经历增加一个彩蛋。
4. 函数会进行署名，你将被每一个使用yidash的人看到。
5. 额外获得VSCode扩展fnMap永久注册码一枚。
