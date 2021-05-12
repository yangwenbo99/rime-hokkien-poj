## 準備使用

佮 `im` 這例目錄當中兮物件契入去汝兮 RIME 設定目錄：
- Linux: `~/.config/ibus/rime/` 或者 `~/.config/fcitx/rime/`
- Windows: `%APPDATA%\Rime`
- MaxOS: `~/Library/Rime/`


### Linux

佇咧 `default.custom.yaml` 後壁加一行，若像是按呢： 

```yaml
patch:
    schema_list:
      - schema: blg_ha_rime
      ...
```

汝會用兮對 `blg_ha_poj`、`blg_chiang_poj`、`blg_choan_poj`佮`blg_tai_poj`當中選。 


### MS Windows

對汝兮 RIME GUI 設定當中激活。

## 按鍵綁定
- o͘: 揤 `w` 或者 `oo`
- ⁿ: 揤 `v` 或者 `nn`
- 汝也是會用兮用徙落來齊兮短手： 
    - 拍 z 出 ch
    - 拍 q 出 chh
    - 拍 f 出 ph
    - 拍 d 出 th
    - 拍 x 出 kh
    - 佇音節尾拍 y 出 i
- 揤  `` ` `` （shift + `1` 倒爿彼粒按鍵）就有法通對「漢語拼音」倒查白話字。 


## Todos

我只是會曉講廈門話，所以無法通完全檢查其他方言兮推導公式，特別是遐 comment formats。


## 技術細節

一過音素佇白話字當中無，但是佇兮臺羅當中有，比如講 `r` 佮 `ee`。佇廈門話 IM 當中，阮將 `r` 佮 `ee` 全部提走。但是汝照原有法通佇兮漳州話、泉州話佮台灣台語兮 IM 當中用 `r` 佮 `ee`，但是怹就袂去佇兮倒查結果當中出現。
