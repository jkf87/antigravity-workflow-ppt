---
name: create_academic_ppt
description: 학술 그림 스타일 이미지를 포함하는 PowerPoint 프레젠테이션을 생성합니다. /create_academic_ppt [주제]
---

1.  **주제 이해**:
    *   슬래시 명령 인수에 제공된 주제를 식별합니다.
    *   주제가 제공되지 않은 경우 사용자에게 "어떤 주제에 대한 프레젠테이션을 만들고 싶으신가요?"라고 묻고 응답을 기다립니다.

2.  **콘텐츠 생성 (JSON)**:
    *   주제를 기반으로 5개의 슬라이드에 대한 JSON 구조를 생성합니다.
    *   각 슬라이드는 다음을 포함해야 합니다:
        *   `title`: 전문적인 제목.
        *   `content`: 주요 글머리 기호.
        *   `image_prompt`: AI 이미지 생성기를 위한 상세 설명. **스타일**: "학술 그림, IEEE/CVPR 논문 스타일, 개략도, 깔끔한 선, 흰색 배경".
    *   이 JSON 콘텐츠를 `slides.json`이라는 파일에 저장합니다.

3.  **PPT 생성**:
    *   생성된 JSON 파일을 사용하여 파이썬 스크립트를 실행합니다.
    *   명령어: `python generate_ppt.py`

4.  **정리**:
    *   출력 파일 이름 (`nano_banana_presentation.pptx`)을 사용자에게 알려줍니다.