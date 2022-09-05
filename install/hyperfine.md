# Hyperfine 使用
hyperfine 使用需要注意需要测试的相关命令是否都安装完毕，

例如测试几个包管理命令速度，使用以下命令
``` bash
hyperfine "bun install --backend=hardlink" "yarn install --no-scripts" "npm install --no-scripts --ignore-scripts" "pnpm install --ignore-scripts" --prepare="rm -rf node_modules" --cleanup="rm -rf node_modules" --warmup=8
```
如果没有安装yarn工具的话就会报以下错误

``` bash
Benchmark 2: yarn install --no-scripts
Error: Command terminated with non-zero exit code: 1. Use the '-i'/'--ignore-failure' option if you want to ignore this. Alternatively, use the '--show-output' option to debug what went wrong.
```