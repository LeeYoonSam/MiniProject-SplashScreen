# SplashScreen
액티비티를 추가하지 않고 Splash Screen을 표시

- 이 접근 방식은 애니메이션과 같은 시간 제한 작업을 허용하지 않습니다.
- 주로 활동이 onCreate를 호출하는 동안 시작 화면을 지속시켜 시작 시 어색한 공백 흰색/검정색 활동을 방지하기 위한 것입니다.


## 1. 스플래시 스크린에서 사용할 로고를 추가
- res > New > Vector Asset
- 로고로 사용하고 싶은 이미지 추가

## 2. 스플래시 이미지 생성
- res > drawable > New > Drawable Resource File > splash_image.xml 생성
- selector -> layer-list 로 변경
- 배경색, 로고 아이콘을 겹쳐서 item 추가

## 3. 스플래시 스크린 테마를 추가
- res > values > themes 이동
- 스플래시 테마 추가
    - windowBackground : 보여줄 로고 이미지
    - statusBarColor : 상태바 색상 변경

## 4. 스플래시 스크린 적용
- AndroidManifest.xml > application 테마 변경 (스플래시 테마)
- MainActivity 테마 변경 (기존에 사용중이던 기본 테마)
    - setContentView 전에 테마를 설정


## 참고
[How to make a Splash Screen without extra Activity in Android](https://www.youtube.com/watch?v=rIHArmoq9f8&t=129s)