

<div align="center">
  <img src="https://i.imgyukle.com/2020/05/29/yBpJsP.jpg" width="200" height="200">
  <h1>Asena UserBot</h1>
</div>
<p align="center">
    Asena UserBot, Telegram kullanmanızı kolaylaştıran bir bottur. Tamamen açık kaynaklı ve ücretsizdir.
    <br>
        <a href="https://github.com/quiec/AsenaUserBot/blob/master/README.md#kurulum">Kurulum</a> |
        <a href="https://github.com/Quiec/AsenaUserBot/wiki/G%C3%BCncelleme">Güncelleme</a> |
        <a href="https://t.me/AsenaUserBot">Telegram Kanalı</a>
    <br>
</p>

----
![Docker Pulls](https://img.shields.io/docker/pulls/fusuf/asenauserbot?style=flat-square) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/fusuf/asenauserbot?style=flat-square)
## Kurulum
### Çok Basit Yöntem
[Youtube Videosu](https://www.youtube.com/watch?v=mUUQ53TYqI0) ![YouTube Video Views](https://img.shields.io/youtube/views/mUUQ53TYqI0?style=flat-square)

**Android:** Termuxu açın ve bu kodu yapıştırın: `bash <(curl -L https://kutt.it/xBmcpZ)`

**iOS:** iSH açın ve bu kodu yapıştırın: `apk update && apk add bash && apk add curl && curl -L -o asena_installer.sh https://kutt.it/ZKR8fq && chmod +x asena_installer.sh && bash asena_installer.sh`

**Windows 10:** [Python](https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l#activetab=pivot:overviewtab) indirin ardından PowerShell bu kodu yapıştırın: `Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://kutt.it/JI1P7S')`

### Basit Yöntem
Eğer botu kurma hakkında fikriniz yoksa burayı okuyunuz: [Kurulum Rehberi](https://github.com/Quiec/AsenaUserBot/wiki/Kurulum/)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/phaticusthiccy/AsenaUserBotDuplicated)
### Zor Yöntem
```python
git clone https://github.com/phaticusthiccy/AsenaUserBotDuplicated.git
cd AsenaUserBotDuplicated
pip install -r requirements.txt
# Config.env oluşturun ve düzenleyin. #
python3 main.py
```

## Örnek Plugin
```python
from userbot.events import register
from userbot.cmdhelp import CmdHelp # <-- Bunu ekleyin.

@register(outgoing=True, pattern="^.deneme")
async def deneme(event):
    await event.edit('Gerçekten deneme!')

Help = CmdHelp('deneme') # Bilgi ekleyeceğiz diyoruz.
Help.add_command('deneme', # Komut
    None, # Komut parametresi varsa yazın yoksa None yazın
    'Gerçekten deneme yapıyor!', # Komut açıklaması
    'deneme' # Örnek kullanım.
    )
Help.add_info('@Fusuf tarafından yapılmıştır.') # Bilgi ekleyebilirsiniz.
# Ya da uyarı --> Help.add_warning('KULLANMA!')
Help.add() # Ve Ekleyelim.
```

## Bilgilendirme
Herhangi bir istek & şikâyet & öneri varsa [destek grubuna](https://t.me/Asenaremaster) ulaşabilirsiniz.

```
    Userbottan dolayı; Telegram hesabınız yasaklanabilir.
    Bu bir açık kaynaklı projedir, yaptığınız her işlemden kendiniz sorumlusunuz. Kesinlikle Asena yöneticileri sorumluluk kabul etmemektedir.
    Asenayı kurarak bu sorumlulukları kabul etmiş sayılırsınız.
```

## Developers

[![Yusuf Usta](https://github.com/yusufusta.png?size=100)](https://quiec.tech) | [![Phaticusthiccy](https://github.com/phaticusthiccy.png?size=100)](https://github.com/phaticusthiccy) | [![Miri](https://github.com/whomiri.png?size=100)](https://github.com/whomiri) | [![Alperen Ç](https://github.com/xacnio.png?size=100)](https://github.com/xacnio)
----|----|----|----
[Yusuf Usta](https://t.me/fusuf) | [Phaticusthiccy](https://github.com/phaticusthiccy) | [Miri](https://github.com/whomiri) | [Alperen Ç](https://t.me/xacnio)
Author, Base, Bug Fixes, Modules | Base, Bug Fixes, Modules | Modules, Idea | Bug Fixes, Modules, Idea |


## Credit
Thanks for;

[Seden UserBot](https://github.com/TeamDerUntergang/Telegram-UserBot)

[Userge](https://github.com/UsergeTeam/Userge)

[Spechide](https://github.com/Spechide)
