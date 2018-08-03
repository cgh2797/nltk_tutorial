
<figure class="align-left">
  <img src="https://static1.squarespace.com/static/538cea80e4b00f1fad490c1b/54668a77e4b00fb778d22a34/54668d8ae4b00fb778d2859c/1416007413413/NLTK.png" alt="">
  <figcaption>nltk 자연어 분석도구</figcaption>
</figure>


## NLTK 설치가 안되는 경우

`nltk.download()` 또는

`$ sudo python -m nltk.downloader -d /usr/local/share/nltk_data all` 를 사용해도 

> `CERTIFICATE_VERIFY_FAILED] certificate verify failed` 

오류로 서버와 연결이 안되는 경우에는 수동으로 Punkt Tokenizer Models 다운받아서 설치를 해야 한다

[NLTK](http://www.nltk.org/nltk_data/) 이곳에서 punkt를 찾아 다운로드를 받는다

    Windows: C:\nltk_data\tokenizers
    OSX: /usr/local/share/nltk_data/tokenizers
    Unix: /usr/share/nltk_data/tokenizers

다운받은 파일을 운영체계별로 해당하는 폴더에 수동으로 압축을 풀어준다. 보다 자세한 설명은 [블로그](http://pubdata.tistory.com/154) 또는 [동영상 해결방법](https://programmers.co.kr/learn/courses/21/lessons/946) 을 참고하면 된다




# 예제와 코드로 알아보는 파이썬 자연어 분석


## 사용한 모듈

    nltk == 3.2.5
    konlpy == 0.4.4
    scikit-learn == 0.19.1
    gensim == 3.5.0
    tensorflow == 1.7.0



## 강의 대상

파이썬 기초를 학습하여, 간단한 파이썬 코드는 이해가능한 학생/ 직장인을 대상으로 자연어 학습에 대한 전반적인 내용을 다룰 예정입니다.


## 강의 목표

Python 사전지식을 바탕으로 **자연어 분석**에 필요한 **용어들의 개념**과 각 각의 차이점 을 이해하고, 사례와 이에 해당하는 샘플코드를 활용하여 이를 실제 구현하는 방법들을 실습합니다.

최대한 수식 및 연산 과정은 제외하고, 대표적인 사례들을 중심으로 개념들을 배치하여 보다 직접적이고, 직관적인 수업이 진행되도록 구성되어 있습니다


## 강의 슬라이드


[wordcloud 실습을 활용한 기본개념 익히기](https://www.slideshare.net/YBkim2/1-word-cloud)

[sentence 구조 분석](https://www.slideshare.net/YBkim2/2-sentence)

[meaning 의미 분석 / 베이지안 분류](https://www.slideshare.net/YBkim2/3-108453530)

[RNN 딥러닝의 활용](https://www.slideshare.net/YBkim2/4-108453864)


전체 과정은 4개의 슬라이드로 구성이 되어 있고, 이들은 순서에 따른 연계성을 갖기 때문에 이해안되는 부분이 있으면 앞의 내용을 한번 더 복습한 뒤 진도를 나아가는 방식으로 진행을 하면 많은 도움이 될 것입니다.


## 소스코드 

코드들은 가장 간단한 구조의 예제들로 구성되어 있으며, 소스 코드에 대한 주석들은 최소화 하여, 코드들이 묶음으로써 전체 진행 Process를 익히는데 도움이 되도록, 단락별 구분내용으로 최소화하여 구분 하였습니다 


## Content

질문 및 건의내용들은 Issue에 남겨주시거나, saltman21@naver.com 로 메일을 보내주신다면, 제가 해결가능한 범위 내 성심성의 것 답변 드리겠습니다.