# NER
Please develop an Event-oriented NER (Name Entity Recognition) tool which can extract 5 entities such as people, time, location, object, and event from input sentence(or article).

Input : sentence(or article)
Output : 5 types of entities (People, Time, Location, Object, Event)

### people
從句子一開先判斷詞語是否有Nb和Nh，如果有則將無放入，但句子中若有包含“自己”時，通常前面會有主要的主詞，所以就跳過
![image](https://user-images.githubusercontent.com/93340978/235042268-22b88ad9-fb03-494d-b330-daf7bd44708b.png)
### event
先分出句子=>依據標點符號，。；等
句子中先找出特定動詞，像是VC、VJ等
從特定動詞開始，一路到句子結束便是完整事件，中間有些特定詞性的詞需扣掉，像是FW、SHI等
![image](https://user-images.githubusercontent.com/93340978/235042376-e9dad7ef-8fea-47df-a1bc-33e0ae05e47f.png)
![image](https://user-images.githubusercontent.com/93340978/235042383-3c6788e4-f396-46c7-95b4-cd5b18613d7d.png)
![image](https://user-images.githubusercontent.com/93340978/235042390-32f78176-fc90-44d8-9dbc-7d7308a321a5.png)
![image](https://user-images.githubusercontent.com/93340978/235042399-80b39d32-43ad-470e-b9d9-45db43b1b0cf.png)
![image](https://user-images.githubusercontent.com/93340978/235042408-27883f28-8b22-4133-a333-18d0e49d8bc8.png)
### time
找句子中的時間時，找出句中是否有Nd和Neu，如果有Neu後面通常會接Nd，例如:20(Neu)年前(Nd)，像有提及數字的也需要把後面的單位放入
![image](https://user-images.githubusercontent.com/93340978/235042454-465fd09c-e9f3-42b8-ba3d-c12abab69f94.png)
### location
找句子中的地點時，找出句中是否有Nc

![image](https://user-images.githubusercontent.com/93340978/235042549-ea7ea5a2-4e30-40d9-8cd9-a310ee11f2aa.png)
### object
找句子中的物件時，找出句中是否有Na

![image](https://user-images.githubusercontent.com/93340978/235042618-0ac9aed2-e1ce-4d6b-9740-12b01f12ac72.png)





