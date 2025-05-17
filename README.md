baseline code AI CUP 2025:https://www.aicup.tw/ai-cup-2025-competition

dataset: https://tbrain.trendmicro.com.tw/Competitions/Details/39

## dataset
下在後解壓縮，train、test資料和 code 放在同一個資料夾下，第一次執行需要建立資料夾`tabular_data_train`、`tabular_data_test`，結構如下:
```
aicup/
├── train_data/
│   ├── 1.txt
│   └── ...
├── test_data/
│   ├── 1968.txt
│   └── ...
├── tabular_data_train/
├── tabular_data_test/
├── baseline.py
├── train_info.csv
├── test_info.csv
├── sample_submission.csv
├── ...
```

## baseline code

run baseline code
```
python baseline.py
```

第一次執行須執行`data_generate`，生成特徵檔案。

## false data

不確定是不是我的問題，測試集中3211的資料開根號會錯誤，所以我在baseline code中將3211的資料跳過，如果要繳交csv，須自己補上3211的資料。
