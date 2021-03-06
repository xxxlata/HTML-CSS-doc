# Box-sizing #

CSS 박스 모델의 기본값에서, 지정한 너비와 높이는 요소의 콘텐츠 박스 크기에만 적용됩니다.
요소에 테두리나 안쪽 여백이 있으면 너비와 높이에 더해서 화면에 그립니다.
따라서 크기를 설정할 때, 원하는 크기를 얻으려면 테두리나 안쪽 여백을 고려해야 합니다.

### content-box ### 
content-box는 기본 CSS 박스 크기 결정법을 사용합니다. 요소의 너비를 100 픽셀로 설정하면 콘텐츠 영역이 100 픽셀 너비를 가지고, 테두리와 안쪽 여백은 이에 더해집니다.

### border-box ###

border-box는 테두리와 안쪽 여백의 크기도 요소의 크기로 고려합니다. 
너비를 100 픽셀로 설정하고 테두리와 안쪽 여백을 추가하면, 콘텐츠 영역이 줄어들어 총 너비 100 픽셀을 유지합니다. 대부분의 경우 이 편이 크기를 조절할 때 쉽습니다.
<img src="https://github.com/xxxlata/HTML-CSS/blob/main/boxsizing.png" width="700" height="300"/>

-------------------
## block ##

block은 한 영역을 차지 하는 박스형태을 가지는 성질입니다. 
그렇기 때문에 기본적으로 block은 width값이 100%가 됩니다. 그리고 라인이 새로 추가된다는 것을 알 수 있습니다. 

<특성><br>
1.block은 height와 width 값을 지정 할 수 있다.<br>
2.block은 margin과 padding을 지정 할 수 있다.
<br>
(ex)<br>
```
<header>
<div>
<h1> ~ <h6>
<section>
<p>
<form>
<footer>
```

## inline ##

inline은 주로 텍스트를 주입 할 때 사용 되는 형태입니다.
그렇기 때문에 기본적으로 block처럼 width값이 100%가 아닌 컨텐츠 영역 만큼 자동으로 잡히게 되며 라인이 새로 추가 되지 않습니다.
높이 또한 폰트의 크기만큼 잡힙니다.(line-height로 설정이 가능 하긴 합니다.)

<특성><br>
1.width와 height를 명시 할 수 없다.<br>
2.margin은 위아래엔 적용 되지 않는다.<br>
3.padding은 좌우는 공간과 시각적인 부분이 모두 적용 되지만 위아래는 시각적으로는 추가되지만 공간을 차지 하지는 않는다.
<br>
(ex)<br>
```
<span>
<a>
<img>
```
## inline-block

inline-block 은 말그대로 inline의 특징과 block의 특징을 모두 가진 요소입니다. inline-block의 특징은 다음과 같습니다.


<특성><br>
1.줄바꿈이 이루어지지 않는다.<br>
2.block처럼 width와 height를 지정 할 수 있다.<br>
3.만약 width와 height를 지정하지 않을 경우, inline과 같이 컨텐츠만큼 영역이 잡힌다.
