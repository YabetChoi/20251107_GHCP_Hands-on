# Task 4: MCP
## MCP 를 활용한 AI Agent 만들기
- Copilot Chat 를 엽니다. <br>
<img width="260" height="130" alt="image" src="https://github.com/user-attachments/assets/a902531e-ca2b-42cd-9d85-13e0cb8e16aa" /><br>
- Copilot Chat에 아래 Prompt 를 입력합니다.
    ```bash
    파이썬 코드로, Microsoft Learn MCP 서버를 이용하는 AI Agent 를 만들거야.
    AI Agent 는 입력을 사용자에게 받아서 Azure OpenAI 모델에게 답변을 generation 해달라고 요청할거야.
    Azure OpenAI 모델은 MCP 의 도구들을 이용해서 주어진 질문에 필요한 context 를 받아와 최종 답변을 생성해야해.
    MCP 서버와 연결할때는 MCP Python SDK 를 사용해줘.

    [Microsoft Learn MCP Server 상세]
    사용할 Microsoft Learn MCP 서버에 대한 상세는 다음과 같아.
    - Github 문서: https://learn.microsoft.com/api/mcp
    - MCP 서버 endpoint: https://learn.microsoft.com/api/mcp

    [MCP Python SDK]
    MCP Python SDK 사용 Github 은 https://github.com/modelcontextprotocol/python-sdk 여기야. 코드 구현시 참고해.

    [AzureOpenAI 사용 가이드]
    - 사용할 환경 변수는 아래와 같아.
    -- AZURE_OPENAI_ENDPOINT="https://yb-kor1.cognitiveservices.azure.com/" 
    -- AZURE_OPENAI_API_KEY="92GIEd0hxEU0NGlpiKunk2ZlFdbzQJWzo1K05qo2lmThFD3hLDqyJQQJ99BIACNns7RXJ3w3AAAAACOGmjUy"
    -- AZURE_OPENAI_DEPLOYMENT="gpt-4.1-mini"
    -- api_version = "2024-12-01-preview"
    - AzureOpenAI.chat.completions.create() 함수의 tools argument 를 통해 MCP Server 의 도구들을 LLM 에게 전달해야해.
    - 이는 OpenAI 에서 제공하는 Function Calling 방식이야.

    [코드 구현시 주의사항]
    - Request 시에 Content-Type은 application/json으로 설정하고,
    - 꼭 Request json 에 "jsonrpc": "2.0" 필드를 포함해야 해.
    ```
    <img width="214" height="512" alt="Screenshot 2025-11-03 at 12 16 49 PM" src="https://github.com/user-attachments/assets/c1abd9c6-319b-4c6c-b35f-e71ed7baa004" />
- Planning 이나 몇번의 Task 를 수행하고 나서 아래와 같이 Workspace 가 생성된다. 버그가 있다면 Chat 을 통해 수정하고, Chat 이 가이드한 실행 명령어를 통해 AI Agent 를 실행해보자. <br>
    <img width="439" height="225" alt="Screenshot 2025-11-03 at 12 24 44 PM" src="https://github.com/user-attachments/assets/e1102780-dbef-41fa-972e-501d0055d454" />
- AI Agent 의 Input line 에 아래 질문을 물어보자.
    ```bash
    You> Azure OpenAI 에서 RBAC 은 어떤게 필요해 ?
    ```
    그러면 AI Agent 가 다음과 같이 답변한다.
    <img width="1394" height="280" alt="Screenshot 2025-11-03 at 12 27 47 PM" src="https://github.com/user-attachments/assets/e4008742-b9ea-461a-9477-695ca7bd6e4b" />
