# AIFFEL Campus Code Peer Review Templete
- 코더 : 김소영
- 리뷰어 : 김원영


# PRT(Peer Review Template)
[O]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
- 문제에서 요구하는 기능이 정상적으로 작동하는지? (요구하는 기능들이 정상적으로 잘 작동합니다)
    - 해당 조건을 만족하는 부분의 코드 및 결과물을 근거로 첨부
  
츨력결과 예시
계산기 프로그램을 시작하겠습니다.
첫번째 숫자를 입력해 주세요.2
연산자를 입력해 주세요. (+,-,*,/,** 연산자만 가능)+
두번째 숫자를 입력해 주세요.1
2 + 1 = 3
계속하시겠습니까?(Y/N)
    
[O]  **2. 핵심적이거나 복잡하고 이해하기 어려운 부분에 작성된 설명을 보고 해당 코드가 잘 이해되었나요?**
- 해당 코드 블럭에 doc string/annotation/markdown이 달려 있는지 확인 (Confirmed)
- 해당 코드가 무슨 기능을 하는지, 왜 그렇게 짜여진건지, 작동 메커니즘이 뭔지 기술. (Confirmed, 화면 공유를 통해 키 코드들의 기능과 역할에 대해 자세하게 설명해 주셨습니다)
- 주석을 보고 코드 이해가 잘 되었는지 확인 (Confirmed, 하기에 부연 설명)
   - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.
  (가독성을 위해 그리고 오류 발생시 수정의 편리함을 위해서 각 코딩의 구조를 세분화였고 해당 코드가 어떤 위치에서 어떤 목적으로 사용되었는지 주석을 통해 자세하게 구현하였습니다)
  
  실제 계산은 calculator 함수에서 전담
  result = calculator(first, operator, second)

  ZeroDivisionError 상황에 대한 처리
  if result == "ZeroDivisionError":
    print("0으로 나눌 수 없습니다. 다시 입력해 주세요.")
    continue

  계산 결과 출력
  print(first, operator, second, "=", result)

  is_continue = input("계속하시겠습니까?(Y/N)").lower()
  if is_continue != 'y':
    print("계산기를 종료하겠습니다.")
    break
        
[O]  **3. 에러가 난 부분을 디버깅하여 “문제를 해결한 기록”을 남겼나요? 또는 “새로운 시도 및 추가 실험”을 해봤나요?**
- 문제 원인 및 해결 과정을 잘 기록하였는지 확인 (Confirmed, 화면 공유를 통한 상세한 설명과 결과값 실행연습을 통해서 일부 오류 확인 후에도 수정을 진행하며 잘 해결하였습니다)
- 문제에서 요구하는 조건에 더해 추가적으로 수행한 나만의 시도, 실험이 기록되어 있는지 확인
    - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
 회고 참조 상단 본문 중....

 김소영 

 예를 들어, #메인프로그램 ~ 쉬운 프로그램이 됐다.
        
[O]  **4. 회고를 잘 작성했나요?**
- 프로젝트 결과물에 대해 배운점과 아쉬운점, 느낀점 등이 상세히 기록 되어 있나요? (Confirmed, 상세히 잘 기록되어있습니다)
	- 딥러닝 모델의 경우, 인풋이 들어가 최종적으로 아웃풋이 나오기까지의 전체 흐름을 도식화하여 모델 아키텍쳐에 대한 이해를 돕고 있는지 확인


# 참고 링크 및 코드 개선
```
# 코드 리뷰 시 참고한 링크가 있다면 링크와 간략한 설명을 첨부합니다.
# 코드 리뷰를 통해 개선한 코드가 있다면 코드와 간략한 설명을 첨부합니다.
```
