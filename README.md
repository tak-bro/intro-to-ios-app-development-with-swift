#Intro-to-ios-app-development-with-swift

## 2017-01-05
####Homework
- 개인의 영어 이름을 지어보세요. 앞으로 서로 이렇게 불러보는 것도 좋을듯… 실제 회사에서는 이렇게 운영되는 경우들이 많아지고 있습니다.
	- 아직 못정함
	
- 지금까지 직접 사용해본 앱들 중에 하나를 골라 UI를 캡처해서 그 이면의 내용을 상상하고 MVC 패턴으로 구성해보세요. 한장이면 됩니다.
	- <img src="https://cloud.githubusercontent.com/assets/7614353/21704734/82709d1e-d3fe-11e6-808e-3ebcaece9715.PNG" width="200">  <img src="https://cloud.githubusercontent.com/assets/7614353/21704732/826e3dc6-d3fe-11e6-8c16-cde19f92b5b2.PNG" width="200">
	- 위 왼쪽이미지(View)에서 Send 버튼 클릭(User Action)
	- User Action을 통해 Controller 에게 "뷰" 라는 문자열이 입력되고, Controller는 이 "뷰" 문자열을 Model로 Update
	- Model에서는 "뷰"를 push하는 내부작업을 진행한 후, Controller에게 Notify
	- Controller는 Model로부터 받은 "뷰" 문자열을 View에게 다시 Update
	- 위 오른쪽 이미지처럼 View에서 "뷰" 문자열 업데이트
	
- 지금까지 사용해본 앱들 중에 Navigation Controller 기반의 앱 3가지와, Single View Controller 기반의 앱 3가지 정도를 찾아 화면을 캡처해 설명을 준비해주세요.
  - Single View Controller
		- <img src="https://cloud.githubusercontent.com/assets/7614353/21704734/82709d1e-d3fe-11e6-808e-3ebcaece9715.PNG" width="200"> 계산기
  - Navigation View Controller
		- <img src="https://cloud.githubusercontent.com/assets/7614353/21704733/826ea8ba-d3fe-11e6-932e-59915bd3ddab.PNG" width="250"> Push Bullet
		- 메모
		- Pitch Perfect...
		- 대부분이 Navigation View
    
- Swift로 아주 간단한 코드를 만들어봅시다. 복수의 로또 번호들을 당첨 번호와 비교해서 각각 몇 개와 일치하는지 알려주는 코드입니다. 코딩방법에 따라 여러가지 모양이 나올 수 있으니 꼭 정답을 찾으실 필요는 없습니다. Playground를 사용하시면 됩니다. 
	- 회식... :(
  
- Auto Layout으로 두장의 사진을 미리 준비해서 그 중 한장을 보여주고, 버튼을 누르면 다른 한장으로 바꿔 보여주는 일을 반복하는 앱을 만들어주세요. 혹시 힘들면 Storyboard만 구성해주셔도 됩니다.
	- 일단 Storyboard만 진행함(ImageTap 프로젝트)
  
  
## 2017-01-01
### Audio in iOS
- ![Audio in iOS](https://cloud.githubusercontent.com/assets/7614353/21580454/413ac8aa-d03a-11e6-9399-b322197c2af0.png)
- AVFoundation: av audio recorder을 포함한다.
- Delegate: 개념정리할것
AVAudioRecorderDelegate : protocol
- ![Stack Views](https://cloud.githubusercontent.com/assets/7614353/21580534/40a32156-d041-11e6-9802-5b5d51eb6965.png)
  - storyboard에서 stack의 distribution을 Fill Equally로 해야 버튼 정렬됨

  
## 2016-12-31
- what I learned
  - how to use storyboard
  - how to add button and enable or disable it
  - how to add other ViewController

### Difference between IBAction and IBOutlet
- UI -> IBAction -> Code
> IBAactions are from UIElement TO code
- UI <- IBOutlet <- Code
> IBOutlets are From code To UIElement

### etc
- option key + 마우스 포인터 : 해당 클래스 설명보기
> help 에서 documentation 볼 수 있다.
- viewDidLoad 가 처음에 call된다.
  - viewDidLoad is called when UIViewController is first loaded into memory
- ![ViewController LifeCycle](https://cloud.githubusercontent.com/assets/7614353/21576472/656c174a-cf74-11e6-94cc-dff728c45303.png)
- ![UINavigationController](https://cloud.githubusercontent.com/assets/7614353/21576686/578daf64-cf7c-11e6-8d6f-516a9e2bc325.png)
- The UINavigationController has a stack of UIViewControllers, and this stack needs to have at least 1 View Controller. It can have as many as your app needs.

