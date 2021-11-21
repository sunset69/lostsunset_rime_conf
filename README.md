# rime输入法配置

## [1] default.custom.yaml

>   -   输入框待选项个数
>   -   ctrl、shift 的切换键效果
>   -   标点符号的映射

- `menu/page_size: 5`：设置后选词个数为5

- `ascii_composer/switch_key:`：ctrl shift 切换键效果

- `punctuator/half_shape:` ：半角修改为中文标点

## [2] weasel.custom.yaml

>   -   输入框显示字体及其字号
>   -   输入框皮肤
>   -   输入框横向显示

-   `"style/color_scheme": aqua`：设置主题
-   `"style/font_face": "Microsoft YaHei" `：设置字体
-   `"style/font_point": 15 `：设置字体大小
-   `"style/horizontal": true` ：false为候选框竖排，true为候选框横排（默认垂直方向）
-   `"style/display_tray_icon": false`
-   `"style/inline_preedit": false`
-   `"style/fullscreen": false`



## [3] luna_pinyin_simp.custom.yaml

>   自定义输入法（luna_pinyin_simp改为使用的输入法）

### 1）特殊符号快速输入

```yaml
patch:
  "punctuator/import_preset" : symbols
  "recognizer/patterns/punct": "^/([A-Z|a-z]*|[0-9]|10)$"
```

通过 `/` 键配合缩写实现快速输入。注意使用键盘的 `?` 键唤起，而不是小键盘的 `/` 键。

-   输入 `/xl` 直接给出希腊字母，如 *α* 等。
-   输入 `/sx` 直接给出常用数学符号，如 ±, ÷ 等。
-   输入 `/jh` 直接给出一些特殊符号，如 ■，□，?，? 等。

## 参考

极速入门配置：https://www.jianshu.com/p/46fb3049e322

sirls:http://sirlis.cn/rime-shift-switch-zh-en/
