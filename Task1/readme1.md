# Task 1: 간단한 함수 코드 작성하기 (Code 완성 기능 사용)

## 📋 개요

### Use case
GitHub Copilot를 활용하여 간단한 함수와 테스트 코드를 제안받습니다. 이를 통해 GitHub Copilot의 기본적인 기능을 익히고, 일반적인 코딩 작업을 어떻게 지원하는지 확인할 수 있습니다.

### 목표
- 주석을 활용하여 간단한 함수 (factorial, is_prime)를 코드완성 기능으로 작성
- 작성한 함수에 대한 테스트 코드 작성
- GitHub Copilot Log를 확인하여 오픈소스와 매치되는 코드의 레퍼런스 정보 확인
- VS Code의 Copilot 메뉴 기본 설정들을 변경

---

## 🚀 Step 1: 기본 함수 작성

### 1.1 작업 환경 설정

1. **VS Code 실행 및 디렉토리 열기**
   - VS Code 실행
   - `File > Open Folder` 선택
   
   ![VS Code 폴더 열기](https://github.com/user-attachments/assets/0db4f3a0-4876-457f-98ce-cdfbbefd90a2)

2. **작업 디렉토리 생성**
   - 작업 디렉토리 `1107-ghcp` 폴더 생성
   
   ![작업 디렉토리](https://github.com/user-attachments/assets/fb4f0a2b-a5b2-4ea0-92c8-393056d3c5df)

### 1.2 팩토리얼 함수 작성

1. **새 파일 생성**
   - Explorer에서 New File 아이콘 클릭
   - 파일명: `factorial.py`
   
   ![새 파일 생성](https://github.com/user-attachments/assets/29e8a59b-9bec-4c50-a225-ac22f7f78497)

2. **함수 작성**
   ```python
   # 팩토리얼 함수
   ```
   - 주석 입력 후 엔터
   - GitHub Copilot이 함수를 제안하면 Tab키로 수락
   
   ![코드 제안](https://github.com/user-attachments/assets/874f68a8-0a1f-4dec-ba0f-0b1fbec31a21)

   > 💡 **팁**: 반응이 없다면 스페이스나 `.`을 눌러 Copilot을 활성화하세요.

### 1.3 Copilot Suggestions 패널 설정

1. **단축키 설정**
   - `Ctrl + Shift + P`로 명령 팔레트 열기
   - `GitHub Copilot: Open Completions Panel` 입력
   - 설정(톱니바퀴) 클릭
   
   ![명령 팔레트](https://github.com/user-attachments/assets/440ec41c-0e76-495e-9038-d565f9be6bcc)

2. **단축키 지정**
   - `+` 버튼 클릭하여 `Ctrl+Enter` 설정
   
   ![단축키 설정](https://github.com/user-attachments/assets/9601fd87-b9f9-48ec-96e4-5651cb33b75b)

### 1.4 소수 판별 함수 추가

1. **함수 추가**
   ```python
   # 소수 판별 함수
   ```
   - 주석 입력 후 엔터
   - `Ctrl + Enter`로 제안 리스트 확인
   
   ![제안 리스트](https://github.com/user-attachments/assets/d415a422-5cea-41db-bb2b-39fc4d8629aa)

2. **코드 실행 테스트**
   - 상단 실행 버튼 클릭
   - 하단 터미널에서 결과 확인
   
   ![코드 실행](https://github.com/user-attachments/assets/cab1300f-d06c-49a6-af58-54a65d0968dc)

---

## 📊 Step 2: Copilot Log 확인하기

### 2.1 로그 확인 방법

1. **OUTPUT 탭 이동**
   - VS Code 하단 터미널 창의 `OUTPUT` 탭 선택
   - 우측 메뉴에서 `GitHub Copilot` 또는 `GitHub Copilot Chat` 선택
   
   ![로그 확인](https://github.com/user-attachments/assets/eaea1b10-a087-448a-9a3a-c29527dc5a59)

### 2.2 Code References 확인

- 오픈소스와 매칭되는 코드가 있을 경우 `GitHub Copilot Log(Code References)`에서 확인 가능
- 관리자 설정에 따라 매칭 코드 제안이 비활성화될 수 있음

![Code References 예시](https://github.com/user-attachments/assets/2a829dd5-e75b-4a71-a5a5-9a744d2973f1)

---

## 🖱️ Step 3: 우클릭 Copilot 메뉴 사용하기

### 3.1 테스트 코드 생성

1. **Generate Test 사용**
   - 소스코드 선택 후 우클릭
   - `Generate Code` > `generate_test` 선택
   
   ![Generate Test](https://github.com/user-attachments/assets/777619a0-381d-4e24-b34a-ec0c867656c3)

2. **테스트 코드 확인**
   - 자동 생성된 테스트 스크립트 확인
   - 동작 테스트 수행
   
   ![테스트 결과](https://github.com/user-attachments/assets/a60d8769-29e9-4b6b-ad53-ed843dc618a6)

### 3.2 문서 생성

- 우클릭 > `Generate Code` > `generate_docs` 선택
- 자동 생성된 주석 확인 후 Accept

![문서 생성](https://github.com/user-attachments/assets/747e48fe-fa66-4fcf-a8dc-5068a2c5ae04)

---

## 🧠 Step 4: 코드 완성 기능 동작 메커니즘 이해하기

### 4.1 컨텍스트 이해 방식

GitHub Copilot은 다음을 기반으로 컨텍스트를 이해합니다:
- **주석과 함수 이름**
- **커서 위치의 전후 데이터**
- **열려있는 주변 탭의 유사한 데이터** (Neighboring Tab)

### 4.2 Neighboring Tab 기법 테스트

1. **파일 준비**
   - `url_tools.py` 파일 생성:
   
   ![url_tools.py](https://github.com/user-attachments/assets/b74d77b7-6470-45ea-9758-351e9206fe77)

   - `url.py` 파일 생성:
   
   ![url.py](https://github.com/user-attachments/assets/15a09539-1f3e-4e1c-90ae-29758d735517)

2. **테스트 수행**
   - `url_utils.py` 파일을 열어둔 상태에서
   - `url.py` 파일 마지막 라인에서 Enter
   - url_tools.py의 함수가 제안되는 것을 확인
   
   ![Neighboring Tab 효과](https://github.com/user-attachments/assets/3e71e41d-c92b-4b24-8a2d-2607a5c352e8)

---

## ⚙️ Step 5: VS Code의 Copilot 설정 메뉴

### 5.1 언어 설정 변경

1. **설정 열기**
   - `Ctrl + Shift + P` → `Preference: Open Settings (UI)` 선택
   
   ![설정 열기](https://github.com/user-attachments/assets/3b23d8ae-82c2-430c-8b77-3481cb5f6f94)

2. **로케일 변경**
   - `Copilot locale` 검색
   - 'ko'로 변경
   
   ![로케일 설정](https://github.com/user-attachments/assets/cefdec05-ec30-483b-92a2-2b79e4813373)

### 5.2 NES(Next Edit Suggestion) 기능 설정

- `copilot next edit` 검색
- 활성화/비활성화 조정 (기본값: Enable)

![NES 설정](https://github.com/user-attachments/assets/4425799a-bd33-41dc-a9ef-3716ce78e163)

### 5.3 LLM 모델 변경

1. **모델 설정 접근**
   - Copilot 아이콘 우측 화살표 클릭
   - `Configure Code completion` 선택
   
   ![모델 설정](https://github.com/user-attachments/assets/8a3dc99c-4df5-477e-96cf-63026e795288)

2. **모델 변경**
   - `Change completion model` 선택
   - 사용 가능한 모델 중 선택
   
   ![모델 선택](https://github.com/user-attachments/assets/2428ed67-8542-4d8d-951e-d1ab01fbea4f)

---

## 📚 참고 자료

### 기술 문서
- [VS Code Copilot settings reference](https://code.visualstudio.com/docs/copilot/copilot-settings)

### 기술 지원
- [GitHub 도움말: Troubleshoot GitHub Copilot](https://docs.github.com/en/enterprise-cloud@latest/copilot/how-tos/troubleshoot)
- [GitHub Support](https://support.github.com) (기업 관리자용)

---

## ✅ 지식 확인 체크리스트

- [ ] GitHub Copilot의 코드 완성 기능 이해
- [ ] 코드완성 기능의 모델 선택 방법
- [ ] GitHub Copilot의 컨텍스트 이해 메커니즘
- [ ] VS Code의 Copilot 설정 메뉴 활용법