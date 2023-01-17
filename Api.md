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
