# Coctohug - Управляйте десятками форков блокчейна chia из веб-браузера!
- Приятная локализация с поддержкой десятков языков: [English](./wiki_en.md), [العربية](./wiki_ar.md), [Bulgarian](./wiki_bg.md), [Catalan](./wiki_ca.md), [Deutsch](./wiki_de.md), [Español](./wiki_es.md), [زبان فارسی](./wiki_fa.md), [Français](./wiki_fr.md), [Galego](./wiki_gl.md), [Indonesian](./wiki_id.md), [Italiano](./wiki_it.md), [日本語](./wiki_ja.md), [한국어](./wiki_ko.md), [Português do Brasil](./wiki_pt.md), [limba română](./wiki_ro.md), [Русский](./wiki_ru.md), [Serbian](./wiki_sr.md), [Thai](./wiki_th.md), [Tagalog (Filipino)](./wiki_tl.md), [Türkçe](./wiki_tr.md), [Українська](./wiki_uk.md), [Vietnamese](./wiki_vi.md), [简体中文](./wiki_zh-CN.md), [繁體中文](./wiki_zh-TW.md)

Простая настройка с помощью [Быстрый старт](https://www.coctohug.xyz/)

*Ищите дополнительную помощь на нашем [Website](https://www.coctohug.xyz/) / [Github](https://github.com/raingggg/coctohug) / [Discussions](https://github.com/raingggg/coctohug/discussions) / [Discord](https://discord.gg/umfKHm7gVM)*.

# Быстрый старт
  - [Настройка Coctohug на ОС Linux](#cch-linux)
  - [Настройка Coctohug в ОС Windows](#cch-windows)
  - [Настройка Coctohug на Mac OS](#cch-macOS)
  

# Общие настройки
  - [Пароль](#cch-password)
  - [Ключи](#cch-keys)
  - [Добыча полезных ископаемых](#cch-farming)
  - [Мониторинг](#cch-monitoring)
  - [Восстановление NFT](#cch-nft_recovery)
  - [Найденные блоки / полученные монеты](#cch-blocks_found)
  - [Предупреждения о майнинге](#cch-farming_warnings)
  - [Ежедневный отчет](#cch-daily_report)
  - [Еженедельный отчет](#cch-weekly_report)
  - [Узел синхронизации](#cch-node_sync)
  - [Управление подключениями](#cch-connections_management)
  - [Управление кошельками](#cch-wallets_management)
  - [Управление руками](#cch-hands_management)
  - [Переводные монеты](#cch-transfer_coins)


# Расширенные настройки
  - [Холодный кошелек](#cch-cold_wallet)
  - [24 мнемонических слова с безопасной парольной фразой](#cch-secure_passphrase)
  - [Форки блокчейна](#cch-forks)
  - [Комбайн](#cch-harvester)
  - [Обновление](#cch-upgrade)

# Лучшие практики
  - [Местный язык](#cch-local_language)
  - [Требования к оборудованию](#cch-hardware_requirements)

<p id="cch-linux">&nbsp;</p>

## Настройка Coctohug на ОС Linux
- Настраивать <a target='_blank' href='https://www.docker.com/products/docker-desktop'>Docker</a> + <a target='_blank' href='https://docs.docker.com/compose/install/'>Docker-Compose</a> 
- Перейти на сайт <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a>, затем введите все необходимые поля формы и загрузите сгенерированные заархивированные файлы docker-compose
- Разархивируйте загруженные папки и скопируйте их в свой рабочий каталог.
- Запускаем все папки по порядку:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Откройте браузер и получите доступ к WebUI с URL-адресом <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Примечание 1: не запускайте более 5 форков блокчейна одновременно, так как форки блокчейна chia действительно съедают ЦП при синхронизации узла в первый раз.
- Примечание 2: для каждой вилки блокчейна требуется около 1,8 ГБ ОЗУ, поэтому выберите несколько вилок цепочки блоков на основе памяти вашего компьютера.
- Примечание 3: Если есть какие-либо проблемы, вам может потребоваться перезапустить все папки по порядку:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- Примечание 4: вам может потребоваться добавить разрешающие порты от 12630 до 12700 в настройках брандмауэра вашей системы.



<p id="cch-windows">&nbsp;</p>

## Настройка Coctohug в ОС Windows
- То же самое с [Настройка Coctohug на ОС Linux](#cch-linux)

<p id="cch-macOS">&nbsp;</p>

## Настройка Coctohug на Mac OS
- То же самое с [Настройка Coctohug на ОС Linux](#cch-linux)

<p id="cch-password">&nbsp;</p>

## Пароль
- Вам будет предложено установить пароль для безопасных настроек при первом доступе к WebUI с URL-адресом. <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- Настройки безопасности включают в себя: холодный кошелек, перевод монет, перезапуск форков блокчейна, комбайн ...

<p id="cch-keys">&nbsp;</p>

## Ключи
- Вам будет предложено ввести 24 мнемонических слова, когда вы впервые обращаетесь к WebUI с URL-адресом - это в основном для целей сельского хозяйства.
- Или вы можете сгенерировать один совершенно новый ключ - это в основном для целей холодного кошелька.

<p id="cch-farming">&nbsp;</p>

## Добыча полезных ископаемых
- После завершения синхронизации узлов сельское хозяйство должно начаться автоматически.
- Тогда вы сможете отслеживать статус майнинга различными способами.

![English](../../images/coctohug-summary-en-min.png)

<p id="cch-monitoring">&nbsp;</p>

## Мониторинг
- Вкладка «Сводка» может отображать: общее количество добытых монет, баланс счета, количество участков, размер участка, размер Netspace и ожидаемое время до победы.
- каждая форк-панель блокчейна на вкладке «Сводка» будет иметь светло-зеленый фон, если он работает нормально, в противном случае это будет светло-желтый фон
- Вы также можете изучить детали, используя другие вкладки

<p id="cch-nft_recovery">&nbsp;</p>

## Восстановление NFT
- На вкладке &#34;Полученные монеты&#34; есть ссылка: <a class="nav-link" target="_blank" href="https://alltheblocks.net/nft-recovery">Получите вознаграждение NFT 7/8</a>

<p id="cch-blocks_found">&nbsp;</p>

## Найденные блоки / полученные монеты
- Список всех найденных блоков
- Перечислить общее количество полученных монет

![English](../../images/received-coins-min.png)


<p id="cch-farming_warnings">&nbsp;</p>

## Предупреждения о майнинге
- Перечислите возможные проблемы с сетью
- Перечислите возможные проблемы со знаком
- Список возможных проблем с поиском на диске
- Перечислите возможные проблемы с уменьшением количества сюжетов

<p id="cch-daily_report">&nbsp;</p>

## Ежедневный отчет
- Суммируйте найденные блоки / полученные монеты за день
- Обобщение предупреждений майнинга по дням

![English](../../images/daily_report-min.png)


<p id="cch-weekly_report">&nbsp;</p>

## Еженедельный отчет
- Суммируйте найденные блоки / полученные монеты по неделям
- Обобщение предупреждений майнинга по неделям

<p id="cch-node_sync">&nbsp;</p>

## Узел синхронизации
- По умолчанию узел будет синхронизироваться автоматически
- Вы можете перейти на вкладку «Подключения» или «Блокчейны», чтобы изучить подробный статус.
- Чтобы ускорить синхронизацию вашего узла, [https://alltheblocks.net/](https://alltheblocks.net/) предоставляет список узлов и файл базы данных (щелкните каждую цепочку блоков, и вы сможете найти их в правом верхнем углу)

<p id="cch-connections_management">&nbsp;</p>

## Управление подключениями
- Список всех подключений узлов
- Вы можете добавлять / удалять соединения во вкладке Connections.

![English](../../images/connections-min.png)


<p id="cch-wallets_management">&nbsp;</p>

## Управление кошельками
- Список статусов кошелька и баланса аккаунта
- Вы также можете переводить монеты во вкладке кошелька

![English](../../images/wallets-min.png)


<p id="cch-hands_management">&nbsp;</p>

## Управление руками
- Это все работники форка блокчейна
- Вы можете убрать одну руку, если больше не планируете ее фармить


<p id="cch-transfer_coins">&nbsp;</p>

## Переводные монеты
- Перейдите на вкладку кошелька и введите свой безопасный пароль для перевода монет.

<p id="cch-cold_wallet">&nbsp;</p>

## Холодный кошелек
- Перейдите на вкладку настроек с вашим безопасным паролем
- Экспорт учетной записи холодного кошелька
  ```
  1. Подготовьте новую машину (отличается от горнодобывающей машины)
  2. Визит https://www.coctohug.xyz и нажмите &#34;Режим кошелька&#34;, чтобы создать папки для создания докеров.
  3. Настройте папки для создания докеров [Настройка Coctohug на ОС Linux]
  4. На экране запуска WebUI на этот раз сгенерируйте новый ключ
  5. Подождите несколько минут для перезапуска форков блокчейна
  6. Зайдите в каждую папку и выполните скрипт docker-compose stop && docker-compose up -d
  7. Визит http://localhost:12630/, и перейдите в настройки - вкладка холодного кошелька, чтобы экспортировать адреса холодного кошелька
  8. Убедитесь, что каждый адрес правильный, сравнивая загруженный файл с информацией, отображаемой на вкладке «Ключи».
  9. Получите 24 мнемонических слова аналогичным скриптом терминала
    docker exec -it coctohug-flora flora keys show --show-mnemonic-seed
    docker exec -it coctohug-covid covid keys show --show-mnemonic-seed
    docker exec -it coctohug-lucky lucky keys show --show-mnemonic-seed
  ```
- Импортировать учетную запись холодного кошелька
  ```
  1. На своей майнинг-машине зайдите в настройки - вкладка холодного кошелька.
  2. Импортируйте ранее загруженный файл json из холодного кошелька (рекомендуется на другой машине).
  3. Подождите несколько минут и перейдите на вкладку кошелька, чтобы узнать, обновлен ли адрес холодного кошелька или нет.
  4. Примечание 1: мы рекомендуем сделать резервную копию конфигурации вашего кошелька перед импортом.
  5. Примечание 2: только рабочие форки блокчейна могут импортировать холодный кошелек. Пожалуйста, проверьте, есть ли остановленные форки блокчейна, прежде чем делать это. Конечно, вы также можете импортировать позже снова, когда они будут перезапущены
  6. Примечание 3: Если есть какие-либо проблемы, вам может потребоваться перезапустить все папки по порядку:
    cd coctohug0 && docker-compose up -d
    cd ../coctohug1 && docker-compose up -d
    cd ../coctohug2 && docker-compose up -d
    cd ../coctohug3 && docker-compose up -d
  ```
![English](../../images/cold_wallet-min.png)



<p id="cch-secure_passphrase">&nbsp;</p>

## 24 мнемонических слова с безопасной парольной фразой
- <a target='_blank' href='https://github.com/raingggg/coctohug-passphrase'>coctohug-passphrase</a> можно использовать для защиты ваших 24 мнемонических слов
- Он шифрует ваши ключи паролем, который знаете только вы
- Вы можете расшифровать его паролем при добавлении новых форков блокчейна.

<p id="cch-forks">&nbsp;</p>

## Форки блокчейна
- Проверяйте coctohug github каждые несколько дней
- Новые форки блокчейна будут поддерживаться очень скоро
  
<p id="cch-harvester">&nbsp;</p>

## Комбайн
- Визит <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a> и нажмите кнопку Harvester Mode, чтобы создать папки для создания докеров.
- Визит <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a> и нажмите Разрешить комбайну установить связь между контроллером и комбайном.
- Настройте папки для создания докеров [Настройка Coctohug на ОС Linux](#cch-linux)
- Через несколько минут вы сможете увидеть комбайн на вкладке рук WebUI.

<p id="cch-upgrade">&nbsp;</p>

## Обновление
- Однострочный сценарий
  ```
  docker-compose stop && docker-compose rm -f && docker-compose pull && docker-compose up -d --force-recreate
  ```
- Вы также можете пошагово выполнить вышеуказанные скрипты.
  ```
  docker-compose stop
  docker-compose rm -f
  docker-compose pull
  docker-compose up -d --force-recreate
  ```
- В случае несовместимой проблемы с базой данных вы можете удалить существующий файл базы данных перед запуском скрипта запуска docker-compose с помощью
  ```
  rm ~/.coctohug-web/db/coctohug.sqlite
  ```

<p id="cch-local_language">&nbsp;</p>

## Местный язык
- В правом верхнем углу WebUI выберите любой язык, который вам нравится больше всего.
- Вы можете переключиться на любой другой язык позже, если захотите
  
  
<p id="cch-hardware_requirements">&nbsp;</p>

## Требования к оборудованию
- После синхронизации процессоров Intel® Core ™ i7 10-го поколения должно хватить для создания более 50 форков блокчейна.
- Однако на этапе начальной синхронизации узла он действительно съедает центральный процессор. Поэтому мы рекомендуем настроить 5 форков блокчейна на группу и начать группировку за группой.
- Требуемая память равна: количество форков блокчейна для майнинга умножается на 1,8 ГБ ОЗУ.
- Нормального диска должно хватить на более чем 50 форков блокчейна.



# Наши проекты с открытым исходным кодом на Github
[webui](https://github.com/raingggg/coctohug-web-docker)

[cactus](https://github.com/raingggg/coctohug-cactus)

[covid](https://github.com/raingggg/coctohug-covid)

[cryptodoge](https://github.com/raingggg/coctohug-cryptodoge)

[ethgreen](https://github.com/raingggg/coctohug-ethgreen)

[flora](https://github.com/raingggg/coctohug-flora)

[greendoge](https://github.com/raingggg/coctohug-greendoge)

[lucky](https://github.com/raingggg/coctohug-lucky) 

[pipscoin](https://github.com/raingggg/coctohug-pipscoin)

[shibgreen](https://github.com/raingggg/coctohug-shibgreen)

[silicoin](https://github.com/raingggg/coctohug-silicoin)

[skynet](https://github.com/raingggg/coctohug-skynet) 

[staicoin](https://github.com/raingggg/coctohug-staicoin)

[stor](https://github.com/raingggg/coctohug-stor)

[tranzact](https://github.com/raingggg/coctohug-tranzact)

[venidium](https://github.com/raingggg/coctohug-venidium)

[btcgreen](https://github.com/raingggg/coctohug-btcgreen)

[hddcoin](https://github.com/raingggg/coctohug-hddcoin)

[maize](https://github.com/raingggg/coctohug-maize)

[flax](https://github.com/raingggg/coctohug-flax)

[aedge](https://github.com/raingggg/coctohug-aedge)

[apple](https://github.com/raingggg/coctohug-apple)

[wheat](https://github.com/raingggg/coctohug-wheat)

[dogechia](https://github.com/raingggg/coctohug-dogechia)

[tad](https://github.com/raingggg/coctohug-tad)

[taco](https://github.com/raingggg/coctohug-taco)

[socks](https://github.com/raingggg/coctohug-socks)

[mogua](https://github.com/raingggg/coctohug-mogua)

[mint](https://github.com/raingggg/coctohug-mint)

[salvia](https://github.com/raingggg/coctohug-salvia)


## Уведомление о товарном знаке
CHIA NETWORK INC, CHIA ™, CHIA BLOCKCHAIN ​​™, CHIA PROTOCOL ™, CHIALISP ™ и «логотип в виде листа» (включая только логотип в виде листа, когда он относится или указывает на Chia) являются товарными знаками или зарегистрированными товарными знаками Chia Network, Inc. ., корпорация Делавэр. * Нет никакой связи между этим проектом Coctohug и основным проектом Chia Network. *