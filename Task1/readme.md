# Task 1: 간단한 함수 및 테스트 코드 제안 받기 (코드완성)

## Use case: 
- GitHub Copilot를 활용하여 간단한 함수와 테스트 코드를 제안받습니다. 이를 통해, GitHub Copilot이 기본적인 기능을 익히고, 어떠한 방식으로 일반적인 코딩 작업을 지원하는지 확인할 수 있습니다.

## 목표:
- 주석을 활용하여, 간단한 함수 (factorial, is_prime)를 코드완성 기능으로 작성합니다. 
- 작성한 함수에 대한 테스트 코드를 작성합니다.
- GitHub Copilot Log를 확인하여, 오픈소스와 매치되는 코드인 경우 레퍼런스 정보를 확인합니다. 
- VS Code의 Copilot 메뉴에 관한 기본적인 설정들을 변경해 봅니다.

## Step 1 : 기본 함수 작성
- VS Code를 열고, 실습을 진행할 디렉토리를 생성(Open Folder), 새로운 파일을 생성합니다. <br>
<img width="352" height="299" alt="image" src="https://github.com/user-attachments/assets/0db4f3a0-4876-457f-98ce-cdfbbefd90a2" /> <br>
- 파일을 생성 (factorial.py)<br>
  <img width="295" height="269" alt="image" src="https://github.com/user-attachments/assets/29e8a59b-9bec-4c50-a225-ac22f7f78497" />


- 아래의 주석을 입력 합니다.<br>
  `# 팩토리얼 함수 `<br>
<img width="242" height="104" alt="image" src="https://github.com/user-attachments/assets/874f68a8-0a1f-4dec-ba0f-0b1fbec31a21" /> <br>
반응이 없을시 스페이스 또는 . 을 눌러서 Copilot이 깨어나도록 해주세요

- 회색으로 제안된 코드를 확인하고, Tab키를 눌러서 코드를 완성합니다.<br>
<img width="242" height="104" alt="image" src="https://github.com/user-attachments/assets/1825fce9-3a29-49c0-a560-6780d7d3241e" />

  <br>
**참고:** <br>
- 제안되는 리스트 목록을 확인하기 위해 Github Copilot Suggestion을 단축키를 통해 설정합니다. <br>
- 버전 업데이트가 진행되면서, 메뉴의 위치나 기능에 변경이 발생 할 수 있습니다. <br>

- 상단의 Copilot 아이콘을 클릭하고, `Configure Code completion`을 선택합니다.<br>
<img width="782" height="189" alt="image" src="https://github.com/user-attachments/assets/c884e16e-88c2-4778-b350-c98da315c0ba" />

- 'Open Completions Panel'을 선택합니다.<br>
<img width="328" height="221" alt="image" src="https://github.com/user-attachments/assets/76befbaa-f8f7-400c-ba02-4ba5343d228a" />

  
- 단축키를 설정할 수 있습니다. <br>
- `Ctrl + Shift + P`를 눌러 명령 팔레트를 열고 '`GitHub Copilot: Open Completions Panel`' 우측의 톱니바퀴 모양을 눌러 키보드 단축키 설정으로 이동합니다.<br>
<img width="535" height="199" alt="image" src="https://github.com/user-attachments/assets/440ec41c-0e76-495e-9038-d565f9be6bcc" />


- 왼편의 '+' 버튼을 눌러 단축키를 설정합니다.<br>
<img width="417" height="72" alt="image" src="https://github.com/user-attachments/assets/9601fd87-b9f9-48ec-96e4-5651cb33b75b" />

- 이어서, factorial.py 코드에서 두번째로 아래 주석을 입력합니다.<br>
  `# 소수 판별 함수`<br>

- (코드를 수락하지 않은 상태에서) Ctrl + Enter를 눌러서 제안되는 리스트를 확인합니다.<br>
  <img width="668" height="289" alt="image" src="https://github.com/user-attachments/assets/d415a422-5cea-41db-bb2b-39fc4d8629aa" />
- Accept Suggestions n을 선택하여 반영합니다.
- 파이썬 코드 동작하는지 수행해봅니다. <br>
<img width="636" height="358" alt="image" src="https://github.com/user-attachments/assets/cab1300f-d06c-49a6-af58-54a65d0968dc" />

## Step 2 : Copilot Log 확인하기
- VS Code 하단 터미널 창 부분의 `OUTPUT` 탭에서 `GitHub Copilot`, `GitHub Copilot Chat` 에서 Copilot 관련 로그를 확인할 수 있습니다.<br>
<img width="700" height="201" alt="image" src="https://github.com/user-attachments/assets/eaea1b10-a087-448a-9a3a-c29527dc5a59" />


- GitHub Copilot 혹은 GitHub Copilot Chat 을 선택해 로그를 확인합니다. <br>
<img width="749" height="201" alt="image" src="https://github.com/user-attachments/assets/0540ccc8-4710-48f6-8a46-f376d4fd33e3" />
<img width="749" height="200" alt="image" src="https://github.com/user-attachments/assets/36f08e92-839a-4e3a-8b9d-78344423f86d" />


