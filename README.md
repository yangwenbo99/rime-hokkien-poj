Type Hokkien (Taiwanese) Han-ji using POJ (Pe̍h-Ōe-Ji, Church Romanisation).  This is a patch to [A-Thok's project](https://github.com/a-thok/rime-hokkien). 

用白話字（教會羅馬字）拍閩南語（福建話/台語）正字文。這是一例對阿托項目兮覆翅 (phak-chhì)。

For the Chinese version of the README file, please see `README.zh.md`. 

中文版本佇咧 `README.zh.md`。


## Setup

Put files in the `poj_patches/` directory, together with the files from [A-Thok's repository](https://github.com/a-thok/rime-hokkien) into your RIME configuration directory, i.e. 
-  `~/.config/ibus/rime/` or `~/.config/fcitx/rime/` on Linux, 
- `%APPDATA%\Rime` on Windows, or
- `~/Library/Rime/` on Mac OS. 


### Linux

You need to add a line under `schema_list:` in `default.custom.yaml`: 

```yaml
patch:
    schema_list:
      - schema: blg_ha_rime
      ...
```

The selected IM can be `blg_ha_poj`, `blg_chiang_poj`, `blg_choan_poj` and `blg_tai_poj`. 


### MS Windows

Activate the input method through your RIME GUI configuration tool. 

## Key bindings

- o͘: press `w` or `oo`
- ⁿ: press `v` or `nn`
- You can use the following shorthand: 
    - z for ch
    - q for chh
    - f for ph
    - d for th
    - x for kh
    - y for the i at the end of a syllabus
- Press `` ` `` (shift + the key on the left-hand-side of `1`) for reverse lookup through "Hanyu Pinyin". 


## Todos

I am only familiar with Amoy Hokkien, so the formulas, especially the comment formats for the reverse lookups, for other dialects are not fully checked



## Technical details

We attempt to modify vowels involving `r` to its counterpart in POJ by using the most common pronunciation without `r`, which is partially based the Amoy pronunciation.  The letter `r` is preserved in Changchow, Chinchew and Taiwan when typing in, but all `r` and `ee` are removed for reverse lookup. 
