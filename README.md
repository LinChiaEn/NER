# NER
Please develop an Event-oriented NER (Name Entity Recognition) tool which can extract 5 entities such as people, time, location, object, and event from input sentence(or article).

Input : sentence(or article)
Output : 5 types of entities (People, Time, Location, Object, Event)

### people
從句子一開先判斷詞語是否有Nb和Nh，如果有則將無放入，但句子中若有包含“自己”時，通常前面會有主要的主詞，所以就跳過
![image](https://user-images.githubusercontent.com/93340978/235042268-22b88ad9-fb03-494d-b330-daf7bd44708b.png)

