# rime���뷨����

## [1] default.custom.yaml

>   -   ������ѡ�����
>   -   ctrl��shift ���л���Ч��
>   -   �����ŵ�ӳ��
>   -   ���/ȥ����ݼ�

- `menu/page_size: 5`�����ú�ѡ�ʸ���Ϊ5

- `ascii_composer/switch_key:`��ctrl shift �л���Ч��

- `punctuator/half_shape:` ������޸�Ϊ���ı��

- ȥ����ݼ�

    >   accept�����ܵĿ�ݼ�
    >
    >   noop����ʾ�޲���

    ```yaml
    key_binder:
      bindings:
        - {accept: "Control+Shift+1", select: noop, when: always}
    ```

    

## [2] weasel.custom.yaml

>   -   �������ʾ���弰���ֺ�
>   -   �����Ƥ��
>   -   ����������ʾ
>   -   �����Ĭ����/Ӣ��ģʽ

-   `"style/color_scheme": aqua`����������

-   `"style/font_face": "Microsoft YaHei" `����������

-   `"style/font_point": 15 `�����������С

-   `"style/horizontal": true` ��falseΪ��ѡ�����ţ�trueΪ��ѡ����ţ�Ĭ�ϴ�ֱ����

-   `"style/display_tray_icon": false`�����̵�ͼ��

-   `"style/inline_preedit": false`

-   `"style/fullscreen": false`

-   �����Ĭ��Ӣ��ģʽ

   ```text
   app_options/photoshop.exe:
     ascii_mode: true
   ```



## [3] luna_pinyin_simp.custom.yaml

>   �Զ������뷨��luna_pinyin_simp��Ϊʹ�õ����뷨��

### 1��������ſ�������

```yaml
patch:
  "punctuator/import_preset" : symbols
  "recognizer/patterns/punct": "^/([A-Z|a-z]*|[0-9]|10)$"
```

ͨ�� `/` �������дʵ�ֿ������롣ע��ʹ�ü��̵� `?` �����𣬶�����С���̵� `/` ����

-   ���� `/xl` ֱ�Ӹ���ϣ����ĸ���� *��* �ȡ�
-   ���� `/sx` ֱ�Ӹ���������ѧ���ţ��� ��, �� �ȡ�
-   ���� `/jh` ֱ�Ӹ���һЩ������ţ��� ��������?��? �ȡ�

## �ο�

�����������ã�https://www.jianshu.com/p/46fb3049e322

sirls:http://sirlis.cn/rime-shift-switch-zh-en/

[����һ��С�׵�rime����ָ��](https://www.zhihu.com/column/c_1176886232608600064)

