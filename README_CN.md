# Im-Select-Imm

## 介紹

原版im-select可以切換輸入法， 但是不能切換中英文。
這個版本可以在第二個參數中切換中英文和全形半形。

## 使用方式

### 下載

### 取得當前輸入法的key

```shell
/path/to/im-select-imm.exe
Out: [當前輸入法]-[輸入法的當前模式]
```

### 切換輸入法

```shell
/path/to/im-select.exe [目標輸入法]  
Or
/path/to/im-select.exe [目標輸入法] [目標輸入法的目標模式]
Or
/path/to/im-select.exe [目標輸入法]-[目標輸入法的目標模式] # 部分外掛下只允許一個參數
Or
/path/to/im-select.exe -d 50 [目標輸入法]-[目標輸入法的目標模式] # 在切換輸入法和模式之間插入延遲，預設30ms，可能可以改善一部分人無效的情況
```
## 已測試輸入法

1. 新舊微軟拼音
2. 新微軟日語輸入法

### 對於微軟輸入法

```
For  Microsoft Old Chinese IME(Win10 and Previous) :
    0: English
    1: Chinese
For  Microsoft New Chinese IME(Win11) :
    0: English / Half Shape
    1: Chinese / Half Shape
    1024: English / Full Shape (雖然存在此模式，但實際仍然為半形)
    1025: Chinese / Full Shape
```