- 만약, 제안되는 코드에서 오픈소스와 매치되는 부분이 있다면, `GitHub Copilot Log(Code References)`에서 관련 로그를 볼 수 있습니다.  `// 소수 판별함수`'제안 받을 때, 이 부분에서 오픈소스의 레퍼런스 정보를 확인할 수 있습니다. <br>
- 다만, 이것은 GitHub Copilot 관리자가 오픈소스 매치되는 코드를 제안받지 않겠다고 설정하면, 로그를 볼 수 없습니다. <br>
<img width="700" height="1168" alt="image" src="https://github.com/user-attachments/assets/2a829dd5-e75b-4a71-a5a5-9a744d2973f1" />


## Step 3 : 오른 마우스 Copilot 메뉴 사용하기
- 마우스 오른 버튼을 클릭하여, 'Generate Code' 메뉴의 'generate_test'를 선택합니다.<br>
<img width="500" height="558" alt="image" src="https://github.com/user-attachments/assets/777619a0-381d-4e24-b34a-ec0c867656c3" /> <br>
- 테스트 수행할수 있는 스크립트를 자동 생성해줍니다.<br>
<img width="700" height="415" alt="image" src="https://github.com/user-attachments/assets/7c0ebe1d-4253-4223-affa-bf6f56996fd5" /> <br>
-동작 정상 확인 <br>
<img width="700" height="707" alt="image" src="https://github.com/user-attachments/assets/a60d8769-29e9-4b6b-ad53-ed843dc618a6" /><br>


- 마우스 오른 버튼을 클릭하여 'Generate Code' 메뉴의 'generate_docs'를 선택합니다.<br>
주석이 생긴것을 확인하고 Accept! <br>
<img width="442" height="463" alt="image" src="https://github.com/user-attachments/assets/747e48fe-fa66-4fcf-a8dc-5068a2c5ae04" /> <br>



## Step 4 : 코드 완성 기능의 컨텍스트 이해하기
- Copilot은 코드 완성 기능을 제공하기 위해, **주석과 함수 이름을 기반으로** 컨텍스트를 이해합니다.<br>
- 또한, 현재 작성중인 파일의 커서 위치의 **전,후 데이터**와, 이 데이터와 유사한 데이터를 **오픈되어져 있는 주변의 탭**에서 찾아 컨텍스트를 이해합니다. (**Neighboring Tab**) <br>
   - 코드 완성 기능에서의 Neighboring Tab 기법을 테스트하기 위해 아래 절차데로 실습합니다. 
   - `/src` 디렉토리의 `url_tools.py`, `url.py` 파일 내용을 현재 실습하는 워크스페이스로 복사 <br>
     <img width="605" height="243" alt="image" src="https://github.com/user-attachments/assets/15a09539-1f3e-4e1c-90ae-29758d735517" />  <br>
     <img width="462" height="413" alt="image" src="https://github.com/user-attachments/assets/b74d77b7-6470-45ea-9758-351e9206fe77" /> <br>

   - 복사된 `url_utils.py` 파일은 오픈된 상태로 두고, `url.py` 파일의 마지막 라인에서 키보드의 Enter를 누르면 아래와 같이 url_tools.py의 함수가 제안됩니다.<br>   
     <img width="642" height="370" alt="image" src="https://github.com/user-attachments/assets/3e71e41d-c92b-4b24-8a2d-2607a5c352e8" />



## Step 5 : VS Code의 Copilot 설정 메뉴
- VS Code에서 Ctrl + Shift + P를 눌러 명령 팔레트를 열고, 'preference'을 검색하여, `Preference: Open Settings (UI)`를 선택합니다.<br>
    <img src = "img/09.png" width = "500">
- Copilot locale을 검색하고, 'ko'로 변경합니다.<br>
    <img src = "img/10.png" width = "500">

- Code완성 기능의 기본 모델을 변경해 봅니다.<br>
  - 상단의 Copilot 아이콘을 클릭하고, `Configure Code completion`을 선택합니다.<br>
    <img src = "img/11.png" width = "400">
  - 'Change completion model'을 선택합니다.<br>
    <img src = "img/12.png" width = "400">
  - 모델을 변경합니다.<br>
    <img src = "img/13.png" width = "400">

- Experimental 기능인 `NES(Next Edit Suggestion)`을 활성화/비활성화 해봅니다.<br>
    <img src = "img/14.png" width = "400">

- Reference : [VS Code Copilot settings reference 문서](https://code.visualstudio.com/docs/copilot/copilot-settings)


## 참고 : Copilot 관련 기술 지원
- [GitHub 도움말 : Troubleshoot GitHub Copilot 문서 참조](https://docs.github.com/en/enterprise-cloud@latest/copilot/how-tos/troubleshoot)

- (기업 관리자)각종 에러로그, 화면 캡쳐 등을 첨부하여 GitHub 글로벌 Support에 기술지원 요청/문의할 수 있습니다. <br>
  - [GitHub Support](https://support.github.com)

## 지식 확인
- GitHub Copilot의 코드 완성 기능
- 코드완성 기능의 모델 선택
- GitHub Copilot의 코드 완성 기능의 컨텍스트
- VS Code의 Copilot 설정 메뉴



