### Component
- UI단위

### Props
- 컴포넌트의 속성값이 저장되는 주머니다.
- 컴포넌트를 생성할 때 Props에 값을 넣어서 상황에 따라 형태가 다르게 만들면 재활용 가능한 컴포넌트를 만들 수 있다.

### State
- 컴포넌트의 상태값이 저장되는 주머니다.
- 유저 인풋이나 서버 응답에 의해 받아온 상태값을 State에 담아 활용할 수 있다. 그러면 동적 UI가 된다.

### Style
- 이미 정의된 Pros.
- CSS와 같은 효과를 낼 수 있으며 CSS에서 처럼 background-color가 아니라 카멜케이스 처럼 backgroundColor로 사용해야 한다.
- 스타일은 배열 형태로 사용할 수도 있고 상속해서 사용할 수도 있다.

### Dimensions
- Fixed
	- 안드로이드의 DIP와 같은 개념으로 사용한다.
	- 크기 지정 시 값에 unit(like px)을 따로 붙이지 않는다.
	- 어떤 크기-비율의 스크린에서 봐도 항상 거의 같은 크기로 그려진다.
- Flex
	- 안드로이드의 LinearLayout 안에서 자식뷰들이 weight를 가지고 서로의 크기를 할당받는 개념과 같다.
	- Flex 크기는 Fixed 크기를 제외한 영역에서 나눠갖는다.

### Flexbox
- Flexbox 개념은 다른 사이즈의 화면에서 일관된 레이아웃을 제공하기 위해 고안됐다.
- 자식뷰들을 어떻게 layout(배치)할지를 자세하게 기술할 수 있다.
- CSS에서 사용하는 것과 같지만 몇 가지 예외가 있다.
	- flexDirection의 기본값은 row가 아니라 column이다.
	- flex의 값은 단일 숫자만 지원된다.
- Styles
	- flexDirection
		- 자식을 나열할 때 가장 먼저 기준이 되는 축(primary axis)의 방향
	- justifyContent
		- 자식들이 공간을 어떻게 나눠가질지
		- 값: flex-start, center, flex-end, space-around, and space-between
	- alignItems
		- primary axis 말고, secondary axis, 즉 flexDirection이 column이었으면 secondary axis는 row가 된다. secondary axis에서 자식들을 어떻게 정렬할 것인지
		
### Networking
- Fetch API
	- 네트워크 요청을 위해 Fetch API를 제공합니다.
	- 네트워킹은 비동기로 진행되기 위해 fetch 메소드는 Promise 객체를 반환합니다.
- WebSocket
	- 웹소켓은 양방향 통신이 가능합니다.


### Popular Libraries
- Redux
	- State를 어떻게 관리하고 다루는가를 패턴화하여 쉽게 사용할 수 있게끔 해주는 라이브러리
	- 매우 단순한 구조
- 샘플
	- 플레이그라운드 : https://rnplay.org/apps/picks
	- 2016 F8앱 소스 : https://github.com/fbsamples/f8app
		- 시리즈 : http://makeitopen.com/tutorials/building-the-f8-app/planning/
- 개발툴
	- Nuclide
		- RN 디버깅 기능 제공
	- Ignite
		- Redux와 UI 라이브러리들에 대한 스타터 킷
	- CodePush
		- 앱스토어 업뎃 없이 라이브로 RN앱을 업데이트 시킬 수 있는 서비스 by 마소
	- Exponent
		- AS, XCode 없이 Javascripty, Webby스럽게 RN앱을 제작할 수 있다.
	- Deco
		- 올인원 RN앱 제작만을 위한 개발툴
		- RN 프로젝트 생성, 라이브러리 검색, 앱 실행 등이 가능
		- 오직 맥에서만 가동



### Widget
- Text
- View
- TextInput
- Image
- ScrollView
	- ScrollView는 스크린에 보이지 않더라도 자식들 모두를 그립니다. 때문에 매우 긴 레이아웃을 가질 경우 ListView를 써야 합니다.
- ListView
	- Props로 dataSource와 renderRow가 필수다.





