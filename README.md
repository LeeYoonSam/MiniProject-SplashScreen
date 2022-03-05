# SplashScreen
액티비티를 추가하지 않고 Splash Screen을 표시

## 1. 스플래시 스크린에서 사용할 로고를 추가
- res > New > Vector Asset
- 로고로 사용하고 싶은 이미지 추가

## 2. 스플래시 이미지 생성
- res > drawable > New > Drawable Resource File > splash_image.xml 생성
- selector -> layer-list 로 변경
- 배경색, 로고 아이콘을 겹쳐서 item 추가

## 3. 스플래스 스크린 테마를 추가
- res > values > themes 이동
- 스플래시 테마 추가
    - windowBackground : 보여줄 로고 이미지
    - statusBarColor : 상태바 색상 변경