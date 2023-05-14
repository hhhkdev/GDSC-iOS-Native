# iOS 네이티브 소모임 1회차

# 섹션 1. Getting Started with iOS Development and Swift 5

[iOS Course Resources](https://www.appbrewery.co/p/ios-course-resources/)

### 1.4 How does an App Work?

앱이 어떻게 동작하는가? 스마트폰도 컴퓨터와 별로 다르지 않음. 

입력에 대해 어떻게 반응할 지 설정해주어야 함. 상호작용에 대한 작동.

컴퓨터와의 차이점 - 배터리가 노트북에 비해 딸림, 메모리와 처리 능력이 떨어짐(리소스 제한). 

# 섹션 2. Xcode Storyboards and Interface Builder

### 2.17 Let’s Create a Brand New Xcode Project

organization identifier: 리버스 도메인 형태

번들 식별자를 통해 앱 스토어에서 구분할 수 있음.

프로젝트 파일 확장자: .xcodeproj

### 2.18 A Walkthrough of the Xcode Development Environment

Xcode의 기본 레이아웃은 4개의 영역으로 나뉨.

상단 상태 표시줄(실행, 경로 등), 왼쪽 내비게이터 창(디렉터리, 프로젝트 내비게이터 등 파일 탐색), 오른쪽 창(크기 검사기 등 중간 창에 보이는 것에 대한 세부 설정), 코드 입력 창(문서 개요 - 레이어)

command + shift + Y 를 통해 하단 창을 토글할 수 있음.

Main.storyboard에서 디자인할 수 있음.

ViewController.swift에서 앱의 동작을 변경하기 위해 코드를 작성할 수 있음.

### 2.19 Let’s Design the User Interface!

LaunchScreen.storyboard에서는 말 그대로 앱을 처음 실행시켰을 때 나오는 로고 같은 화면.

따라서 디자인하기 위해서는 Main.storyboard에서 해야 함.

[Color Palettes for Designers and Artists - Color Hunt](https://colorhunt.co/)

왼쪽 상단을 (0, 0)으로 하여 좌표평면이 있다고 가정함. 요소의 좌표는 요소의 좌측 상단을 기준으로 측정함.

[PaintCode - Turn your drawings into Objective-C or Swift drawing code](https://www.paintcodeapp.com/news)

### 2.20 Let’s Incorporate Some Image Assets

이미지뷰 - 이미지를 넣을 수 있는 하나의 액자. 

[App Icon Generator](https://www.appicon.co/#image-sets)

위 링크를 통해 1x 2x 3x 앱 아이콘을 바로 생성해낼 수 있음. 

### 2.21 How to Design and Add an App Icon

아이콘 이미지 이름을 통해 Xcode에서 사진을 자동으로 배치해줄 수 있음.

앱 아이콘도 App Icon Generator를 통해 여러 사이즈의 아이콘을 만들어 낼 수 있음.

App Icon 사진 넣는 곳이 강의와 다르게 나오는데 뭐가 문제지? 단순히 성능이 좋아져서 사진을 여러 종류 넣을 필요가 없어진걸까?

# 섹션 3. Xcode Storyboards and Interface Builder Challenge
