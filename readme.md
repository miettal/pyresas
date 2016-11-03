#pyresas

## これはなに？
地域経済分析システム（RESAS：リーサス） API https://opendata.resas-portal.go.jp/ をpythonから使うライブラリです。

## どうやってつかうの？
1. まず、RESAS-API利用登録 https://opendata.resas-portal.go.jp/form.html に登録し、API Keyを取得する。
2. 下記のコマンドを叩く。
```sh
pip install pyresas
```

## コード例
```python
import pyresas
from pyresas.resas import RESASAPI
resas_api = '4omuCllKHK4cuzLvHPM764UZohdjk8eM1Wpl1bQj'
resas_api = RESASAPI('4omuCllKHK4cuzLvHPM764UZohdjk8eM1Wpl1bQj')
resas_api.getPrefectures()
# =>[{u'prefName': u'\u5317\u6d77\u9053', u'prefCode': 1}, {u'prefName': u'\u9752\u68ee\u770c', u'prefCode': 2}, {u'prefName': u'\u5ca9\u624b\u770c', u'prefCode': 3}, {u'prefName': u'\u5bae\u57ce\u770c', u'prefCode': 4}, {u'prefName': u'\u79cb\u7530\u770c', u'prefCode': 5}, {u'prefName': u'\u5c71\u5f62\u770c', u'prefCode': 6}, {u'prefName': u'\u798f\u5cf6\u770c', u'prefCode': 7}, {u'prefName': u'\u8328\u57ce\u770c', u'prefCode': 8}, {u'prefName': u'\u6803\u6728\u770c', u'prefCode': 9}, {u'prefName': u'\u7fa4\u99ac\u770c', u'prefCode': 10}, {u'prefName': u'\u57fc\u7389\u770c', u'prefCode': 11}, {u'prefName': u'\u5343\u8449\u770c', u'prefCode': 12}, {u'prefName': u'\u6771\u4eac\u90fd', u'prefCode': 13}, {u'prefName': u'\u795e\u5948\u5ddd\u770c', u'prefCode': 14}, {u'prefName': u'\u65b0\u6f5f\u770c', u'prefCode': 15}, {u'prefName': u'\u5bcc\u5c71\u770c', u'prefCode': 16}, {u'prefName': u'\u77f3\u5ddd\u770c', u'prefCode': 17}, {u'prefName': u'\u798f\u4e95\u770c', u'prefCode': 18}, {u'prefName': u'\u5c71\u68a8\u770c', u'prefCode': 19}, {u'prefName': u'\u9577\u91ce\u770c', u'prefCode': 20}, {u'prefName': u'\u5c90\u961c\u770c', u'prefCode': 21}, {u'prefName': u'\u9759\u5ca1\u770c', u'prefCode': 22}, {u'prefName': u'\u611b\u77e5\u770c', u'prefCode': 23}, {u'prefName': u'\u4e09\u91cd\u770c', u'prefCode': 24}, {u'prefName': u'\u6ecb\u8cc0\u770c', u'prefCode': 25}, {u'prefName': u'\u4eac\u90fd\u5e9c', u'prefCode': 26}, {u'prefName': u'\u5927\u962a\u5e9c', u'prefCode': 27}, {u'prefName': u'\u5175\u5eab\u770c', u'prefCode': 28}, {u'prefName': u'\u5948\u826f\u770c', u'prefCode': 29}, {u'prefName': u'\u548c\u6b4c\u5c71\u770c', u'prefCode': 30}, {u'prefName': u'\u9ce5\u53d6\u770c', u'prefCode': 31}, {u'prefName': u'\u5cf6\u6839\u770c', u'prefCode': 32}, {u'prefName': u'\u5ca1\u5c71\u770c', u'prefCode': 33}, {u'prefName': u'\u5e83\u5cf6\u770c', u'prefCode': 34}, {u'prefName': u'\u5c71\u53e3\u770c', u'prefCode': 35}, {u'prefName': u'\u5fb3\u5cf6\u770c', u'prefCode': 36}, {u'prefName': u'\u9999\u5ddd\u770c', u'prefCode': 37}, {u'prefName': u'\u611b\u5a9b\u770c', u'prefCode': 38}, {u'prefName': u'\u9ad8\u77e5\u770c', u'prefCode': 39}, {u'prefName': u'\u798f\u5ca1\u770c', u'prefCode': 40}, {u'prefName': u'\u4f50\u8cc0\u770c', u'prefCode': 41}, {u'prefName': u'\u9577\u5d0e\u770c', u'prefCode': 42}, {u'prefName': u'\u718a\u672c\u770c', u'prefCode': 43}, {u'prefName': u'\u5927\u5206\u770c', u'prefCode': 44}, {u'prefName': u'\u5bae\u5d0e\u770c', u'prefCode': 45}, {u'prefName': u'\u9e7f\u5150\u5cf6\u770c', u'prefCode': 46}, {u'prefName': u'\u6c96\u7e04\u770c', u'prefCode': 47}]
```
