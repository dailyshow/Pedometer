# Peometer
###1. 참고 사이트

+ https://gist.github.com/bjoernQ/6975256 always showing service
+ http://isntyet.tistory.com/97 오버레이 권한 6.xx 버전에서 문제 생김 주의
+ http://blog.daum.net/mailss/20 출저
+ http://egloos.zum.com/louienine9/v/9453346 안드로이드 화면 온오프 받아오기
+ http://www.jksii.or.kr/upload/1/845_1.pdf 스텝수 검출 알고리즘
+ http://arabiannight.tistory.com/entry/180 컨텐츠 프로바이더
+ https://github.com/bagilevi/android-pedometer 구글 페도미터
+ http://www.findbestopensource.com/tagged/pedometer 페도미터 오픈소스
+ http://blog.naver.com/cestlavie_01/40188369345 죽지않는 서비스
+ https://github.com/greenrobot/greenDAO 그린다오
+ https://github.com/JakeWharton/butterknife 버터 나이
+ http://gun0912.tistory.com/61 권한 체크
+ https://github.com/ParkSangGwon/TedPermission 권한체크 라이브러리
+ https://gist.github.com/bjoernQ always overayview
+ 이미지 출처 : flaticon.com

###2. 모듈 설명

* com/threabba/android루트폴더
* config 전역 변수 관련
* Const.java 상수 모음
* http
* AddressVO.java 네이버 지도 api json object
* HttpUtil.java http 접속 유틸
* pedometer 만보기 앱 폴더
* components activity, service, contentsprovider등 안드로이드 컴포넌트 모음
* GPSService.java gps송/수후 네이버 api를 이용해 주소를 받아오는 서비스
* MainActivity.java 만보기 기본 메인 엑티비티 본 앱의 컨트롤러 역할을 함
* RecordContentProvider.java db 컨텐츠 프로바이더, greendao에서 자동 generator후 SQLiteDatabase를 추가
* StepService.java 센서 스텝 서비스 및 미니모드 뷰 제공
* db
* DaoMaster.java db 세션관리
* DaoSession.java db 세션, dao 관리
* DBManager.java 데이터를 가공하여 쓰기 위한 메니저
* Record.java 만보기 정보 기록을 위한 data type object
* RecordDao.java record정보를 db에 핸들링 하기 위한 data access object
* fragments 프레그먼트 및 뷰 컴포넌트
* ListViewRecordAdapter.java 만보기 정보 기록을 위한 listview adapter
* PedometerFragment.java 만보기 모니터링 프레그먼트
* RecordFragment.java 만보기 정보 기록 화면 프레그 먼트
* StepMiniView.java 미니 모드를 위한 커스텀 레이아웃
* TabPagerAdapter.java 탭에 프레그먼트를 나누기 위한 아답터
* step
* StepDetector.java
* StepListener.java
* App.java applcation 클래스, db 객체 생성 및 네트워크,로케이션 체크를 담당
* util
* AsyncCallback.java asynctask 콜백
* AsyncExecutor.java aysnctask 클래스 제네릭