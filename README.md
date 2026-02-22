# **<img src="./assets/YMRPC_ico.ico" alt="[DISCORD RPC]" width="30"/> &nbsp;Fork of [WinYandexMusicRPC](https://github.com/FozerG/WinYandexMusicRPC)**

[![TotalDownloads](https://img.shields.io/github/downloads/tired272/WinYandexMusicRPC/total)](https://github.com/tired272/WinYandexMusicRPC/releases "Download") [![LastRelease](https://img.shields.io/github/v/release/tired272/WinYandexMusicRPC)](https://github.com/tired272/WinYandexMusicRPC/release)

**Discord RPC для показа музыки которую вы сейчас слушаете на компьютере. Загрузка треков и их обложек происходит из Яндекс Музыки.**

<img width="287" height="125" alt="image" src="https://github.com/user-attachments/assets/6b873398-af5a-41ad-bb51-2c1de1d28029" />

Существуют похожие RPC, которые показывают текущий трек, используя API Яндекс Музыки. Однако они не могут отображать информацию о том, что играет из радио (например, `Моя Волна`).

FozerG создал скрипт, который использует `Windows.Media.Control` для получения информации о текущем треке, выполняет поиск в Яндекс Музыке и отображает трек в Discord.

Плюсы по сравнению с другими скриптами:    
Не нужен токен Яндекс Музыки ✅  
Показывает треки из подборок, радио ✅  
Не ограничен использованием Яндекс Музыки, музыку можно слушать хоть из ВКонтакте ✅  
Работает как с браузерами так и с приложениями ✅   
Показывает статус паузы ✅  
Показывает сколько осталось до конца трека ✅  
Статус "Слушает" вместо "Играет в игру" ✅

## Требования
Работа проверена только на Windows 11 и Windows 10, на других версиях и платформах работать не будет. **С урезанными Lite и Custom версиями Windows работа не гарантируется.**

## Как скачать и использовать Exe?
1. Скачиваем [последний доступный релиз](https://github.com/tired272/WinYandexMusicRPC/releases)
2. Извлекаем из архива папку WinYandexMusicRPC-cli, запускаем WinYandexMusicRPC.exe
3. Скрипт через 3 секунды автоматически скроется в системный трей. Откройте консоль через трей чтобы убедиться в работе.

## Как использовать main.py?
Python <3.14, >=3.10
1. Открываем терминал и идем в папку где находится файл `requirements.txt`.
2. Пишем `pip install -r requirements.txt` для того что бы установить зависимости.
3. В терминал пишем `python main.py`

>Чтобы скомпилировать скрипт с помощью [Pyinstaller](https://pypi.org/project/pyinstaller/), выполните данную команду:  
`pyinstaller --noconfirm main.spec`

------------
В случае если вы слушаете музыку не только из яндекс музыки, рекомендую заменить строку `strong_find = True` на `strong_find = False`, или воспользуйтесь системным треем. Тогда будет показыватся лучший результат по поиску, но не всегда точный.

Если вы нашли ошибку, то не стесняйтесь сообщать о ней в [Issues](https://github.com/tired272/WinYandexMusicRPC/issues)
------------
>Используется [Yandex Music API](https://github.com/MarshalX/yandex-music-api)   
