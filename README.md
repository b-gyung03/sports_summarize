# sports_summarize 

## 📂 스포츠 경기 요약

이 프로젝트는 Google의 Gemini AI 모델을 활용하여, 스포츠 경기 중계 이미지(스코어보드, 스탯)를 분석하고 구조화된 JSON 데이터로 요약하는 간단한 데모입니다. 

## ✨ 핵심 기능

* **멀티모달 입력:** 여러 장의 경기 관련 이미지를 동시에 입력받아 종합적으로 분석합니다.
* **다종목 분석:** 꼼꼼한 프롬프트 엔지니어링을 통해 '축구'와 '야구' 종목을 자동으로 인식하고, 각 종목에 맞는 스탯(점유율, 안타 등)을 기반으로 요약합니다.
* **안정적인 JSON 출력:** AI가 분석한 결과를, 다른 시스템에서 즉시 활용할 수 있는 깨끗한 `JSON` 형식으로 생성합니다.

## 🛠️ 사용한 기술

* **AI Model:** Google `Gemini 2.5 Flash` (Multimodal)
* **Environment:** `Python` on `Google Colab`
* **Libraries:** `google-generativeai`, `json`, `PIL`

## 🚀 실행 방법 (Google Colab)

1.  이 GitHub 리포지토리의 `.ipynb` 파일을 다운로드하여 Google Colab에서 엽니다.
2.  **[Cell 4]**을 실행하여 필요한 라이브러리를 설치하고, `YOUR_API_KEY_HERE` 부분에 본인의 Google AI Studio API 키를 입력합니다.
3.  **[Cell 7]**를 실행하고, 분석을 원하는 경기 이미지 파일(들)을 업로드합니다.
4.  **[Cell 9]**을 실행하면, AI가 이미지를 분석하여 최종 `JSON` 결과를 출력합니다.
