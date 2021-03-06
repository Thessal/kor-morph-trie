# kor-morph-trie

## Introduction
NLP course work의 첫번째 과제로 구현한 한국어 형태소 분석기 입니다. Trie 자료구조와 tabular parsing 을 이용하였으며, 주어진 다섯문장에 대해 문장 분석이 가능합니다.

## 프로그램 실행 환경
```
window10 python3.6.7
```

## 사용 라이브러리
```buildoutcfg
numpy : 1.16.2
collections ( 파이썬 기본 )
```

## 프로그램 실행 방법
윈도우 커맨드라인 창에서 kor-morph-trie 폴더로 이동하여 main 프로그램을 실행합니다.
```
$ cd kor-morph-trie
$ python main.py 
```

```buildoutcfg
문법 정보를 불러왔습니다.
사전 정보를 불러왔습니다.
사전에 들어있는 단어 개수는 71개 입니다.
TRIE 사전 구축을 완료하였습니다.
분석할 문장을 입력하세요.
<분석할 문장 입력> ex) 사람이 교만하면 낮아지고 겸손하면 존경을 받는다. 
```

```
문장 분석 결과는 다음과 같습니다.
사람/일반명사
사람/일반명사+이/보격조사
사람/일반명사+이/주격조사
교만/일반명사
교만/일반명사+하/형용사파생접미사
교만/일반명사+하/동사파생접미사+면/연결어미
교만/일반명사+하/형용사파생접미사+면/연결어미
하/보조용언
하/보조용언+면/연결어미
낮/형용사+아/연결어미
낮/형용사+아/연결어미+지/보조용언+고/연결어미
지/보조용언
지/보조용언+고/연결어미
겸손/일반명사
겸손/일반명사+하/형용사파생접미사
겸손/일반명사+하/동사파생접미사+면/연결어미
겸손/일반명사+하/형용사파생접미사+면/연결어미
하/보조용언
하/보조용언+면/연결어미
존경/일반명사
존경/일반명사+을/목적격조사
받/동사+는/관형형전성어미
받/동사+는다/종결어미
```

입력된 문장에서 구성 가능한 문법을 전부 출력하도록 구성하였습니다.
