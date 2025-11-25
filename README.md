# 학술 PPT 생성기 (Academic PPT Generator)

이 도구는 Google의 Gemini API를 사용하여 학술적 스타일의 이미지가 포함된 PowerPoint 프레젠테이션을 생성합니다.

## 설정 (Setup)

1. 의존성 패키지 설치:
   ```bash
   pip install -r requirements.txt
   ```

2. API 키 설정:
   - `.env.example` 파일을 복사하여 `.env` 파일 생성
   - Google Gemini API 키를 `.env` 파일에 붙여넣기 (`API_KEY=` 접두사 없이 키 값만 입력)

## 사용법 (Usage)

1. `slides.json` 파일에 슬라이드 내용을 준비합니다.
2. 스크립트 실행:
   ```bash
   python generate_ppt.py
   ```

## 워크플로우 설정 (선택 사항)

Antigravity Workflow로 사용하려면 다음 단계를 따르세요:

1. 워크플로우 디렉토리가 없다면 생성:
   ```bash
   mkdir -p .agent/workflows
   ```

2. 워크플로우 파일 복사:
   ```bash
   cp create_academic_ppt.md .agent/workflows/
   ```

3. 사용 방법:
   - 이제 `@create_academic_ppt`를 입력하거나 에이전트에게 "학술 ppt 만들어줘"라고 요청하여 워크플로우를 사용할 수 있습니다.
   - 예시: `/create_academic_ppt [주제]`

