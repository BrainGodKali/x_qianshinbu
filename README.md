# 个人博客

这是我个人网站的源代码（是我第一次用VScode做开发，在此之前我没有任何网页开发基础）。

我使用的开发工具为Visual Studio Code，（一开始用的是Adobe Dreamweaver，但因各种原因改用Visual Studio Code）。

---

## 开始制作

再次说明，在此之前我没有任何网页开发基础，所以先学习（速成）再开发。

速成班：[HTML](https://www.bilibili.com/video/BV1vs411M7aT/) & [CSS](https://www.bilibili.com/video/BV1bW411R7hg) (暂时没有JavaScript[😢]()😢😢)，

我使用的开发工具为Visual Studio Code，（一开始用的是Adobe Dreamweaver，但因显示与edge网页不同的原因改用Visual Studio Code）。

## 遇到麻烦

最头疼的就是关于分辨率的问题，我的电脑说1080P分辨率为主，但是放到手机这样的小分辨率设备上，可能会出现文字挤压的情况

以下代码解决。

```css
@media screen and (min-width:1200px){ /*1280分辨率以上（大于1200px）*/
#page{ width: 1100px; }#content,.div1{width: 730px;}#secondary{width:310px}
}
```

```css
@media screen and (min-width: 960px) and (max-width: 1199px) { /*1100分辨率（大于960px，小于1199px）*/
    #page{ width: 960px; }#content,.div1{width: 650px;}#secondary{width:250px}select{max-width:200px}
}
```

```css
@media screen and (min-width: 768px) and (max-width: 959px) { /*880分辨率（大于768px，小于959px）*/
    #page{ width: 900px; }#content,.div1{width: 620px;}#secondary{width:220px}select{max-width:180px}
}
```

```css
@media only screen and (min-width: 480px) and (max-width: 767px){ /*720分辨率（大于480px，小于767px）*/
    #page{ width: 450px; }#content,.div1{width: 420px;position: relative; }#secondary{display:none}#access{width: 450px; }#access a {padding-right:5px}#access a img{display:none}#rss{display:none}#branding #s{display:none}
}
```

```css

@media only screen and (max-width: 479px) { /*440分辨率以下（小于479px）*/
    #page{ width: 300px; }#content,.div1{width: 300px;}#secondary{display:none}#access{width: 330px;} #access a {padding-right:10px;padding-left:10px}#access a img{display:none}#rss{display:none}#branding #s{display:none}#access ul ul a{width:100px}
}
```

## 完工

然后我就不多说了😂😂😂
