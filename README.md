# BPN для Windows

VPN-клиент сервиса BPN для Windows 10 и 11 (x64).

Здесь только готовые установщики, исходного кода в этом репозитории нет.

## Скачать

Последняя версия — на странице [Releases](https://github.com/Rerowros/bpn-releases/releases/latest), файл `BadVpn_<версия>_x64-setup.exe`.

Тот же установщик с нашего сервера: https://dl.badvpn.win/windows/BadVpn_x64-setup.exe

Дальше приложение обновляется само, установщик нужен только для первой установки.

## Подписка

Подписку BPN можно получить в Telegram: https://t.me/bpn228bot?start=c_desktopApp

## Проверка файла

SHA-256 каждого установщика указан в описании релиза и в файле `SHA256SUMS.txt` рядом с ним. Проверить в PowerShell:

```powershell
Get-FileHash .\BadVpn_1.1.0_x64-setup.exe -Algorithm SHA256
```

Установщик пока не подписан сертификатом, поэтому Windows может показать «Неизвестный издатель». Нажмите «Подробнее» → «Выполнить в любом случае».

## Сторонние компоненты

При первом подключении приложение скачивает и проверяет по хешу:

- [Mihomo](https://github.com/MetaCubeX/mihomo) — ядро VPN (GPL-3.0);
- [zapret](https://github.com/bol-van/zapret) — обход блокировок для YouTube, Discord и игр (MIT);
- [WinDivert](https://github.com/basil00/WinDivert) — драйвер перехвата пакетов для zapret (LGPL-3.0).

## English

BPN is a Windows 10/11 (x64) VPN client for the BPN service. This repository hosts release installers only; it contains no source code. Download the latest installer from [Releases](https://github.com/Rerowros/bpn-releases/releases/latest) and check its SHA-256 against `SHA256SUMS.txt`.

## Лицензия

См. [LICENSE.txt](LICENSE.txt).
