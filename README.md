# **<img src="./assets/YMRPC_ico.ico" alt="[DISCORD RPC]" width="30"/> &nbsp;WinSdk + Yandex Music Discord Rich Presence**
[![TotalDownloads](https://img.shields.io/github/downloads/FozerG/WinYandexMusicRPC/total)](https://github.com/FozerG/WinYandexMusicRPC/releases "Download") [![LastRelease](https://img.shields.io/github/v/release/FozerG/WinYandexMusicRPC)](https://github.com/FozerG/WinYandexMusicRPC/releases "Download") [![CodeOpen](https://img.shields.io/github/languages/top/FozerG/WinYandexMusicRPC)](https://github.com/FozerG/WinYandexMusicRPC/blob/main/main.py "Show code") [![OS - Windows](https://img.shields.io/badge/OS-Windows-blue?logo=windows&logoColor=white)](https://github.com/FozerG/WinYandexMusicRPC/releases "Download")

>Несмотря на неразумное решение о блокировке Discord в РФ, я продолжу поддерживать скрипт в рабочем состоянии, насколько это будет возможно 🕊️

>[Мы будем пользоваться тем, что нам нравится.](https://github.com/Flowseal/zapret-discord-youtube)

**Этот вариант скрипта не устарел, но возможно вы захотите использовать [эту версию](https://github.com/FozerG/YandexMusicRPC). Она работает через сервера Яндекса, и показывает треки даже с других устройств таких как Mac, iPhone или Android.**

⚠️ **16.12.2025:** Если вы используете приложение «Яндекс Музыка», отключите в настройках опцию **«Плавные переходы между треками»**. В текущей версии эта функция нарушает работу `Media.Control` и скрипта.

**Discord RPC для показа музыки которую вы сейчас слушаете на компьютере. Загрузка треков и их обложка происходит из Яндекс Музыки.**

<img src="https://github.com/user-attachments/assets/99d15c70-632f-41ec-a6cd-49de8a7d2a8f" alt="discord" width="340">

Существуют похожие RPC, которые показывают текущий трек, используя API Яндекс Музыки. Однако они не могут отображать информацию о том, что играет из радио (например, `Моя Волна`).

Поэтому я создал скрипт, который использует `Windows.Media.Control` для получения информации о текущем треке, выполняет поиск в Яндекс Музыке и отображает трек в Discord.

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

Если вы не будете использовать ехе файл то:
1. Python <3.14, >=3.10

## Как скачать и использовать Exe?
1. Скачиваем [последний доступный релиз](https://github.com/tired272/WinYandexMusicRPC/releases)
  
2. Открываем WinYandexMusicRPC

3. Скрипт через 3 секунды автоматически скроется в системный трей. Откройте консоль через трей чтобы убедиться в работе.

## Как использовать main.py?

1. Открываем терминал и идем в папку где находится файл `requirements.txt`.
2. Пишем `pip install -r requirements.txt` для того что бы установить зависимости.
3. В терминал пишем `python main.py`

>Чтобы скомпилировать скрипт с помощью [Pyinstaller](https://pypi.org/project/pyinstaller/), выполните данную команду:  
`pyinstaller --noconfirm main.spec`

------------
В случае если вы слушаете музыку не только из яндекс музыки то рекомендую заменить строку `strong_find = True` на `strong_find = False`, или воспользуйтесь системным треем. Тогда будет показыватся лучший результат по поиску, но не всегда точный.

## Баги
Баги всегда существуют, но сначала их надо найти 🫡  
Если вы нашли ошибку, то не стесняйтесь сообщать о ней в [Issues](https://github.com/FozerG/WinYandexMusicRPC/issues)
   
------------
Пожалуйста, покажите вашу заинтересованность в этом проекте, что бы я мог его обновлять по мере возможности.

>Код не идеален, так как Python не является моим основным языком, и скрипт был написан для личного использования. Однако он может стать основой для ваших собственных скриптов.

>Используется [Yandex Music API](https://github.com/MarshalX/yandex-music-api)   
