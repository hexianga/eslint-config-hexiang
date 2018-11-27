## eslint-config-hexiang

自己使用的 npm 包

## 发布自己的配置和发布 npm 包

## npm config get prefix

将本地开发模块链接到全局，进入自己的开发模块，执行下面的指令:

    npm link
    
`npm link` 命令可以将一个任意位置的 `npm包` 链接到全局执行环境，

此时会在下面的全局目录中建立一个软链接指向当前的 `npm` 项目。


全局的位置:

    {prefix}/lib/node_modules/<package>

获取 `prefix` 的值的指令：

    npm config get prefix

如果要使用这个本地开发的包，那么进入自己需要使用这个模块的目录下面，然后执行下面的指令：

    npm link my-test-module
    // 如此就会将本地开发的那个包链接到当前包的 node_modules 目录下面。

