# GEMSTON Observatory

## О проекте / токене

По описанию STON.fi, GEMSTON — взаимозаменяемый токен вовлечённости экосистемы протокола на TON. Пользователи получают GEMSTON при стейкинге STON и могут переводить или обменивать его. GEMSTON не предоставляет права голоса в DAO.

Краткое описание по указанным первичным источникам.

Источники (проверены 2026-11-25):

- <https://ston.fi/tokens/gemston>
- <https://ston.fi/staking>
- <https://tonapi.io/v2/jettons/EQBX6K9aXVl3nXINCyPPL86C4ONVmQ8vK360u6dykFKXpHCa>

Generated from https://github.com/Freebielife/TON-Observatory-Template.

Run python3 -m scripts.refresh_observatory; python3 build.py; python3 verify.py.
Publish index.html in TON Sites only after independent on-chain verification.
The bundled snapshot contains verified GEMSTON data. Section timestamps and incomplete history are shown in the interface.
Only native TON swap pairs supported. Locks, staking and custom project NFT badges are configured through project.json and verified against TonAPI.
The update.yml workflow supports manual and external scheduler dispatch. A successful Actions run must be observed before claiming automatic refresh is verified.

Foundation version: 1.3.0. Holders show 10, expandable to top 20.
`project.json` is the per-project specification. Contract/pool/precision changes require regenerating from the factory; do not reuse another token's snapshot.
Run `python3 build.py` for an atomic bundle and `build/report.json` size report.
No external fonts, scripts or images are needed to render the saved page. Fresh data checks and manual wallet lookups require network access.
Cloudflare dispatch registration and GitHub repository access remain separate deployment steps. No credentials go into HTML.

## Оформление и источники

Контракт: `0:57e8af5a5d59779d720d0b23cf2fce82e0e355990f2f2b7eb4bba772905297a4`, decimals: 9.
Пользовательское изображение GEMSTON использовано для баннера и флага по прямому указанию пользователя; источник файла и выбор сохранены в project.json. Официальный URL изображения из метаданных при проверке ответил HTTP 403.
Официальная страница: https://ston.fi/tokens/gemston . Канал STON.fi: https://t.me/stonfidex (ссылка с https://ston.fi/).

Подтверждены три прямых TON-пула (STON.fi и DeDust); доказательства успешных swap-действий сохранены в project.json. Другие обнаруженные пары перечисляются отдельно и не включаются в заявленное покрытие прямых обменов с TON.

Публикация в TON Storage и наблюдение планового запуска проверяются отдельно от сохранения в main.

## Проверка сборки 2026-11-25

17 Python-тестов и 15 JavaScript-тестов пройдены. Проверены RU/EN, раскрытие держателей 10 → 20, переключение валюты и периода графика. На настольном экране 1363 px и в мобильной области 390 px горизонтальное переполнение отсутствует. Все якоря ведут к существующим разделам; шрифты, стили, скрипты и изображения встроены.

Официальные ссылки подтверждены через страницы STON.fi и TON API. Прямой HTTP-контроль внешних страниц из среды сборки возвращает 403, поэтому доступность всех внешних страниц из браузера посетителя не заявляется.
