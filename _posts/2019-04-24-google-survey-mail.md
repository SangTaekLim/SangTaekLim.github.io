---
layout: post
title: test
img: google-survey-tit.jpg
---


# 구글설문지 메일 연동
구글 설문지를 작성하면 신청자를 메일로 받을 수 있다. 

#### 응답 페이지에서 플러스 버튼을 누른 후 새 스프레드시트 만들기를 누르면

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_1.jpg)

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_2.jpg)

#### 도구에 스크립트 편집기를 클릭후 프로젝트 이름을 편집 가능하다

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_3.jpg)

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_4.jpg)

#### 스크립트를 통해 양식작성시 원하는 메일로 신청자를 확인 할 수 있다.

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_5.jpg)

```javascript
function onFormSubmit(e) {
    MailApp.sendEmail("관리자 메일 주소", "000 설문이 접수되었습니다.", e.values);
}
```

#### 트리거 설정

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_6.jpg)

새 트리거를 만듭니다.

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_7.jpg)

이벤트 유형을 양식 제출시로 변경

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_8.jpg)

#### 엑세스 허용

트리거 설정을 완료하면 엑세스 허용 페이지가 나옵니다.

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_9.jpg)

#### 메일확인

엑세스 까지 허용 완료 후 설문지를 제출해보면 등록한 메일에서 확인 가능합니다.

![delete gh-pages branch]({{site.baseurl}}/images/gogle_survey_10.jpg)
