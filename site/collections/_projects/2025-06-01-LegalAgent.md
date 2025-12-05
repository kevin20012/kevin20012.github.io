---
date: 2025-06-01 08:20:35 +0300
title: RAG를 활용한 gpt-4o 기반의 법률 에이전트 개발
subtitle: 개인프로젝트
image: '/images/legal/logo.png'
---

| Method            | Score |
|-------------------|-------|
| 0-shot            | 37    |
| 5-shot            | 37.5  |
| **with RAG (ours)**   | **42.5**  |


LLM을 사용한 법률 도우미 시스템을 만들기 위해, RAG를 바탕으로 실제 법률에 기반한 대답을 하도록 LLM 에이전트를 구현하였습니다. 법률 데이터는 '국가법령정보 공동활용' 사이트에서 제공하는 API를 사용하여 총 1682개의 법률데이터를 크롤링하였습니다. 이후 임베딩과 인덱싱을 거쳐 FAISS 인덱싱 DB를 구축하고, 주어지는 쿼리에 대한 코사인 유사도 기반으로 상위 20개의 문서를 가져온 뒤, 이를 바탕으로 질문에 답변하는 시스템을 구현하였습니다. KMMLU 법률 분야에서 제로샷 대비 14%의 성능 향상을 보였습니다.

[GitHub Repository](https://github.com/kevin20012/Legal-Agent-with-gpt-4o-using-RAG)