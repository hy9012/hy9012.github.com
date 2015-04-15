---
title:  "우분투에서 서브라임텍스트에 나눔 글꼴 설치"
date:   2015-04-14 22:37:00
categories: sublimetext
---

#우분투에 나눔 글꼴 설치

* wget http://cdn.naver.com/naver/NanumFont/fontfiles/NanumFont_TTF_ALL.zip
* unzip NanumFont_TTF_ALL.zip
* mkfontscale
* mkfontdir
* fc-cache -r

#서브라임 텍스트 설정

* Preferences -> user에 아래내용 복사
{% highlight json %}

{
	"font_face":"{설정할 글꼴}",
	"font_size": 12,
	"ignored_packages":["Vintage"]
}

{% endhighlight %}
