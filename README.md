## 开发环境安装

### 依赖

- jruby 9.1.7.0 (be compatible with Ruby 2.3.x)，参考 [www.ruby-lang.org](https://www.ruby-lang.org/) 和 [jruby.org](http://jruby.org/)

### 步骤

- 用 `jruby -S bundle install` 安装依赖

## 部署

- 执行 `bundle exec rake war:executable war`，在根目录生成 `jruby-test.war`
- 启动 jetty server，命令是

```bash
$ java -jar jruby-test.war
# access in http://#{IP address}:8080
```
