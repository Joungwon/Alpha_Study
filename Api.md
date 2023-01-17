# API

ex) telegram bot api   텔레그램에서 제공하는 공개 api  

1. BotFather를 통해 token 정보 


sendMessage 의 경우 Required가 Yes 존재 : 무조건 출력

코드 

import requests

token = '5418588382:AAE_hOjyCEDyh2NYO5gukuJFjVuGzEdzNGI'
  (텔레그램
# https://api.telegram.org/bot5418588382:AAE_hOjyCEDyh2NYO5gukuJFjVuGzEdzNGI/getMe

url = f'https://api.telegram.org/bot{token}/getupdates'

data = requests.get(url).json()

chat_id1 = data.get('result')[0].get('message').get('chat').get('id')
msg = '졸려..'

send_url = f'https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id1}&text={msg}'

requests.get(send_url)







# api 실행
# url = 'https://api.bithumb.com/public/ticker'
# response = requests.get(url)
# # print(response)     # 객체 수만 나온다 200개
# data = response.json()['data']    #json을 붙여서 딕셔너리로 만든다.
# print(data)
# print(data['opening_price'])





# #로또 당첨번호
# import requests

# url = 'https://dhlottery.co.kr/common.do?method=getLottoNumer&drwNo=1049'
# response = requests.get(url)
# # print(response)     # 객체 수만 나온다 200개
# data = response.json()    #json을 붙여서 딕셔너리로 만든다.
# print(data)

# # for i in range(1,7):
# #     key = f'drwtNo{i}'                #f스트링 사용: drwtNo1, drwtNo2등 축약가능
# #     print(response.get(key))

# for i in range(1,7):
#     print(data.get(f'drwtNo{i}'))




# #코드 공유하는법
# ```python
# import requests

# url = 'https://www.dhlottery.co.kr/common.do?method=getLottoNumber&drwNo=1049'

# data = requests.get(url).json()
# print(data)

# for i in range(1,7):
#     key = f'drwtNo{i}'
#     print(data.get(key))
# ```
