
## NLTK 설치가 안되는 경우

<figure class="align-left">
  <img src="https://i.stack.imgur.com/0F2k3.png" alt="">
  <figcaption>nltk.download() 설치오류 메세지</figcaption>
</figure>

과거 버젼에서 사용되었던 `nltk.download()` 를 사용하면 `CERTIFICATE_VERIFY_FAILED] certificate verify failed` 서버연결 오류로 문제가 발생합니다. 이 대에는 오류 메세지에서 제시하는 각각의 Corpus 파일을 다운받는 방법으로 문제를 해결을 합니다 


>  pip3 install -U nltk 

> import nltk; nltk.download('punkt')

만약 위의 방법으로도 해당 Corpus 가 설치되지 않고 계속 오류메세지를 출력하는 경우에는 수동으로 Punkt Tokenizer Models 다운받아서 설치를 하면 되고. 자세한 내용은 [블로그](http://pubdata.tistory.com/154) 또는 [동영상 해결방법](https://programmers.co.kr/learn/courses/21/lessons/946) 을 참고하세요




<figure class="align-left">
  <img src="https://static1.squarespace.com/static/538cea80e4b00f1fad490c1b/54668a77e4b00fb778d22a34/54668d8ae4b00fb778d2859c/1416007413413/NLTK.png" alt="">
  <figcaption>nltk 자연어 분석도구</figcaption>
</figure>


# 예제와 코드로 알아보는 파이썬 자연어 분석


## 사용한 모듈

    nltk == 3.3
    konlpy == 0.5.1
    wordcloud == 1.5.0
    scikit-learn == 0.19.2
    scipy == 1.1.0
    gensim == 3.5.0
    tensorflow == 1.9.0



## 강의 대상

파이썬 기초를 학습하여, **간단한 파이썬 코드는 이해가능 한** 학생/ 직장인을 대상으로 **자연어 분석과정 전반에 대한** 내용을 다룹니다.


## 강의 목표

Python 기본지식과 딥러닝 기본 이론을 학습해본 분들을 대상으로 **자연어 분석**에 필요한 **용어들의 개념**을 익히고, 간단한 사례와 코트를 통해서 실제 구현하는 방법을 익힙니다.


## 강의 슬라이드


[Step1 wordcloud 실습을 활용한 기본개념 익히기](https://www.slideshare.net/YBkim2/1-word-cloud-108677087)

[Step2 sentence 문장분석](https://www.slideshare.net/YBkim2/2-108677123)

[Step3 meaning 의미분석 / 베이지안 분류](https://www.slideshare.net/YBkim2/3-108677208)

[Step4 RNN 딥러닝 활용](https://www.slideshare.net/YBkim2/4-108677404)


전체과정을 4개의 슬라이드로 분할 구성하였고, 각 각 순서에 따른 연계성을 갖으므로, 이해안되는 부분이 있으시다면 앞의 내용을 한번 더 복습한 뒤 진도를 나아가는 방식으로 진행하시면 도움이 될 것입니다.


## 소스코드 

소스 코드의 주석은 전체 **진행 Process를** 익히는데 도움이 되도록, 작업 단락별 구분하였습니다.