# Task 1: 간단한 함수 및 테스트 코드 제안 받기 (코드완성)

## Use case: 
- GitHub Copilot를 활용하여 간단한 함수와 테스트 코드를 제안받습니다. 이를 통해, GitHub Copilot이 기본적인 기능을 익히고, 어떠한 방식으로 일반적인 코딩 작업을 지원하는지 확인할 수 있습니다.

## 목표:
- 주석을 활용하여, 간단한 함수 (factorial, is_prime)를 코드완성 기능으로 작성합니다. 
- 작성한 함수에 대한 테스트 코드를 작성합니다.
- GitHub Copilot Log를 확인하여, 오픈소스와 매치되는 코드인 경우 레퍼런스 정보를 확인합니다. 
- VS Code의 Copilot 메뉴에 관한 기본적인 설정들을 변경해 봅니다.

## Step 1 : 기본 함수 작성
- VS Code를 열고, 새로운 파일을 생성합니다. (factorial.py)<br>
  <img src = "img/01.png" width = "400">

- 아래의 주석을 입력 합니다.<br>
  `# 팩토리얼 함수 `<br>
  <img src = "img/02.png" width = "400">

- 회색으로 제안된 코드를 확인하고, Tab키를 눌러서 코드를 완성합니다.<br>
   <img src = "img/03.png" width = "400">

- 제안된 코드 위에 마우스를 올려 가능한 옵션을 확인합니다.<br>
    <img src = "img/04.png" width = "400">

- 두번째로 아래 주석을 입력합니다.<br>
  `# 소수 판별 함수`<br>

- 회색으로 제안된 상태에서, (코드를 수락하지 않은 상태에서) Ctrl + Enter를 눌러서 제안되는 리스트를 확인합니다.<br>
  <img src = "img/05.png" width = "500"> <br>
  
**참고:** <br>
- 제안되는 리스트 목록을 확인하는 Ctrl + Enter 키에 변경 내용이 있어, 이를 확인하려면 아래와 같이 진행합니다. <br>
- 이렇듯, 버전 업데이트가 진행되면서, 메뉴의 위치나 기능에 변경이 발생 할 수 있습니다. <br>

- 상단의 Copilot 아이콘을 클릭하고, `Configure Code completion`을 선택합니다.<br>
<img src = "img/19.png" width = "300"> <br>
- 'Open Completions Panel'을 선택합니다.<br>
<img src = "img/20.png" width = "300"> <br>
- 단축키를 설정할 수 있습니다. <br>
- `Ctrl + Shift + P`를 눌러 명령 팔레트를 열고 '`GitHub Copilot: Open Completions Panel`' 우측의 톱니바퀴 모양을 눌러 키보드 단축키 설정으로 이동합니다.<br>
<img src = "img/22.png" width = "400"> <br>
- 왼편의 '+' 버튼을 눌러 단축키를 설정합니다.<br>
<img src = "img/23.png" width = "400"> <br> 
<img src = "img/24.png" width = "400"> <br>

## Step 2 : Copilot Log 확인하기
- VS Code 하단 터미널 창 부분의 `OUTPUT` 탭에서 `GitHub Copilot`, `GitHub Copilot Chat` 에서 Copilot 관련 로그를 확인할 수 있습니다.<br>
  <img src = "img/25.png" width = "400"> <br>
  <img src = "img/28.png" width = "600"> <br>

- GitHub Copilot 혹은 GitHub Copilot Chat 을 선택해 로그를 확인합니다. <br>
  <img src = "img/29.png" width = "400">
  <img src = "img/30.png" width = "400">

- 만약, 제안되는 코드에서 오픈소스와 매치되는 부분이 있다면, `GitHub Copilot Log(Code References)`에서 관련 로그를 볼 수 있습니다.  `// 소수 판별함수`'제안 받을 때, 이 부분에서 오픈소스의 레퍼런스 정보를 확인할 수 있습니다. <br>
- 다만, 이것은 GitHub Copilot 관리자가 오픈소스 매치되는 코드를 제안받지 않겠다고 설정하면, 로그를 볼 수 없습니다. <br>
  <img src = "img/15.png" width = "800"> <br>

## Step 3 : 오른 마우스 Copilot 메뉴 사용하기
- 마우스 오른 버튼을 클릭하여, 'Copilot' 메뉴의 'generate_test'를 선택합니다.<br>
    <img src = "img/06.png" width = "500">

- 마우스 오른 버튼을 클릭하여 'Copilot' 메뉴의 'generate_docs'를 선택합니다.<br>
    <img src = "img/07.png" width = "500"> 
    <img src = "img/08.png" width = "500">


## Step 4 : 코드 완성 기능의 컨텍스트 이해하기
- Copilot은 코드 완성 기능을 제공하기 위해, **주석과 함수 이름을 기반으로** 컨텍스트를 이해합니다.<br>
- 또한, 현재 작성중인 파일의 커서 위치의 **전,후 데이터**와, 이 데이터와 유사한 데이터를 **오픈되어져 있는 주변의 탭**에서 찾아 컨텍스트를 이해합니다. (**Neighboring Tab**) <br>
   - 코드 완성 기능에서의 Neighboring Tab 기법을 테스트하기 위해 아래 절차데로 실습합니다. 
   - `/src` 디렉토리의 `url_tools.py`, `url.py` 파일 내용을 현재 실습하는 워크스페이스로 복사 <br>
     <img src = "img/16.png" width = "400"> <br>
     <img src = "img/17.png" width = "400"> <br>

   - 복사된 `url_utils.py` 파일은 오픈된 상태로 두고, `url.py` 파일의 마지막 라인에서 키보드의 Enter를 누르면 아래와 같이 url_tools.py의 함수가 제안됩니다.<br>   
     <img src = "img/18.png" width = "500">


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



