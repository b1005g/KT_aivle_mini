# KT_aivle_mini

## **0.미션**

단계 1에서는, 응급상황의 음성을 인식해서 텍스트로 변환하고, 변환된 텍스트를 다시 요약 및 핵심키워드 도출 작업을 수행합니다.  
이를 위해 사전학습된 모델을 API로 연결하여 활용합니다.

* 음성인식 : STT(Speech-to-Text)
    * 사용 모델 : OpenAI의 **Whisper-1**
    * 제공받은 음성 파일과 새로 제작하는 5건 이상의 음성파일을 텍스트로 변환하고, 변환작업이 잘 되는지 확인해 봅시다.
* 텍스트 요약 및 핵심 키워드 도출
    * 사용 모델 : OpenAI의 **GPT-3.5-turbo**
    * 내용 요약과 주요 키워드를 도출하도록 프롬프트 입력과 출력을 구성하고 테스트 해 봅시다.

* 음성데이터 : 위급상황_음성-음향_고도화_119_지능형_신고접수_음성_인식_데이터
    * https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=71768
    * 서울데이터 사용
      
![image](https://github.com/user-attachments/assets/b48b79a4-b851-495a-9729-1c77ff94b162)
