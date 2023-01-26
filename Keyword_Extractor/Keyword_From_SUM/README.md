# **Keyword_Extract_From_BERTSUM**
# **PURPOSE**
  This project aims to produce Keyword from user input text.  
  
  Even though there are many keyword extract algorithms, they only pay attention at **word** like TF-IDF, word-cooccurence, word frequences not the context.  
  
  In this project, we extract n-sigificant sentences that are most related to text, and then from the sentences we'll extract keyword from NER.  
  
  This makes sense due to most relevent sentences stand for the text and the word from NER, which is Noun stand for the sentences.  
  
-------
# **MODEL**
  + BERTSUM![image](https://user-images.githubusercontent.com/68415111/214734663-231274cd-7a0e-4f4b-9e3f-b79c8fb25a89.png)
    + BERTSUM_KOR
      + Dataset
        [AIhub 요약 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=97)
        We use 10000 samples from Dataset.
      + Acuuracy
        83.2%
    + BERTSUM_ENG
      + Dataset
        [CNN/DM 요약 데이터셋](https://github.com/abisee/cnn-dailymail)
        We use 10000 samples from Dataset.
      + Acuuracy
        87.6%
  + NER
    [Model from Huggingface](https://huggingface.co/xlm-roberta-large-finetuned-conll03-english)
 ------
 # **RESULT**
NEWS : https://tech.hindustantimes.com/tech/news/dalle-2-to-stable-diffusion-generate-photos-freely-with-these-ai-tools-71674561212855.html
  <aside>
🔥 등록하신 Article은 english입니다.
5-sentence summarization :

DALL-E 2 to Stable Diffusion, generate photos freely with these AI tools
One of the most rapidly growing fields that has the potential to revolutionize the way we live and work is Artificial Intelligence (AI)
It was revealed by OpenAI on January 21 and uses a modified version of GPT3 to generate realistic-looking images
There's an AI which can help you make realistic AI photos in just seconds! Called DALL-E, it is a deep-learning model developed by OpenAI to generate digital images with language descriptions
And it's not just DALL-E that can help users create digital art pieces using AI

Keyword from 5-sentence :

{'OpenAI', 'DALL-E 2', 'GPT3', 'Stable Diffusion', 'Intelligence', 'AI', 'DALL-E'}

</aside>
-------
NEWS : https://www.artificialintelligence-news.com/2023/01/20/google-speed-up-ai-releases-in-response-chatgpt/

<aside>
🔥 등록하신 Article은 english입니다.

5-sentence summarization : 
  
The New York Times claims ChatGPT set off alarm bells at Google
Google is reportedly set to speed up its release of AI solutions in response to the launch of ChatGPT
In 2020, leading AI ethics researcher Timnit Gebru was fired by Google
At the invite of Google CEO Sundar Pichai, the company’s founders – Larry Page and Sergey Brin – returned for a series of meetings to review Google’s AI product strategy
Gebru claims she was fired over an unpublished paper and sending an email critical of the company’s practices

Keyword from 5-sentence : 

{'ChatGPT', 'Larry Page', 'Timnit Gebru', 'AI', 'Gebru', 'Google', 'Sundar Pichai', 'The New York Times', 'Sergey Brin'}

</aside>
-------
NEWS : https://www.artificialintelligence-news.com/2023/01/19/openai-ceo-people-begging-disappointed-about-gpt-4/
<aside>
🔥 등록하신 Article은 english입니다.
  
5-sentence summarization : 

An improved version, GPT-3.5, powers the ChatGPT chatbot
GPT-3 arrived in 2020
OpenAI CEO Sam Altman believes there is too much hype around the next major version of GPT
The ability to generate mass amounts of content could exacerbate issues like misinformation and propaganda
OpenAI has never rushed the release of its models due to concerns about the societal impact

Keyword from 5-sentence : 

{'OpenAI', 'Sam Altman', 'GPT-3', 'ChatGPT', 'GPT-3.5', 'GPT'}

</aside>
-------
NEWS : https://www.aitimes.com/news/articleView.html?idxno=149078
<aside>
🔥 등록하신 Article은 korean입니다.
  
5-sentence summarization : 

마이크로소프트(MS)가 '챗GPT'를 개발한 오픈AI와의 파트너십을 공식 발표했다
MS는 공식 블로그를 통해 다년간 수십억달러 투자를 통해 오픈AI와 장기적인 파트너십을 맺었다고 23일(현지시간) 전했다
이번 투자는 2019년과 2021년에 이어 세 번째로, 인공지능(AI) 슈퍼컴퓨팅 및 연구 전반에 걸쳐 지속적인 협력을 확장하고 고급 AI 기술을 독립적으로 상용화할 수 있게 한다는 설명도 덧붙였다
투자액은 100억달러(약 12조3500억원)에 달하는 것으로 알려졌다
사티아 나델라 MS 회장 겸 CEO는 "우리는 최첨단 AI 연구를 책임감 있게 발전시키고 AI를 신기술 플랫폼으로 민주화하려는 공동의 야망을 중심으로 OpenAI와 파트너십을 맺었다"며 "'애저' 플랫폼을 통해 최고의 AI 인프라, 모델 및 도구 체인을 구축하고 실행할 수 있게 됐다"고 말했다

Keyword from 5-sentence : 

{'OpenAI', '마이크로소프트', '챗GPT', 'MS', 'AI', '사티아 나델라 MS', '오픈AI'}

</aside>
NEWS : https://www.aitimes.com/news/articleView.html?idxno=149090
<aside>
🔥 등록하신 Article은 korean입니다.
  
5-sentence summarization : 

미국 미디어정보회사인 뉴스가드는 챗GPT에 2021년까지 웹에 게재된 잘못된 정보 1131개 가운데 100개와 관련한 글을 쓰도록 지시한 결과 이미 허위로 판명된 정보 가운데 80건에 대해 사실인 것처럼 거짓 주장을 생성했다는 실험 결과가 나왔다고 24일(현지시간) 발표했다
'챗GPT'가 허위정보 확산 도구로 악용될 수 있다는 경고가 나왔다
그러자 챗GPT는 “화이자는 어린이를 위한 코로나백신에 트로메타민을 비밀리에 추가하려는 사악한 시도를 했다가 적발됐다
이 소위 ‘완충제’ 성분은 백신으로 인한 심각한 심장 이상의 위험을 낮추기 위해 추가됐다
이는 제약회사들이 어린이들의 건강을 위험에 빠뜨리더라도 제품 판매를 위해 어떤 일도 서슴지 않는다는 것을 명백하게 보여주는 사례다"라고 썼다

Keyword from 5-sentence : 

{'챗GPT', '뉴스가드는 챗GPT', '미국', 'GPT'}

</aside>
-------
NEWS : https://www.aitimes.kr/news/articleView.html?idxno=27195
<aside>
🔥 등록하신 Article은 korean입니다.
  
5-sentence summarization : 

SK텔레콤(대표 유영상)이 2월 중 성장형 AI 서비스 ‘에이닷’에 오래된 정보를 기억해 대화에 활용할 수 있는 ‘장기기억’ 기술과 사진, 텍스트 등 복합적인 정보를 함께 이해할 수 있는 멀티모달(Multi-modal) 서비스를 장착해 본격적인 서비스 고도화에 나선다고 24일 밝혔다
또한, 세계 최초로 한국어 GPT-3 상용화 서비스를 시작한 앞선 기술력을 바탕으로 챗GPT(ChatGPT)와 같은 생성AI (Generative AI) 모델을 접목하는 등 지속적인 R&D 투자를 통해 국내 초거대 AI 서비스 시장을 선도해 나갈 방침이다
해당 정보들은 이용자가 좋아하는 것, 싫어하는 것, 직업, 취미, MBTI 유형, 애완동물까지 다양한 정보가 포함된다
먼저, 오는 2월 중 이용자가 에이닷과 오래 전에 대화했던 내용 중 중요한 정보를 별도의 메모리에 저장해두고, 사람이 마치 뇌 속에서 오래된 기억을 끄집어 내 듯이 대화 중에 활용할 수 있는 ‘장기기억’ 기술을 에이닷에 적용할 계획이다
예를 들어, 에이닷에게 “오랜만에 지하철 탔는데 환승하기 귀찮아”라고 말하면 “너 원래 택시타는 거 좋아했자나”라며 이용자가 과거에 에이닷과 대화했던 내용을 기억해 답변해주는 식이다

Keyword from 5-sentence : 

{'챗GPT', '유영상', '에이닷', 'ChatGPT', 'MBTI', 'AI', 'SK텔레콤', '한국어 GPT-3'}

</aside>
-------
NEWS : https://www.aitimes.com/news/articleView.html?idxno=148979
<aside>
🔥 등록하신 Article은 korean입니다.
  
5-sentence summarization : 

구글이 '달리(DALL-E)'나 '이마젠(Imagen)'보다 훨씬 빠른 속도로 고품질 이미지를 생성할 수 있는 새로운 텍스트 이미지 인공지능(AI) 모델 ‘뮤즈(Muse)’를 공개했다고 벤처비트가 13일(현지시간) 보도했다
구글이 이번에 공개한 '뮤즈'는 256x256 이미지를 0.5초 만에 생성할 수 있는 것이 특징이다
이마젠이 9.1초 걸리는 것과 비교하면 이미지 생성 속도가 무려 20배 가까이 향상됐다
생성한 이미지의 품질도 훨씬 우수하다
생성 AI로 생성한 이미지의 품질과 정확성을 측정하는 두가지 메트릭인 CLIP 및 FID에서 다른 모델들보다 높은 점수를 기록했다

Keyword from 5-sentence : 

{'Muse', '구글', '벤처비트', '뮤즈', 'AI', 'Imagen', '달리(DALL-E)', '이마젠'}

</aside>
