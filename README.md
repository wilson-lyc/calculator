# Calculator

一个仿照 Windows 计算器制作的桌面项目，基于 Java 8、JavaFX 和 FXML 开发，使用 Maven 管理。

## 主要功能

- 基础运算：加减乘除、小数输入、正负号切换、退格和清空。
- 历史回溯：查看计算记录，并恢复先前的计算结果；记录仅在本次运行期间保留。
- 异常处理：对除零、结果未定义、输入长度超限等情况提供提示，并在数值过大或过小时提示精度风险。

## 启动运行

准备包含 JavaFX 的 JDK 8 和 Maven。当前项目未配置独立的 JavaFX 依赖，使用更高版本 JDK 需要额外配置。

### IntelliJ IDEA

以 Maven 项目打开根目录，将项目 SDK 和运行配置的 JRE 设置为上述 JDK 8，运行 `src/main/java/MainApplication.java` 的 `main` 方法。

### 命令行

将 `JAVA_HOME` 指向上述 JDK 8，确认 `mvn -version` 使用该 JDK，然后在项目根目录执行：

```sh
mvn compile
"$JAVA_HOME/bin/java" -cp target/classes MainApplication
```

