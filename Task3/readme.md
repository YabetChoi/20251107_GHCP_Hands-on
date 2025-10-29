# Task 3: 나만의 음성비서 앱만들기 (AI 및 LLM활용)
- 간단한 채팅 앱을 로컬에서 생성하고 기동해봅니다.
- 채팅앱에 생성형 LLM을 통해 답변을 받도록 기능을 추가합니다.
- 음성 인식 기능과 음성 출력 기능을 추가합니다.

## 1) 로컬에서 간단한 웹앱을 생성 합니다.
- Copilot Chat 를 엽니다. <br>
<img width="260" height="130" alt="image" src="https://github.com/user-attachments/assets/a902531e-ca2b-42cd-9d85-13e0cb8e16aa" /><br>
- 간단한 파이썬 웹앱 코드를 생성해달라고 Copilot Chat에 입력합니다. <br>
`파이썬 코드로, 내 랩탑에서 웹화면을 띄워주는 코드를 만들어주고, 상단에는 사용자 Input을 받고 아래는 send 버튼을 만들어줘` <br>
<img width="382" height="51" alt="image" src="https://github.com/user-attachments/assets/f45b1c23-6468-4181-8868-100ee1e66827" /><br>
<img width="392" height="431" alt="image" src="https://github.com/user-attachments/assets/be1ffc8f-dff6-420b-95bc-ca3bfef24826" /> <br>
- Create Workspace를 클릭합니다. <br>
(결과가 다르더라도 Copilot Chat과 질문/답변하며 파일을 수동으로 생성할수도 있습니다)
- 신규 폴더를 내 랩탑의 적절한 위치에 "my-web-app" 이름으로 생성합니다. <br>
<img width="471" height="183" alt="image" src="https://github.com/user-attachments/assets/a54bb6c3-f6b6-4e55-8d9d-39ce97ba32f2" /> <br>
- 생성한 Workspace가 생성되고, 필요한 파일들도 함께 만들어진것을 확인합니다. <br>
app.py, index.html등 <br>
<img width="264" height="374" alt="image" src="https://github.com/user-attachments/assets/1de6cb26-4250-49c7-90d6-e92250d9ccc8" /> <br>
- app.py를 열어보고, 실행해봅니다.<br>
<img width="910" height="386" alt="image" src="https://github.com/user-attachments/assets/54cb6613-9260-4ffe-9734-dfb7860258ef" /> <br>
- 유사한 다른 에러가 발생했다면 필요한 조치를 Copilot Chat에 에러를 넣고 물어봅니다. <br>
<img width="560" height="242" alt="image" src="https://github.com/user-attachments/assets/99c9b487-c42b-40b9-8a34-12ff4923d1c5" /><br>
<img width="383" height="325" alt="image" src="https://github.com/user-attachments/assets/6c761286-addb-45a2-8deb-bc39842ac0ee" /> <br>
<img width="552" height="198" alt="image" src="https://github.com/user-attachments/assets/3cb241b0-ba38-4235-ad2b-e6d6b7442d4d" /> <br>
- Error Fix 후에 다시 파이선을 수행합니다. <br>
<img width="550" height="218" alt="image" src="https://github.com/user-attachments/assets/a569cc7c-716d-477e-91ba-15a3667890de" /> <br>
- 정상 동작되면서 로컬에 웹이 기동됩니다. Ctrl누른 후 URL을 클릭합니다. <br>
<img width="820" height="287" alt="image" src="https://github.com/user-attachments/assets/6f76f922-0480-4278-b880-38b11912b167" /> <br>

## 2) 채팅 기능의 강화를 위해 LLM(Chatgpt)을 연동해보겠습니다.
- Copilot Chat에 추가 보완하고자 하는 내용을 추가합니다. <br>
`예) 사용자의 Input로 부터 값을 받아서, 이 값을 Azure openAI의 gpt4.1 로 보내고 , 나온 결과를 화면 상단에 출력해주도록 코드를 추가하고 싶어. 코드는 최소한만 수정하고 간단하게 알려줘`<br>
<img width="365" height="474" alt="image" src="https://github.com/user-attachments/assets/489de208-59f9-4fc6-b7db-38c5e79142d5" /><br>
- (참고) 아래 코드 가이드 순서는 개인마다 다를수 있으며, 표준 방법을 기준으로 설명합니다.
- 필요한 Python 라이브러리를 설치합니다. <br>
<img width="380" height="73" alt="image" src="https://github.com/user-attachments/assets/79fd4772-a1f1-435a-9ea6-9bfeda4b5b92" /><br>
<img width="405" height="137" alt="image" src="https://github.com/user-attachments/assets/3ff4629b-31c2-4509-af20-8f7e92437c0b" /><br>
- Azure OpenAI API정보등을 담을 .env 파일을 생성합니다. <br>
<img width="360" height="101" alt="image" src="https://github.com/user-attachments/assets/e774a900-d7f0-43fc-ba57-a1ab349ea6da" /><br>
<img width="269" height="284" alt="image" src="https://github.com/user-attachments/assets/96fefc83-cc3e-4a95-9e8a-605364ca8b65" />
















  
