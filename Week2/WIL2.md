# iOS 네이티브 소모임 2회차

# 섹션 4: Swift Programming Basics - Collections, Constants & Variables

### 4.35. Cloning from GitHub and How to Download the L.A.B Project Stubs

Xcode에서 GitHub에 올라온 프로젝트를 Clone하여 사용할 수 있음.

단순히 Http로 복사한 링크를 Xcode에 입력하여 Clone할 수 있음.

[https://github.com/dkhamsing/open-source-ios-apps](https://github.com/dkhamsing/open-source-ios-apps)

### 4.36. How to Design Your App

Content Mode를 변경해주어서 배경화면에 이용할 사진을 꽉 채우게 변경할 수 있음.

Aspect fill로 설정하면 전체 이미지뷰에 맞추면서 세로 비율을 유지함. (여러 개를 선택하여 동시에 복제할 수도 있음.)

`Option[Alt] + 드래그`를 하여 기존의 개체를 복제하여 배치할 수 있음.

### 4.37. Let’s Link Our Design to Our Code

ViewController.swift → 메인 코드 파일, Main.storyboard → 디자인 파일

Assistant 상태에서는 코드와 스토리보드 파일을 동시에 켜놓고 볼 수 있음.

이미지 뷰를 참조하기 위해 `Control + 드래그`를 하여 코드의 원하는 위치로 보내어 사용할 수 있음. → **`Interface Builder Outlet`**

반대 방향으로도 단축키를 이용하여 링크할 수 있음.

**camelCase**: 첫 글자는 소문자, 이후 단어마다 맨 첫 글자는 대문자.

viewDidLoad(): 앱이 폰에 처음 나타날 때 보여지는 화면을 설정할 수 있음.

Image Literal을 통해 이미지 뷰의 이미지를 설정할 수 있음.

`ex) diceImageView1.image = Image Literal #`

### 4.38. Responding to User Interactions with IBActions

이미지 뷰의 모습을 바꾸기 위해서는 참조 또는 IBOutlet이 올바른 이미지뷰를 잡을 수 있어야함.

버튼도 IB로 연결하기 위해서 똑같이 `Control + 드래그`를 함.

→ Connection을 Action으로 설정하여 상호작용이 되도록 함. 

→ 해당 Action은 특정 이벤트에 의해 트리거됨. 

⇒ 흔히 필요한 것은 `**Touch Up Inside**`: 손가락이 버튼의 테두리 안에 들어갔고, 테두리 안에 있을 때 손가락을 들어올림.(일반적인 탭 제스처)

→ 생성되는 코드가 Interface Builder Action 형식. (함수처럼 생김.)

IBOutlet은 Code에서 Design 방향으로 상호작용하지만, IBAction은 Design에서 Code 방향으로 작동함.

### 4.40. [Swift Deep Dive] Naming Conventions, Commenting and String Interpolation

> Naming Conventions
> 

`**camelCase**, kebab-case, snake_case`

> Commenting
> 

`Command + /`를 통해 주석으로 만들어 버릴 수 있음.

> String Interpolation
> 

`\()`를 이용하여 print()내에서 연산을 할 수 있음.

ex) `print(”Hello World \(1+2)”)`

### 4.41. Storing Data using Variables and Arrays

swift에서 배열 만드는 방법: 대괄호를 이용하여 선언. 인덱스도 대괄호를 이용하여 접근.

### 4.42. [Swift Deep Dive] Variables

변수: 데이터에 이름을 부여하는 방법(Lable)

변수를 선언하는 키워드: `var`

### 4.43. [Swift Deep Dive] Arrays

데이터와 마찬가지로 변수에 저장할 수 있음.

### 4.44. How to Randomise the Dice Images

`Int.random(in: 1…10)`

배열을 선언할 때, 등호를 기준으로 양쪽에 공백이 둘다 있거나, 둘다 없거나 해야 오류가 생기지 않음.

ex) `Arrays = [], Arrays=[]`

상수를 선언하는 키워드: let → 코드에서 변수의 값이 변하는 코드가 없는 경우 상수로 선언하도록 주의 표시가 뜸.

배열에서 임의의 요소를 반환하는 메소드: `Array.randomElement()`

### 4.46. [Swift Deep Dive] Constants, the Range Operator and Randomisation

> 기본 데이터 타입
> 

`String`: `“”`를 통해 구분함. (큰따옴표)

`Integer, Floating Point Number, Double, Boolean`

> Range Operator
> 

`Int.random(in: lower ..< upper)` → upper 값은 나오지 않음.

Float, bool에도 똑같이 사용 가능.

⇒ 배열에서 랜덤 요소를 뽑아내기 위해서 `randomElement` 메소드를 사용하는 방법도 있지만, `Array.shuffle()`을 통해 요소를 섞을 수도 있음.

문자열은 단순히 덧셈으로 더할 수 있음.