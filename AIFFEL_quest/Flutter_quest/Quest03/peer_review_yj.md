🔑 **PRT(Peer Review Template)**

- [O]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 기능이 정상적으로 작동하는지?
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 근거로 첨부
        icon 및 appbar, elevationbutton, image 잘 들어가있었습니다.
        데이터를 전달하는 부분도 구현이 잘 되어있어 true, false값이 잘 넘어가서 출력되는것을 확인할 수 있었습니다.    
        코드부분 발췌 :     
        

```
# 1. statefulwidget으로 구성함   
class FirstPage extends StatefulWidget { 
  @override
  _FirstPageState createState() => _FirstPageState(); // 상태 객체를 생성
}
class _FirstPageState extends State<FirstPage> { // 상태 객체를 정의
    onPressed: () {
        print("is_cat: $is_cat"); // 현재 is_cat 값을 콘솔에 출력
        setState(() {
            is_cat = false; // is_cat 값을 false로 설정
     });
### 이부분에서 setState로 state객체를 관리해주신 점이 인상적이었습니다.

#2.    
#FirstPage에서 
bool is_cat = true; // is_cat 변수를 정의하고 초기값을 true로 설정
is_cat = false; // is_cat 값을 false로 설정   
Navigator.push(
    context,
    MaterialPageRoute(
        builder: (context) => SecondPage(isCat: is_cat), // SecondPage로 이동하고 is_cat 값을 전달   
#SecondPage에서   
final bool isCat; // isCat 변수를 정의합니다.
SecondPage({required this.isCat}); // isCat 변수를 생성자에서 초기화

### 이렇게 전달받은 데이터를 잘 출력해주셨습니다.


```

- [O]  **2. 핵심적이거나 복잡하고 이해하기 어려운 부분에 작성된 설명을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭에 doc string/annotation/markdown이 달려 있는지 확인
    - 해당 코드가 무슨 기능을 하는지, 왜 그렇게 짜여진건지, 작동 메커니즘이 뭔지 기술.
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.
```
1번에서 캡쳐한 부분을 예시로 주석이 잘 달려있어서 어떤 기능을 구현하신 건지 잘 파악할 수 있었습니다.
```
        
- [O]  **3.** 에러가 난 부분을 디버깅하여 “문제를 해결한 기록”을 남겼나요? 또는
   “새로운 시도 및 추가 실험”을 해봤나요? ****
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인 또는
    - 문제에서 요구하는 조건에 더해 추가적으로 수행한 나만의 시도,
    실험이 기록되어 있는지 확인
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.   
```
기록이 특별하게 남아있지 않지만 한번에 잘 구현하셔서 없는것으로 보입니다 ^^  
```

- [O]  **4. 회고를 잘 작성했나요?**
    - 프로젝트 결과물에 대해 배운점과 아쉬운점, 느낀점 등이 상세히 기록 되어 있나요?   
```
회고가 잘 작성되어 icon에 대해 배운점이 작성되어 있었습니다.
```

- [O]  **5. 코드가 간결하고 효율적인가요?**
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 모듈화(함수화) 했는지
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.   
```
1번에서 캡쳐한 부분에서 보이듯이, 데이터를 효과적으로 전달하고, 잘 전달받아 사용하셨습니다.
```
