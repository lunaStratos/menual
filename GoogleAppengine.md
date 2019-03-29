# Google GCP App engine Tip

## 앱엔진 depoly [엔진에 프로그램 올리기]

* gcloud app deploy
일반적인 올리기 

* gcloud app deploy app.yaml
app.yaml 설정 적용한 프로그램 올리기 

* gcloud app deploy cron.yaml

일정 주기로 실행하는 프로그램 메뉴얼 설정을 올리기
(애는 프로그램 deploy후 따로 하면 된다. 한 30초 걸림)

## Google mysql 연결

왠만하면 같은 프로젝트 내에서 실행.
cloudsql 빈 폴더를 만들어 놓아야 한다.

## Time

* let d = new Date(new Date().getTime() + 9 * 3600000);
이렇게 해야 KST에 맞춰집니다. 

* let arriveDate = new Date(d.getFullYear(), new Date().getMonth(), new Date().getDate(), 10, 02, 10)
정상적으로 출력 되는 시간 설정 

* const waitTime = new Date(d.getTime() + 30 * 60000)
30분 추가 
