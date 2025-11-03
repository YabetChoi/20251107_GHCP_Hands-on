# Task 2: 가위, 바위, 보 게임 만들기 (Copilot Chat사용)

## Use case: 
- GitHub Copilot를 활용하여 가위, 바위, 보 게임을 만들고, 기본 게임에 추가적인 게임 로직을 추가하는 실습을 통해, Copilot의 활용도를 높입니다.

## 목표:
- Python으로 가위, 바위, 보 게임을 만듭니다.
- 게임을 실행하고 게임 결과를 출력합니다.
- 기본적인 가위, 바위, 보 게임 외에, Lizard, Spock 등의 확장판 게임을 추가합니다.
- Copilot Chat의 `Vision` 기능을 활용하여, 그림파일을 붙여넣기 하고, 이를 기반으로 코드를 제안받아 봅니다.
- Copilot Chat의 `Review and Comment` 기능을 활용하여, 코드에 대한 리뷰를 받아 봅니다.
- `Review and Comment`에 Custom instruction을 제공하여, 원하는 형태로 리뷰를 받아 봅니다.

## Step 1: 가위, 바위, 보 게임 만들기
- Copilot Chat을 이용하여, 가위, 바위, 보 게임을 만들 수 있는 코드를 요청합니다.
- 사용자가 가위,바위,보 중 하나를 선택하고, 컴퓨터와 대결하는 로직을 추가합니다.
- 사용자가 선택한 가위, 바위, 보와 컴퓨터의 선택을 비교하여 승패를 결정하는 로직을 추가합니다.
- 사용자가 게임을 계속할 것인지 종료할 것인지 선택할 수 있는 로직을 추가합니다.<br><br>
- 먼저 "가위바위보.py" 새파일을 만듭니다.<br>
<img width="269" height="253" alt="image" src="https://github.com/user-attachments/assets/9252f597-1df4-4449-ac6c-19fc0ca0c958" /><br>

- Copilot Chat을 실행합니다. <br>
   <img width="907" height="263" alt="image" src="https://github.com/user-attachments/assets/9b2f1c9d-1f5c-49b0-a5a2-a38d1b77ec3f" /><br>
- 예시 문구) <br>
가위,바위, 보 게임을 만든다. 사용자가 가위,바위,보 중 하나를 선택하고, 컴퓨터는 무작위로 선택한다.
사용자의 선택과 컴퓨터의 선택을 비교하여 승패를 결정한다. 사용자가 이기면 "You Win!", 컴퓨터가 이기면 "You lose", 비기면 "Its a tie!"를 출력한다. 사용자가 "exit"를 입력하면 게임을 종료한다.<br>
<img width="650" height="657" alt="image" src="https://github.com/user-attachments/assets/7bb0e676-2759-44f3-aa06-a89c49254deb" /> <br>
- 생성한 코드를 삽입합니다. <br>
<img width="192" height="128" alt="image" src="https://github.com/user-attachments/assets/ae15f102-aedf-4a13-b930-3f932cc69310" /> <br>
<img width="486" height="646" alt="image" src="https://github.com/user-attachments/assets/f523eec2-e86d-4079-bbc7-95e94d50b00a" /> <br>


- 게임을 실행하고, 게임 결과를 출력 받아 봅니다.<br>
  <img width="817" height="218" alt="image" src="https://github.com/user-attachments/assets/52fde1c8-e681-43ed-8cd6-58e000cc5bef" /><br>
- Copilot Chat과 동일하게, **Inline Chat** 모드를 실행해보겠습니다.<br>
가위바위보.py 코드에서 일부 영역을 선택하고  `Ctrl + I` 버튼을 눌러봅니다.<br>
<img width="324" height="245" alt="image" src="https://github.com/user-attachments/assets/c7cda2df-e798-4fc6-92b3-69ae26084024" /><br>
선택된 코드에 대한 설명을 요청하거나, 코드를 수정해달라고 요청할수 있습니다. `while이 왜 쓰여지는거니?`<br>
<img width="301" height="365" alt="image" src="https://github.com/user-attachments/assets/108c8007-3ea4-456c-b7d9-c5b9bc1dea84" /><br>
Copilot Chat과 마찬가지로, Chat에서 제안받을 LLM 모델을 선택할수 있습니다.<br>
<img width="150" height="295" alt="image" src="https://github.com/user-attachments/assets/aea9c471-5b29-4789-922a-12310f1f9702" /><br>




## Step 2 : Lizard, Spock 추가하기
- 만들어진 게임에 추가로 Lizard, Spock의 로직을 Copilot을 활용하여 추가합니다.<br>
   <img width="640" height="597" alt="image" src="https://github.com/user-attachments/assets/f48ab55c-8f55-4fda-b075-37a5c0cb21d9" /> <br>

