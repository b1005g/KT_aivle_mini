# KT_aivle_big_project
![stop_robot](https://github.com/user-attachments/assets/f6a03d10-e9b4-4359-afb8-042bd867af4f)

- Project_name : 악성 필터링 AI
- 악성민원 방지를 위한 필터링 시스템 구축
- 기술 스택 : python

# 구현 기술
- 파일 업로드 내용 필터링, 선정적 이미지 필터, 민원보고서 작성 
- fastapi, pytorch, transformer, langchain

# 서비스 플로우
1. 게시글 내용 -> 정상 / 악성(label 11개) 분류 -> 내용 순화(oepnai_api)
- roberta 파인튜닝(데이터셋) -> 라벨 분류 시행
- 내용 순화 --> gpt-4 모델을 이용하여 순화
  
2. 파일 필터링
- nsfw_image_detection 모델 사용, 이미지 필터
- langchain-loader를 이용하여 문서 내부 text 읽어옴 -> roberta로 분류
- 부적절한 파일일 경우 업로드 제한
  
3. 민원보고서 작성(악성 판단시)
- 민원 내용 fastapi basemodel으로 받아서 해당 내용을 gpt로 요약하고, 민원보고서 자동작성 및 저장

