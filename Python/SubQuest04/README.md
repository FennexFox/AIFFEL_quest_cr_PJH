# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 박정현
- 리뷰어 : 윤형석


# PRT(Peer Review Template)
- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
        ```python
            # 입력받은 정수에 대한 계산식
            first_num = int(first_num)
            second_num = int(second_num)
            operator_dict = {"+": lambda x, y: x + y, "-": lambda x, y: x - y, "*": lambda x, y: x * y, "/": lambda x, y: x / y, "**": lambda x, y: math.pow(x, y)}
            operator = operator_dict[operator_input]
            res = operator(first_num, second_num)
            print(f'계산 결과: {res}')
        ```
    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
        ```python
            """
            OperatorError Class
            - Except 클래스를 상속받는 클래스.
            - 지원하지 않는 연산자에 대한 예외 처리를 위해 사용됩니다.
            """
            class OperatorError(Exception):
                pass
        ```
        - 해당 클래스의 선언 목적은 이해하였으나, 구현 없이 비어있는 이유를 이해하지 못하였음
        - 확인 결과, 구현은 범위 바깥이라 생략하였다는 것을 알게 됨

        ```python
            # 입력받은 정수에 대한 계산식
            first_num = int(first_num)
            second_num = int(second_num)
            operator_dict = {"+": lambda x, y: x + y, "-": lambda x, y: x - y, "*": lambda x, y: x * y, "/": lambda x, y: x / y, "**": lambda x, y: math.pow(x, y)}
            operator = operator_dict[operator_input]
            res = operator(first_num, second_num)
            print(f'계산 결과: {res}')
        ```
        - lambda 표현식과 dictionary 구조를 중첩 사용하여 if-else 구문 없이 한 줄로 구현한 점이 탁월함
        - 그러나 그 원리와 과정에 대한 주석이 작성되지 않아 이해하기 위한 노력이 필요함
        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 에러 핸들링 과정에서 디버깅 작업을 수행함
        
- [ ]  **4. 회고를 잘 작성했나요?**
    - 
        
- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였음
    - 에러 핸들링 관련한 차후 기능 구현을 위해 클래스를 미리 작성하여 적응성을 높임


# 회고(참고 링크 및 코드 개선)
```
# 세상에 람다와 딕셔너리를 저렇게 사용하다니
```
