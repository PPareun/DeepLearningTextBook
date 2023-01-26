# **Keyword_Extract_From_BERTSUM**
+ PURPOSE
  This project aims to produce Keyword from user input text. Even though there are many keyword extract algorithms, they only pay attention at **word** like TF-IDF, word-cooccurence, word frequences not the context.
  In this project, we extract n-sigificant sentences that are most related to text, and then from the sentences we'll extract keyword from NER.
  This makes sense due to most relevent sentences stand for the text and the word from NER, which is Noun stand for the sentences.
+ MODEL
  + BERTSUM
    [BERTSUM](https://www.google.com/url?sa=i&url=https%3A%2F%2Ffacerain.club%2Fbertsum-paper%2F&psig=AOvVaw1xywCNDUIhL40yiZmUpxLv&ust=1674782280751000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJDAo6qI5PwCFQAAAAAdAAAAABAE_
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
    
