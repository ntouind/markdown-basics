---
image: https://cdn.staticaly.com/gh/dcurtis/markdown-mark/3a8ab86a/png/1664x1024.png
tags: Markdown, 文件標記語言, 教材, 簡報, HackMD
---

# Markdown<br>文件標記語言簡介

<https://hackmd.io/p/HkgoF4i9gG>

海洋大學網路發展協會  
<http://ind.ntou.edu.tw>

這是一個基於 Markdown 的 [HackMD](https://hackmd.io) 簡報  
[點此查看本簡報的來源碼](https://hackmd.io/GYUwDAHAzGJQtGAJmAxvALNY8BGwA2DeJEDDAQygE4RUlrUg)

---

<a href='https://creativecommons.org/licenses/by-sa/4.0/' target='_blank'><img src='https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-sa.svg' style='width: 50%; height:auto' /></a><br>歡迎於授權範圍內自由使用本作品

---

## Markdown 的特色<br><small>Markdown Features</small>

* 源碼可讀性高（與純文字電子郵件格式雷同）
* 可直接轉換為 HTML 網頁，可混用 HTML 標記
* 內容與格式化分離，要美化可套用 CSS
* 第三方功能擴充性高（視 Markdown 應用支援）

---

## 支援 Markdown 的編輯器<br><small>族繁不及備載</small>

### Web 應用

* [HackMD](https://hackmd.io)
* [Stackedit](http://stackedit.io)

### 本地端應用

* [Typora](https://typora.io/)

---

## 標題<br><small>Headings</small>

---

### ATX 風格

```markdown
# 第一階標題
## 第二階標題
...
###### 第六階標題（行尾的井號僅有美觀效果不會出現在轉換結果中） ######
```

<hr>

<h1>第一階標題</h1>
<h2>第二階標題</h2>
...
<h6>第六階標題（行尾的井號僅有美觀效果不會出現在轉換結果中）</h6>

---

### Setext 風格

```markdown
第一階標題
===

第二階標題
---
```

<hr>

<h1>第一階標題</h1>
<h2>第二階標題</h2>

---

## 一般文字<br><small>Regular Text</small>

```markdown
不需要任何語法，直接輸入即可
```

<hr>

不需要任何語法，直接輸入即可

---

## 換行<br><small>Line Breaks</small>

行尾加上兩空白字元就能換行

```markdown
第一行[][]   
第二行
```

<hr>

第一行  
第二行

---

## 段落<br><small>Paragraphs</small>

```markdown
這是第一段的內容。

間隔一空行的內容會自動呈現為第二段。

第三段，留意段落之間的留白並非為一空行所構成。
```

<hr>

這是第一段的內容。

間隔一空行的內容會自動呈現為第二段。

第三段，留意段落之間的留白並非為空行所構成。

---

## 超連結<br><small>Hyperlinks</small>

```markdown
[Google 搜尋引擎](https://google.com)

<https://google.com>
```

<hr>

[Google 搜尋引擎](https://google.com)

<https://google.com>

---

## 插入圖片<br><small>Image Insertion</small>

```markdown
![Reddit r/place畫布中的Taiwan No.1](https://i.imgur.com/fefdJO5.png "Taiwan No.1")

![圖片失效時會顯示其替代文字](https://i.imgur.com:65536/fefdJO5.png)
```

<hr>

![Reddit r/place畫布中的Taiwan No.1](https://i.imgur.com/fefdJO5.png "Taiwan No.1")

![圖片失效時會顯示其替代文字](https://i.imgur.com:65536/fefdJO5.png)

---

## 清單<br><small>Lists</small>

* 購物清單
* 代辦事項清單
* 資產清單

---

### <ruby>無序<rp>(</rp><rt>無順序性的</rt><rp>)</rp></ruby>清單<br><small>Unordered List</small>

```markdown
* 就像這樣
	+ 子清單項目
	+ 星號、減號、加號都可以當作清單項目符號（不影響呈現式樣）
		- Markdown 主要使用 4 個空格或 1 個換欄號(Tab)作為縮排使用
```

<hr>

* 就像這樣
	+ 子清單項目
	+ 星號、減號、加號都可以當作清單項目符號（不影響呈現式樣）
		- Markdown 主要使用 4 個空格或 1 個換欄號(Tab)作為縮排使用

---

### <ruby>有序<rp>(</rp><rt>有順序性的</rt><rp>)</rp></ruby>清單<br><small>Ordered List</small>

```markdown
1. 就像這樣
1. 呈現出來的編號永遠用自然數遞增，不隨源碼使用的編號數字影響
	* 子清單可混用無序清單
		1. 反之亦可
5. 同第 2 項
```

<hr>

1. 就像這樣
1. 呈現出來的編號永遠用自然數遞增，不隨源碼使用的編號數字影響
	* 子清單可混用無序清單
		1. 反之亦可
5. 同第 2 項

---

### 清單與非清單內容間須額外留一空行

```markdown
這是等一下要採購的東西：

* 蘋果
* 香蕉
* 芭樂

記得要拿發票
```

<hr>

這是等一下要採購的東西：

* 蘋果
* 香蕉
* 芭樂

記得要拿發票

---

## 區塊引言<br><small>Blockquotes</small>

```
> > 奇藍藍奇CP可逆不可拆
> > 
> 我覺得不行
> 
我覺得可以
```

<hr>

> > 奇藍藍奇CP可逆不可拆
> > 
> 我覺得不行
> 
我覺得可以

---

## 預格式化文字<br><small>Pre-formatted Text</small>

<pre>
```
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char * argv[]){
	printf("Hello world!\n");
	return EXIT_SUCCESS;
}
```
</pre>

<hr />

```c
/* 程式碼語法色彩突顯為擴充語法 */
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char * argv[]){
	printf("Hello world!\n");
	return EXIT_SUCCESS;
}
```

---

## 水平線<br><small>Horizontal Line</small>

```
---
```

<hr />

就會呈現為一水平線↑

---

## 強調<br><small>Emphasis</small>

```
**這段文字呈現為粗體**

*這段文字呈現為斜體*

***這段文字呈現為粗斜體***
```

<hr />

**這段文字呈現為粗體**

*這段文字呈現為斜體*

***這段文字呈現為粗斜體***

---

## 第三方擴充語法<br><small>Third-party Syntax Extensions</small>

這些語法並非在 Markdown 標記語言中，是否支援視各應用實作而定

---

### 刪除線<br><small>GitHub Flavored Markdown 擴充語法</small>

```markdown
在套用的內容兩側加上兩個波浪號即可套用~~刪除線~~
```

<hr>

在套用的內容兩側加上兩個波浪號即可套用~~刪除線~~

---

### 插入表格<br>Table Insertion<br><small>GitHub Flavored Markdown 擴充語法</small>

```markdown
| 表頭1 | 表頭2 |
| ---- | ---- |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |
```

<hr>

| 表頭1 | 表頭2 |
| ---- | ---- |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |

---

### 插入表格<br>Table Insertion<br><small>GitHub Flavored Markdown 擴充語法</small>

```markdown
| 表頭1 | 表頭2 |
| :--: | :--: |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |
```

<hr>

| 表頭1 | 表頭2 |
| :--: | :--: |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |

---

### 插入表格<br>Table Insertion<br><small>GitHub Flavored Markdown 擴充語法</small>

```markdown
| 表頭1 | 表頭2 |
| ---: | ---: |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |
```

<hr>

| 表頭1 | 表頭2 |
| ---: | ---: |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |

---

### 插入表格<br>Table Insertion<br><small>GitHub Flavored Markdown 擴充語法</small>

```markdown
| 表頭1 | 表頭2 |
| :--- | :--- |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |
```

<hr>

| 表頭1 | 表頭2 |
| :--- | :--- |
| 第1列第1欄的值 | 第1列第2欄的值 |
| 第2列第1欄的值 | 第2列第2欄的值 |

---

## Task List Item<br><small>GitHub Flavored Markdown 擴充語法</small>

```
* [ ] 吃飯
* [ ] 睡覺
* [x] 打東東
```

<hr>

* [ ] 吃飯
* [ ] 睡覺
* [x] 打東東

---

### LaTeX 數學 / 科學公式輸入<br><small>GitBook/ReText/HackMD/StackEdit等Markdown應用限定</small>

```markdown
$$ 
	F_e = \frac{1}{4 \pi \epsilon_0} \frac{q_1 q_2}{r^2}
$$

答案是 $3X$
```

<hr />

$$ 
	F_e = \frac{1}{4 \pi \epsilon_0} \frac{q_1 q_2}{r^2}
$$

<a href='https://youtu.be/sVLtR8Ebq0U?t=45s'><img src='https://i.imgur.com/HBLcK6v.png' style='height: 80px' title='哽來源：芬達廣告（依據合理使用原則引用）' /></a>答案是 $3X$ 


---

## 語法參考<br><small>References</small>

* [Daring Fireball: Markdown Syntax Documentation](https://daringfireball.net/projects/markdown/syntax)  
  Markdown 發明者的說明文件
* [Markdown 語法說明](http://markdown.tw)  
  前一項目的台灣中文翻譯
* [CommonMark - A strongly defined, highly compatible specification of Markdown](http://commonmark.org)
  定義更精確的第三方Markdown規範