- Copilot Chat에 위 그림파일을 복사하여 Copilot Chat에 붙여넣기 합니다.<br>
    <img width="541" height="512" alt="image" src="https://github.com/user-attachments/assets/309c92b7-4c0c-4e80-8baa-6483923a3d08" /><br>
    <img width="100" src="https://github.com/user-attachments/assets/2958ec6e-3c20-425f-b21d-f9b6cd82cf4b" /><br>

- Copilot Chat에 붙여넣기 한 그림파일 'Pasted Image'가 있음을 확인합니다.<br>
    <img width="198" height="99" alt="image" src="https://github.com/user-attachments/assets/a0638f2d-15cd-42d9-8b8d-292185e34d9d" /><br>

- Copilot Chat에 `그림파일데로 Lizard, Spock을 추가해 주세요` 라고 요청합니다.<br>
    <img width="192" height="47" alt="image" src="https://github.com/user-attachments/assets/fdfdc381-370c-4b36-b541-c78c1f3e9778" /><br>

- Copilot Chat에서 제안된 코드를 확인합니다.<br>
    <img width="475" height="715" alt="image" src="https://github.com/user-attachments/assets/c8a3b9b5-1fde-49d7-887f-b705f57822d6" /><br>

- Copilot Chat에서 `Apply to file` 버튼을 클릭하여, 제안된 코드를 적용합니다.<br>
    <img width="147" height="43" alt="image" src="https://github.com/user-attachments/assets/38480cdf-bdc6-4a3d-9f61-f1763a0a0675" /> <br>

- 필요시 미진한 코드를 추가하고 실행해 봅니다. 간단하게 줄여달라 요청해봅니다.<br>
<img width="470" height="235" alt="image" src="https://github.com/user-attachments/assets/4b792eef-e61e-4cab-acd3-58f8a5d9e148" /> <br>
    <img width="436" height="218" alt="image" src="https://github.com/user-attachments/assets/c0135804-8c10-4c4c-b7c3-b1f3ccb00fcb" /> <br>

## Step 3: Code Review 사용해 보기
- 마우스 오른 버튼을 클릭하여, `Generate Code` /  `Review` 기능을 사용하여, 코드에 대한 리뷰를 받아 봅니다.<br>
    <img width="552" height="753" alt="image" src="https://github.com/user-attachments/assets/36228fca-a108-4496-b5f6-079a7d879e5f" /><br>
    - 제안된 코드를 적용해봅니다. <br>
    <img width="539" height="380" alt="image" src="https://github.com/user-attachments/assets/d22dafac-da1c-4f9d-bf8b-8d2cad280fe9" /><br>

- 코딩 규칙을 추가한후 Review를 다시 받아보겠습니다. (`Custom instruction` 추가)<br>
- 아래 절차데로 Custom instructions을 설정해 봅니다.<br>
  - Ctrl + Shift + P를 눌러서 명령 팔레트를 엽니다.<br>
  - `Workspace settings(JSON)`을 선택합니다.<br>
    <img width="445" height="127" alt="image" src="https://github.com/user-attachments/assets/f1a94015-eb25-4995-969f-4a4dc6c02280" /> <br>

  - 설정 JSON 파일을 열고, 'github.copilot.chat.codeGeneration.instructions' 을 설정해봅니다.<br>
  <img width="363" height="87" alt="image" src="https://github.com/user-attachments/assets/3af6ea94-7a6f-4141-96ad-5bb6af790837" /> <br>
    <img width="486" height="230" alt="image" src="https://github.com/user-attachments/assets/bc0ea122-af20-4c8c-87fd-bba89c2e4dc5" /> <br>
`{
  "github.copilot.chat.codeGeneration.instructions": [
    {
      "text": "함수의 이름은 '_'로 시작하고, 변수 네이밍 규칙과 동일하게 작성합니다. 클래스와 생성자의 이름은 파스칼케이스(PascalCase)를 사용합니다. 들여쓰기는 스페이스 2개로 한다."
    }
  ]
}`

   - 다시 한번 `Code Review` 기능을 사용하여, 코드에 대한 리뷰를 받아 봅니다.<br>
   <img width="495" height="418" alt="image" src="https://github.com/user-attachments/assets/969bfe07-71c9-4263-aeaf-4cfb09c31445" /> <br>

## 지식 확인:
- 코드 완성 기능과, Copilot Chat 기능의 차이점
- Vision 기능으로 가능한 다른 활용법
- Copilot Chat의 `Code Review` 기능과 custom instruction을 활용하여, 원하는 형태로 리뷰를 받아 보는 방법
