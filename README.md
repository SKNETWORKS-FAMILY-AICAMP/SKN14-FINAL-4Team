<p align="center"><img src="https://elasticbeanstalk-ap-northeast-2-967883357924.s3.ap-northeast-2.amazonaws.com/static/images/logo_big.png" alt="project-image"></p>
 
> [SKN14-Final-4Team-Web(Frontend Git Repo)](https://github.com/skn-ai14-250409/SKN14-Final-4Team-Web)
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
> [SKN14-Final-4Team-AI(Backend Git Repo)](https://github.com/skn-ai14-250409/SKN14-Final-4Team-AI)

------------------------------------------------------------------------------------------------------------------------

# 할당받은 주제
LLM 활용 인공지능 인플루언서 만들기


# 초기 기획 방향
1. 특정 인플루언서의 영상/말투 데이터를 수집하고 모델에 학습시킨 후, **사용자와 영상통화처럼 실시간 대화(또는 채팅)하는 App** 구상.  
   => 주어진 시간/인력/비용을 벗어나고, 난이도가 높다는 피드백에 따라 <span style='color: red;'>폐기</span>
2. 특정 **인플루언서들의 음성파일로 모델을 Fine-Tuning** 하고, 그들과 대화(또는 채팅)할 때 **인플루언서의 목소리로 대화를 나눌 수 있는 채팅 App** 구상.  
   => 이전 기수에서 진행되었던 프로젝트와 너무 많이 겹치고, 아이디어 구상 자체가 너무 단순하다는 내부 의견에 따라 <span style='color: red;'>폐기</span>
3. **친환경 제품들을 판매하는 브랜드를 알릴 수 있는 정보전달용 사이트**를 구축하고, 해당 사이트에서 **인공지능 인플루언서가 TTS 로 정보를 전달하는 Webapp** 구상.  
   => '친환경 제품' 이라는 범주가 너무 크고, 프로젝트의 주제와 방향을 알기 어렵다는 피드백에 따라 <span style='color: red;'>기획 수정</span>
4. <span style='color: green; font-size:bold; font-size:16px;'>최종 주제</span>  
   => '친환경 제품' 의 범위를 '재활용 의류제품' 으로 한정하여, `'재활용 제품' 에 대한 검색 및 스타일링 추천, 친환경 정보를 전달하는 서비스`를 구상.  
   => 이 때 `인공지능 인플루언서의 TTS 를 도입`하여, 사용자로 하여금 `소통/교감/신뢰도/흥미를 느낄 수 있도록 유도`한다. 

------------------------------------------------------------------------------------------------------------------------

# 🔎 문제 정의
- 온난화, 각국의 이상기후 등 `환경 문제에 대한 위기감 증가`


# 📌 시장 분석
- `기후감수성`              : 환경 문제에 대하여 2030 세대가 갖는 인식의 변화 [[ 출처 ]](http://news-j.co.kr/View.aspx?No=3489567)
- `지속가능 패션 시장 성장` : 글로벌 친환경 패션 시장 규모 2025년 13억 달러 → 2032년 53억 달러 전망 [[ 출처 ]](https://www.coherentmarketinsights.com/industry-reports/global-sustainable-fashion-market)
- `MZ세대 트렌드`           : 브랜드 충성도보다 가치소비·지속가능성을 우선시 [[ 출처 ]](https://www.k-trendynews.com/news/articleView.html?idxno=176226#:~:text=%5BKtN%20%EC%B5%9C%EC%9C%A0%EC%8B%9D%EA%B8%B0%EC%9E%90%5D%20MZ%EC%84%B8%EB%8C%80(%EB%B0%80%EB%A0%88%EB%8B%88%EC%96%BC+Z%EC%84%B8%EB%8C%80)%EA%B0%80%20%EC%86%8C%EB%B9%84%20%EC%8B%9C%EC%9E%A5%EC%9D%98%20%EC%A3%BC%EC%9A%94%20%EC%A3%BC%EC%B2%B4%EB%A1%9C,%EC%82%AC%ED%9A%8C%EA%B0%80%20%EC%A3%BC%EB%AA%A9%ED%95%B4%EC%95%BC%20%ED%95%A0%20%EB%B3%80%ED%99%94%EC%9D%98%20%ED%9D%90%EB%A6%84%EC%9C%BC%EB%A1%9C%20%EC%9E%90%EB%A6%AC%20%EC%9E%A1%EC%95%98%EB%8B%A4.)
- `패션+AI 융합`            : AI 기반 스타일 추천 시장과 ESG 경영 확산이 동시에 부상 [[ 출처 ]](https://seochocnc.com/53/?bmode=view&idx=165508709)


# ䷒ 접근방식
- 소비자가 `패션 선택과 동시에 친환경적 가치를 실현할 수 있도록 유도한다.`
  - 비슷한 디자인과 스타일의 기존제품들에 비해 `가성비가 높고 비용도 더 저렴한 Recycling product 들을 쉽게 검색`해볼 수 있다.
  - Recycling product 를 사용함으로써 환경이슈에 어느정도로 기여할 수 있는지를 함께 제공함으로써 `환경이슈에 대한 사용자들의 관심도`를 높인다.
- 인공지능 인플루언서의 톤앤매너로 `개인 맞춤형 추천+가이드를 간편 대화형으로 제공한다.`
  - Recycling product 를 제작하는 브랜드의 제품들 정보를 수집하고, 그 `제품들이 환경에 어떻게 기여하는지 정보를 함께 전달`하는 서비스.


# 👤 활용대상 및 기회
- **Customer Aspect**
  - 기존에 환경이슈에 관심이 많았던 사람
  - 환경이슈에 무심하거나 그러한 정보가 있음을 알지 못했던 사람
  - 비슷한 디자인에 더 저렴한 제품을 찾는 사람
- **Brand Aspect**
  - 비싼 광고비 없이 자사의 여러 제품들을 알릴 수 있는 기회
  - Recycling product 만을 다루는 서비스에서 제품을 홍보함으로써 기업이미지에 도움
- **Influencer Aspect**
  - 인지도 향상을 고민중인 패션/환경 관련 인플루언서
- **Government Aspect**
  - Recycling product 적극 활용을 통한 국내 탄소배출권 추가확보
  - 국가 차원의 지속가능성 지표, 환경성과 지수(EPI), ESG 평가도 상승
  - ‘친환경 국가’의 브랜드 아래, 환경기준이 높은 국가들의 무역 장벽 완화 가능성


# 인공지능 인플루언서 적용 방향
사용자가 선택한 `인플루언서가 그들의 말투와 어조, 목소리로 사용자에게 정보를 전달`함으로써  
사용자로 하여금 `소통/교감으로 인한 흥미를 유도`하고,  
전달하는 `정보에 대한 신뢰감 조성` 등에 인공지능 인플루언서를 활용한다.


# Agent-Flow ( 에이전트 흐름도 ) 
![](images/Agent_Flow.svg)


# 📅 프로젝트 진행일정
┌─ **2025.8.11** : 주제 회의 및 기획  
├  
├─ **2025.8.19** : 멘토링 이후 주제 전환을 위한 회의  
├  
├─ **2025.8.21** : 주제 변경 및 기획문서들 수정  
├    
├─ **2025.8.26** : 중간 발표  
├    
├─ **2025.8.27** : UI 작업  
├    
├─ **2025.9.04** : DB 연동  
├    
└─ **2025.10.2** ( 최종발표 )


# 🛠️ Tech Spec.
- Web Application ( Frontend / Backend / Database )  
![](https://img.shields.io/badge/html5-E34F26?style=for-the-badge&amp;logo=html5&amp;logoColor=white)
![](https://img.shields.io/badge/CSS-663399?style=for-the-badge&amp;logo=css&amp;logoColor=white)
![](https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&amp;logo=javascript&amp;logoColor=white)
![](https://img.shields.io/badge/django-092E20?style=for-the-badge&amp;logo=django&amp;logoColor=white)
![](https://img.shields.io/badge/fastapi-009688?style=for-the-badge&amp;logo=fastapi&amp;logoColor=white)
![](https://img.shields.io/badge/MYSQL-003B57?style=for-the-badge&amp;logo=mysql&amp;logoColor=white)
![](https://img.shields.io/badge/Pinecone-003B57?style=for-the-badge&amp;logo=pinecone&amp;logoColor=white)

- Collaboration & IDE & API  
![](https://img.shields.io/badge/Git-F05032?style=for-the-badge&amp;logo=git&amp;logoColor=white)
![](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&amp;logo=discord&amp;logoColor=white)
![](https://img.shields.io/badge/Notion-000000?style=for-the-badge&amp;logo=notion&amp;logoColor=white)
![](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&amp;logo=figma&amp;logoColor=white)
&nbsp;&nbsp;&nbsp;
![](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&amp;logo=visualstudiocode&amp;logoColor=white)
![](https://img.shields.io/badge/PyCharm-000000?style=for-the-badge&amp;logo=pycharm&amp;logoColor=white)
&nbsp;&nbsp;&nbsp;
![](https://img.shields.io/badge/OpenAI-10a37f?style=for-the-badge&amp;logo=openai&amp;logoColor=white)
![](https://img.shields.io/badge/elevenlabs-000000?style=for-the-badge&amp;logo=elevenlabs&amp;logoColor=white)

- Infrastructure  
![](https://img.shields.io/badge/AWS-Elastic--beanstalk-ff9900?style=for-the-badge&amp;logo=aws&amp;logoColor=white)
![](https://img.shields.io/badge/Certificate--manager-ff9900?style=for-the-badge&amp;logo=aws&amp;logoColor=white)
![](https://img.shields.io/badge/route53-ff9900?style=for-the-badge&amp;logo=aws&amp;logoColor=white)
![](https://img.shields.io/badge/RDS-ff9900?style=for-the-badge&amp;logo=aws&amp;logoColor=white)

- DevOps  
![](https://img.shields.io/badge/github--action-F05032?style=for-the-badge&amp;logo=git&amp;logoColor=white)
![](https://img.shields.io/badge/docker-2496ED?style=for-the-badge&amp;logo=docker&amp;logoColor=white)
![](https://img.shields.io/badge/Elastic--beanstalk-ff9900?style=for-the-badge&amp;logo=aws&amp;logoColor=white)
![](https://img.shields.io/badge/nginx-009639?style=for-the-badge&amp;logo=nginx&amp;logoColor=white)


# 🎛️ System Architecture
![](images/System_Architecture_After_SSL.svg)


# 🖼️ ERD
![](images/new_erd.png)


# 📸 Project Main pages Screenshots
<div>
  <img src="images/screenshot01.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot02.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot03.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot04.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot05.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot06.jpg" alt="project-screenshot" width="200" height="340"/>
  <img src="images/screenshot07.jpg" alt="project-screenshot" width="200" height="340"/>
</div>



# 🚀 Demo
> [LoopLabeL 사이트 바로가기](https://www.looplabel.site)


# 👥 팀 소개 :: 4-Seed
| 4-Seed | 공지환                | 송지훈                | 윤이서                | 조성렬(PM)            |
|:-----------------------:|:-----------------------:|:-----------------------:|:-----------------------:|:-----------------------:|
| ![](images/new_4seed.jpg) | ![](images/1.jpg) | ![](images/2.jpg) | ![](images/3.jpg) | ![](images/4.jpg) |


# 후기
<table>
  <thead>
    <tr>
      <th>참여자</th>
      <th>소감</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>조성렬</th>
      <td>6개월동안 배웠던 내용을 종합하여 프로젝트에 적용해본게 좋은 경험이였습니다. 시간이 3주만 더있었다면 완성도가 더 높지않았을까하는 아쉬움도 남습니다.</td>
    </tr>
    <tr>
      <th>공지환</th>
      <td>파인튜닝, 음성 합성 모델링, 말투 RAG 등 여러 AI 엔지니어링 작업을 수행하면서 개발과 협업 경험을 쌓을 수 있었습니다. runpod serverless의 파이프라인을 직접 구축해보며 새로운 방식을 도전하였고, 이 과정에서 협업과 소통의 중요성을 배웠습니다.</td>
    </tr>
    <tr>
      <th>윤이서</th>
      <td>이번 프로젝트를 발판 삼아, AI 생태계에 대해 더 많이 배우고 공부해야겠다는 생각이 들었습니다. 단순한 사용자가 아닌 생산자로서 직접 AI 서비스를 만들어 본 뜻깊은 경험이었습니다!</td>
    </tr>
    <tr>
      <th>송지훈</th>
      <td>
        <ul>
          <li>Django, FastAPI, OpenAI, VectorDB 를 종합적으로 사용한 웹서비스를 A to Z 로 만들어봤다는 점에서 재미있었습니다.</li>
          <li>개별과제부터 프로젝트에 이르기까지 LLM 프롬프팅의 중요성과 어려움을 알수있었습니다.</li>
          <li>다른 팀들의 작업을 보면서 좀더 유연하게 모델을 활용하는 방법도 배울수 있었습니다.</li>
          <li>LLM 을 활용한 서비스를 계획한다면, LLM 의 응답속도 및 응답방식에 대한 고민도 중요하다는 것을 느꼈습니다.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
