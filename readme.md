# Project
1. 관심 데이터 선정
    - AIHUB에서 한글 -> 영어 말뭉치 번역 데이터 선택

2. 데이터 선정이유
   - 파파고와 같은 번역 프로그램을 만들때, 트랜스포머와 RNN 둘 중 어느 모델이 더 적합할지 궁금했다.
   - 자료 출처 : https://aihub.or.kr/

3. 데이터를 이용한 가설 수립
- 비슷한 조건에서 두 모델을 가동했을때, 트랜스포머 모델이 좀 더 나은 번역을 해낼 것 이다.

4. 데이터 전처리
   - 데이터 양이 많을 경우 학습시간도 오래 걸릴뿐 아니라 메모리 부족으로 토큰화나 모델가동에 에러가 발생하였음.
    1,210,529 데이터를 10,000 개의 데이터만 사용하는 것으로 축약함.

5.딥러닝 방식 적용
- transformer
- RNN
- 모델 검증(Validation)

6. 데이터 구성

- sn - 데이터 번호
- file_name - 정제된 원본 문서명
- data_set - 기술과학/사회과학 구분
- domain - 데이터 대분야
- subdomain - 데이터 소분야
- source - 원문 출처
- ko - 한국어 문장
- mt - 기계번역 문장
- en - 영어 문장
- source_language - 원문 언어 코드
- target_language - 번역문 언어 코드
- license - 라이선스
- style - 문체


회고
- 형태소 분석을 활용하지 못해서 번역에서 약간 부족한 모습을 보여주었지만, 추후 형태소분석 부분을 추가하면 괜찮은 결과를 나타내줄것으로 예상됨.