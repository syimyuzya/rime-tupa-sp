# RIME 切韻拼音三拼輸入方案

基於 [RIME 切韻拼音輸入方案](https://github.com/nk2028/rime-tupa)，用固定三鍵打出一字。

__注意__：本輸入方案目前為 beta 版，設計已基本敲定，並經過測試。歡迎反饋使用體驗～

[安裝方式](#installation)見文末。

![Screenshot](screenshot.png)

### 反查功能

與 RIME 拼韻拼音輸入法相仿，可按 <kbd>\`</kbd> 然後鍵入漢語拼音，或按 <kbd>~</kbd> 然後鍵入粵拼來反查切韻拼音。

## 鍵位表

此為簡表，具體說明及鍵位排佈邏輯（亦是記憶方法）在後文，建議先閱讀一遍。

![Layout](layout.png)

其中[標為「-*」的韻尾鍵用法可點此預先了解](#special-final)。

## 聲母

25 鍵：

- 端知章組（含日母，不含書船母）同鍵
- 精莊組同鍵

### 鍵位

| 左五         | 左四        | 左三         | 左二          | 左一        | 右一         | 右二         | 右三         | 右四         | 右五        |
| ------------ | ----------- | ------------ | ------------- | ----------- | ------------ | ------------ | ------------ | ------------ | ----------- |
| 影 q<br />Q  | 云 ∅<br />W | 影 q<br />E  | 清 tsh<br />R | 端 t<br />T | 透 th<br />Y | 疑 ng<br />U | 溪 kh<br />I | 滂 ph<br />O | 幫 p<br />P |
| 從 dz<br />A | 心 s<br />S | 定 d<br />D  | 精 ts<br />F  | 羣 g<br />G | 曉 h<br />H  | 以 j<br />J  | 見 k<br />K  | 來 l<br />L  |             |
| 邪 z<br />Z  | 匣 x<br />X | 船 zj<br />C | 書 sj<br />V  | 並 b<br />B | 泥 n<br />N  | 明 m<br />M  |              |              |             |

如何記憶鍵位：

- 拼音為單字母的聲母，與字母鍵一致（惟影母除 Q 外亦可用 E）
- 滂在幫之左 (O)、透在端之右 (Y)、溪在見之上 (I)
- 疑在溪之左 (U)
- 云在 W、匣在 X
- 從在 A 與心邪均相鄰
- 精在 F、清在精之上 (R)
- 書在 V、船在書之左 (C)

## 韻尾、四聲

25 鍵

- -∅ 平上去、-ng/k 平上去入（7 鍵）
- -j、-n/t（7 鍵）
- -w、-m/p（7 鍵）
- -*（平上去入 4 鍵）

寫為「-*」的四個鍵為特殊韻尾鍵，和特定元音鍵形成固定組合（詳見後面元音表）。

### 鍵位

| 左五                 | 左四                | 左三                 | 左二                  | 左一                  | 右一                | 右二                | 右三               | 右四                 | 右五                 |
| -------------------- | ------------------- | -------------------- | --------------------- | --------------------- | ------------------- | ------------------- | ------------------ | -------------------- | -------------------- |
| <br />Q              | N入<br />-t<br />W  | N平<br />-n<br />E   | N上<br />-nq<br />R   | N去<br />-nh<br />T   | J去<br />-jh<br />Y | J上<br />-jq<br />U | J平<br />-j<br />I | \*上<br />-*q<br />O | \*去<br />-*h<br />P |
| \*平<br />-*<br />A  | NG入<br />-k<br />S | NG平<br />-ng<br />D | NG上<br />-ngq<br />F | NG去<br />-ngh<br />G | ∅去<br />-∅h<br />H | ∅上<br />-∅q<br />J | ∅平<br />-∅<br />K | W平<br />-w<br />L   |                      |
| \*入<br />-*k<br />Z | M入<br />-p<br />X  | M平<br />-m<br />C   | M上<br />-mq<br />V   | M去<br />-mh<br />B   | W去<br />-wh<br />N | W上<br />-wq<br />M |                    |                      |                      |

```
Q    W E R T       Y U I    O P
     入平上去<n  j>去上平 *>上去
A    S D F G       H J K    L
平<* 入平上去<ng 0>去上平 w>平
Z    X C V B       N M
入<* 入平上去<m  w>去上
```

如何記憶鍵位：

- 三排對應韻尾三類，左手陽聲韻，右手陰聲韻（惟 -w 尾平聲挪至旁邊中排 L 鍵）
- 「-*」尾四鍵均在邊緣

## 元音

26 鍵

| 三A<br />章、精           | 三B或知組<br />知、莊          | 三C<br />章、精          | 一四等<br />端、精      | 二等<br />知（端併入）、莊 |
| ------------------------- | ------------------------------ | ------------------------ | ----------------------- | -------------------------- |
|                           |                                | ya<br />接 -*: 知莊-yang | a                       | ae                         |
|                           |                                | ua                       | wa                      | wae                        |
| ie<br />接 -ng/*: iae(ng) | ye (知-ie)<br />接 -ng: yaeng  |                          | e                       | ee                         |
| wie<br />接 -ng: wiaeng   | ue (知-wie)<br />接 -ng: uaeng |                          | we                      | wee                        |
|                           |                                | yo<br />接 -*: 知莊-yo   | eo<br />接 -*: weong    | oeu                        |
|                           |                                | uo<br />接 -*: 知莊-uo   | o<br />接 -*: 知莊-uong |                            |
| i                         | yi (知-i)<br />接 -*: 知莊-yng | y<br />接 -*: 知莊-y     |                         |                            |
| wi                        | ui (知-wi)                     | u<br />接 -*: 知莊-u     | ou<br />接 -*: 知莊-ung |                            |

- iae、yae、wiae、uae 併入 ie、ye、wie、ue，靠 -ng 尾區分（麻三則用 -* 尾區分）
- 「端知章」「精莊」鍵，拼三AC兩欄時默認為章、精，拼三B一欄時默認為知、莊，但通過「-*」韻尾鍵可改變搭配

### 「-*」尾用法

1. 調整聲母搭配：
   - 主要的 3C 元音 yo/uo/y/u 後接 -* 時為 -∅ 尾，並由原先拼章精組改為拼知莊組
   - ya 後接 -* 時為 -ng 尾，並改拼知莊組
2. 調整等第及聲母搭配
   - 通攝 ung、uong 欲拼知莊組，用對應的一等元音 ou、o 接 -* 尾
   - 蒸韻 yng 欲拼知莊組，用對應的B類元音 yi 接 -* 尾
3. 調整個別元音：
   - 麻三 iae 為 ie 接 -* 尾，與清開 iaeng 為 ie 接 -ng 平行
   - 登合 weong 為 eo 接 -* 尾


### <a name="special-final"></a>如何掌握「-*」尾用法？

上一節所述「-*」尾用法<b>並不需要硬記！</b>只需要以下三條處理原則就可以對着鍵位表<b>立即開始打字</b>，並在實際使用中漸漸熟悉其用法：

1. 章精變知莊
2. 通曾攝用鄰元音
3. 麻三、登合直接記

具體來說：

1. __章精變知莊__：想打「知」「莊」組聲母卻打出「章」「精」組，說明此處可能就是「-\*」尾派上用場的時候！如果想打的元音是央後元音（y/u、yo/uo、ya/ua），就換用「-\*」韻尾鍵試試吧！（當然，前元音 (w)i、(w)i(a)e 就只需換用B類 ui、u(a)e 的鍵位，即可切換聲母，不用換韻尾）
   - 例：初學三拼時想試着打「張」tryang，敲 t-ya-ng (<kbd>T</kbd>-<kbd>A</kbd>-<kbd>D</kbd>) 發現打出的是「章」tjyang，且 ya 不是前元音，那麼改打 t-ya-* (<kbd>T</kbd>-<kbd>A</kbd>-<kbd>A</kbd>) 就能成功打出「張」
   - 例二：想打「事」dzryh，敲 dz-y-h (<kbd>A</kbd>-<kbd>R</kbd>-<kbd>H</kbd>) 發現打出的是「字」dzyh，且 y 不是前元音，改打 dz-y-*h (<kbd>A</kbd>-<kbd>R</kbd>-<kbd>P</kbd>) 就能成功打出「事」
2. __通曾攝用鄰元音__：打「知」「莊」組 -ng 尾三等字，照着上一條做，卻打出了不帶韻尾的字，說明除了韻尾鍵用「-*」外，還需要換用與其接近的相鄰元音鍵（鍵盤上也是相鄰的），這種情況只在通、曾兩攝三等韻出現，只有三個：ung 用 ou 鍵、uong 用 o 鍵、yng 用 yi 鍵就可以了！
   - 例：初學三拼想打「中」trung，敲 t-u-ng (<kbd>T</kbd>-<kbd>F</kbd>-<kbd>D</kbd>) 發現打出的是「終」tjung，改用「-\*」尾打 t-u-* (<kbd>T</kbd>-<kbd>F</kbd>-<kbd>A</kbd>) 發現打出的是「啁」tru 沒有 -ng 尾，那麼再改打鄰元音 t-ou-* (<kbd>T</kbd>-<kbd>G</kbd>-<kbd>A</kbd>) 就能成功打出「中」
   - 例二：想打「懲」dryng，敲 d-y-ng (<kbd>D</kbd>-<kbd>R</kbd>-<kbd>D</kbd>) 發現打出的是「承」djyng，改用「-\*」尾打 d-y-* (<kbd>D</kbd>-<kbd>R</kbd>-<kbd>A</kbd>) 發現打出的是「持」dry 沒有 -ng 尾，那麼再改打鄰元音 d-yi-* (<kbd>D</kbd>-<kbd>E</kbd>-<kbd>A</kbd>) 就能成功打出「懲」
3. __麻三、登合直接記__：最後就只剩下麻三 iae 用 ie-\*，以及登合 weong 用 eo-\* 這兩個特別組合了，請直接記住就好。

### 特殊處理

- 「地」dih 單獨編碼為「d-i-jh」，以區別於「視」（常母，d-i-∅h）（其他此類端組字不特殊編碼）
- 「𩦠」biangq 元音 ia 按 ya 來輸入
- 「怎」tsoymq（精開一侵上）該音是後起音，不在切韻音系中，其主元音 oy（表示「一等的 y 元音」）寄於最不常用的 ui 鍵，編碼為「ts-ui-mq」

### 鍵位

| 左五      | 左四       | 左三      | 左二      | 左一       | 右一       | 右二      | 右三      | 右四       | 右五      |
| --------- | ---------- | --------- | --------- | ---------- | ---------- | --------- | --------- | ---------- | --------- |
| ui<br />Q | wi<br />W  | yi<br />E | y<br />R  | wa<br />T  | we<br />Y  | yo<br />U | ye<br />I | wie<br />O | ue<br />P |
| ya<br />A | a<br />S   | i<br />D  | u<br />F  | ou<br />G  | o<br />H   | uo<br />J | ie<br />K | e<br />L   |           |
| ua<br />Z | wee<br />X | ee<br />C | ae<br />V | wae<br />B | oeu<br />N | eo<br />M |           |            |           |

如何記憶鍵位：

- 左手中排食指為 u，其正上為對應的開口 y，其右為對應的一等 ou
  - 右手對稱，中排食指為 uo，其上為開口 yo，其左為一等 o；此外其正下為 o 所對應的開口 eo
- 左手中排中指為 i，其正上開始往左分別為 yi、wi、ui
  - 右手對稱，中排中指為 ie，其正上開始往右分別為 ye, wie, ue
- 左手中排無名指為 a，其合口 wa 在食指右上
  - 右手對稱，中排無名指為 e，其合口 we 在食指左上
  - 左手小指（即 a 左邊）為 ya，合口 ua 在其下
- 二等元音在下排連續五鍵

## <a name="installation"></a>安裝

### Windows

1. 參見[切韻拼音輸入法 Windows 安裝方法](https://github.com/nk2028/rime-tupa#windows-%E5%AE%89%E8%A3%9D%E6%96%B9%E6%B3%95)

2. 在第二步鍵入 `nk2028/rime-tupa` 按 <kbd>Enter</kbd> 後，再額外鍵入 `syimyuzya/rime-tupa-sp` <kbd>Enter</kbd>，然後再繼續第三步。

   ※ 如果之前已經安裝過切韻拼音，則在跳出的視窗僅鍵入 `syimyuzya/rime-tupa-sp` <kbd>Enter</kbd> 即可。

3. 在第三步勾選輸入法時，額外勾選「切韻拼音·三拼」。

### macOS

1. 參見[切韻拼音輸入法 macOS 安裝方法](https://github.com/nk2028/rime-tupa#macos-%E5%AE%89%E8%A3%9D%E6%96%B9%E6%B3%95)

2. 在第二步後，再額外複製粘貼以下命令：

   ```sh
   curl -fsSL https://git.io/rime-install | bash -s -- syimyuzya/rime-tupa-sp custom:set:config=default,key=installed_from,value=syimyuzya/rime-tupa-sp custom:clear_schema_list custom:add:schema=tupa custom:add:schema=tupa_sp custom:add:schema=luna_pinyin custom:add:schema=jyut6ping3
   ```

   ※ 如果之前已安裝切韻拼音，則只須複製粘貼上述命令即可。

3. 之後繼續第三步，選取輸入法。

### Arch Linux

1. 參見[切韻拼音輸入法 Arch Linux 安裝方法](https://github.com/nk2028/rime-tupa#arch-linux-%E5%AE%89%E8%A3%9D%E6%96%B9%E6%B3%95)

2. 第二步改為從 AUR 安裝 [`rime-tupa-sp`](https://aur.archlinux.org/packages/rime-tupa-sp)：

   ```sh
   yay -S rime-tupa-sp
   ```
   
   在建立的 `default.custom.yaml` 中額外加入一行 `- schema: tupa_sp`，效果如下：
   
   ```yaml
   patch:
   schema_list:
     - schema: tupa
     - schema: tupa_sp
   ```
   
   然後重新部署。

### 手動安裝

1. 先[安裝 RIME 輸入法及切韻拼音輸入方案](https://github.com/nk2028/rime-tupa#%E5%AE%89%E8%A3%9D)

2. 下載此處的 `tupa_sp.schema.yaml`

2. 將 `tupa_sp.schema.yaml` 放入 RIME 用戶目錄

3. 在 `default.custom.yaml` 的 `schema_list` 中仿照已有項目加入一行 `- schema: tupa_sp`，注意與已有的項目對齊（如下方代碼所示）

   若用戶目錄無該文件，則新建並貼上以下內容：

   ```yaml
   patch:
     schema_list:
       - schema: tupa
       - schema: tupa_sp
   ```

4. 重新部署後即可選擇「切韻拼音·三拼」輸入法

## 聲明

本方案（及其他類似方案）僅為基於切韻拼音所設計的便捷輸入方案，不是切韻拼音方案的一部分。此類輸入法亦非切韻拼音規範所涉及的領域，故本方案（及其他類似方案皆）不具有和切韻拼音同等的通用規範地位，亦不會作為切韻拼音的「指定配套方案」等。

PS 本方案名為「切韻拼音三拼輸入方案」，可簡稱「切拼三拼」，不叫「切韻三拼」哦～
