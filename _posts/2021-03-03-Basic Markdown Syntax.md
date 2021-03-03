---
layout: post
title: Basic Markdown Syntax
---

>자주 사용하는 Markdown 문법 모음

Github 블로그를 꾸며 나가면서 필요한 기본적인 Markdown 문법들을 정리해 보았습니다. Markdown 문서를 사용하면서 느낀 점은 기본적으로 html 문법에 대한 이해가 있다면 배우기 어렵지 않다는 점입니다. 하지지만 그보다 가독성이 뛰어나고, 문법과 구조가 간단하여 쓰기 쉬운 특징을 갖습니다.


### 해더 Header 사용법
<hr/>
해더는 제목(글머리)입니다. H1일수록 크고 H6일수록 작아요. #의 개수와 동일하으로 쉽게 사용하실 수 있습니다.

```markdown
# H1 Header
## H2 Header
### H3 Header
#### H4 Header
##### H5 Header
###### H6 Header
```

# H1 Header
## H2 Header
### H3 Header
#### H4 Header
##### H5 Header
###### H6 Header

<br>
### BlockQuote 사용법
<hr/>
BlockQuote는 인용 블록입니다. >가 반복될수록 들여쓰기 됩니다. BlockQuote안에 다른 마크다운 요소도 포함 가능합니다.


```markdown
> BlockQuote
> ** asterisks를 사용하여 bold text 표현 **
> > BlockQuote
> - 다른 마크다운 요소 삽입 가능
>	>	> BlockQuote

```

> BlockQuote
> ** asterisks를 사용하여 bold text 표현 **
> > BlockQuote
> - 다른 마크다운 요소 삽입 가능
>	>	> BlockQuote

<br>
### Link 사용법
<hr/>
블로그를 쓰다보면 다양한 링크를 사용하게 됩니다. 링크를 사용하는 많은 방법이 있으나 본 포스트에서는 아래의 3가지 방법만 소개합니다.


```markdown
[Google](https://google.com, "google link") // 'Google' 클릭시 이동
<https://google.com> // 링크가 보임
<dm.jskang@kyonggi.ac.kr> // 이메일
```

[Google](https://google.com, "google link") <br>
<https://google.com> <br>
<dm.jskang@kyonggi.ac.kr>

<br>
### CodeBlock 사용법
<hr/>
아직 포스팅하지는 않았지만, 코드를 포함한 글을 쓸 일이 많을 것 같습니다. 기본적인 CodeBlock 사용법을 정리합니다. 좋은 방법이 있다면 추천해주세요!


```markdown

```python
from sklearn.datasets import load_iris
from sklearn.tree import DecisionTreeClassifier

iris = load_iris()
X = iris.data[:, 2:] # 꽃잎 길이와 너비
y = iris.target

tree_clf = DecisionTreeClassifier(max_depth=2, random_state=42)
tree_clf.fit(X, y)
```

```


``` python
from sklearn.datasets import load_iris
from sklearn.tree import DecisionTreeClassifier

iris = load_iris()
X = iris.data[:, 2:] # 꽃잎 길이와 너비
y = iris.target

tree_clf = DecisionTreeClassifier(max_depth=2, random_state=42)
tree_clf.fit(X, y)
```

<br><hr/>
더 자세한 내용은 아래의 markdown 사용법을 확인하세요.<br>
[Basic Syntax](https://www.markdownguide.org/basic-syntax/)<br>
[마크다운(Markdown) 사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601)<br>
[Creating and highlighting code blocks](https://docs.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks#syntax-highlighting)<br>
