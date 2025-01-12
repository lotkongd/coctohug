# Coctohug - ده ها چنگال بلاک چین چیا را که از یک مرورگر وب استخراج می کنند را مدیریت کنید!
- بومی سازی خوب با پشتیبانی از ده ها زبان: [English](./wiki_en.md), [العربية](./wiki_ar.md), [Bulgarian](./wiki_bg.md), [Catalan](./wiki_ca.md), [Deutsch](./wiki_de.md), [Español](./wiki_es.md), [زبان فارسی](./wiki_fa.md), [Français](./wiki_fr.md), [Galego](./wiki_gl.md), [Indonesian](./wiki_id.md), [Italiano](./wiki_it.md), [日本語](./wiki_ja.md), [한국어](./wiki_ko.md), [Português do Brasil](./wiki_pt.md), [limba română](./wiki_ro.md), [Русский](./wiki_ru.md), [Serbian](./wiki_sr.md), [Thai](./wiki_th.md), [Tagalog (Filipino)](./wiki_tl.md), [Türkçe](./wiki_tr.md), [Українська](./wiki_uk.md), [Vietnamese](./wiki_vi.md), [简体中文](./wiki_zh-CN.md), [繁體中文](./wiki_zh-TW.md)

راه اندازی آسان با استفاده از [شروع سریع](https://www.coctohug.xyz/)

*از ما کمک بیشتری بخواهید [Website](https://www.coctohug.xyz/) / [Github](https://github.com/raingggg/coctohug) / [Discussions](https://github.com/raingggg/coctohug/discussions) / [Discord](https://discord.gg/umfKHm7gVM)*.

# شروع سریع
  - [راه اندازی Coctohug در سیستم عامل لینوکس](#cch-linux)
  - [Coctohug را در سیستم عامل ویندوز راه اندازی کنید](#cch-windows)
  - [راه اندازی Coctohug در سیستم عامل مک](#cch-macOS)
  

# تنظیمات مشترک
  - [کلمه عبور](#cch-password)
  - [کلیدها](#cch-keys)
  - [معدن](#cch-farming)
  - [نظارت بر](#cch-monitoring)
  - [بازیابی NFT](#cch-nft_recovery)
  - [بلوک پیدا شد / سکه دریافت شد](#cch-blocks_found)
  - [هشدارهای معدن](#cch-farming_warnings)
  - [گزارش روزانه](#cch-daily_report)
  - [گزارش هفتگی](#cch-weekly_report)
  - [همگام سازی گره](#cch-node_sync)
  - [مدیریت اتصالات](#cch-connections_management)
  - [مدیریت کیف پول](#cch-wallets_management)
  - [مدیریت دست](#cch-hands_management)
  - [انتقال سکه](#cch-transfer_coins)


# تنظیمات پیشرفته
  - [کیف پول سرد](#cch-cold_wallet)
  - [رمز عبور امن 24 کلمه یادگاری](#cch-secure_passphrase)
  - [فورک های بلاک چین](#cch-forks)
  - [دروگر](#cch-harvester)
  - [ارتقا دهید](#cch-upgrade)

# بهترین شیوه ها
  - [زبان محلی](#cch-local_language)
  - [الزامات سخت افزاری](#cch-hardware_requirements)

<p id="cch-linux">&nbsp;</p>

## راه اندازی Coctohug در سیستم عامل لینوکس
- برپایی <a target='_blank' href='https://www.docker.com/products/docker-desktop'>Docker</a> + <a target='_blank' href='https://docs.docker.com/compose/install/'>Docker-Compose</a> 
- به سایت بروید <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a>, سپس تمام فیلدهای فرم لازم را وارد کرده و فایل های زیپ شده docker-compose تولید شده را دانلود کنید
- پوشه های دانلود شده را از حالت فشرده خارج کنید و آنها را در پوشه کاری خود کپی کنید
- همه پوشه ها را به ترتیب اجرا کنید:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- مرورگر را باز کنید و با url به WebUI دسترسی پیدا کنید <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- نکته 1: بیش از 5 فورک بلاک چین را همزمان راه اندازی نکنید، زیرا فورک های بلاک چین چیا هنگام همگام سازی گره برای اولین بار CPU را می خورند.
- نکته 2: برای هر فورک بلاک چین حدود 1.8 گیگ رم لازم است، بنابراین چند فورک بلاک چین را بر اساس حافظه رایانه خود انتخاب کنید.
- نکته 3: در صورت وجود هر گونه مشکل، ممکن است لازم باشد همه پوشه ها را به ترتیب مجدد اجرا کنید:
  ```
  cd coctohug0 && docker-compose up -d
  cd ../coctohug1 && docker-compose up -d
  cd ../coctohug2 && docker-compose up -d
  cd ../coctohug3 && docker-compose up -d
  ...
  ```
- نکته 4: ممکن است لازم باشد پورت های مجاز از 12630 تا 12700 را به تنظیمات فایروال سیستم خود اضافه کنید.



<p id="cch-windows">&nbsp;</p>

## Coctohug را در سیستم عامل ویندوز راه اندازی کنید
- مشابه با [راه اندازی Coctohug در سیستم عامل لینوکس](#cch-linux)

<p id="cch-macOS">&nbsp;</p>

## راه اندازی Coctohug در سیستم عامل مک
- مشابه با [راه اندازی Coctohug در سیستم عامل لینوکس](#cch-linux)

<p id="cch-password">&nbsp;</p>

## کلمه عبور
- هنگامی که برای اولین بار با URL به WebUI دسترسی پیدا می کنید، از شما خواسته می شود یک رمز عبور برای تنظیمات ایمن تنظیم کنید <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a>
- تنظیمات ایمن عبارتند از: کیف پول سرد، انتقال سکه، راه اندازی مجدد فورک های بلاک چین، دروگر...

<p id="cch-keys">&nbsp;</p>

## کلیدها
- هنگامی که برای اولین بار با URL به WebUI دسترسی پیدا می کنید، از شما خواسته می شود 24 کلمه یادگاری را وارد کنید - این عمدتا برای اهداف کشاورزی است.
- یا می توانید یک کلید کاملاً جدید ایجاد کنید - این عمدتاً برای اهداف کیف پول سرد است

<p id="cch-farming">&nbsp;</p>

## معدن
- هنگامی که همگام سازی گره انجام شد، کشاورزی باید به طور خودکار شروع شود
- سپس می توانید وضعیت استخراج را با روش های مختلف نظارت کنید

![English](../../images/coctohug-summary-en-min.png)

<p id="cch-monitoring">&nbsp;</p>

## نظارت بر
- برگه خلاصه می تواند موارد زیر را نشان دهد: مجموع سکه های استخراج شده، موجودی حساب، تعداد قطعه، اندازه قطعه، اندازه Netspace و زمان مورد انتظار برای برنده شدن
- هر چنگال-پنل بلاک چین در تب Summary اگر خوب کار کند پس زمینه سبز روشن خواهد داشت، در غیر این صورت پس زمینه زرد روشن خواهد بود.
- شما همچنین می توانید جزئیات را با استفاده از برگه های دیگر بررسی کنید

<p id="cch-nft_recovery">&nbsp;</p>

## بازیابی NFT
- برگه سکه های دریافتی دارای پیوند است: <a class="nav-link" target="_blank" href="https://alltheblocks.net/nft-recovery">جوایز NFT 7/8 خود را مطالبه کنید</a>

<p id="cch-blocks_found">&nbsp;</p>

## بلوک پیدا شد / سکه دریافت شد
- کل بلوک های یافت شده را فهرست کنید
- کل سکه های دریافتی را فهرست کنید

![English](../../images/received-coins-min.png)


<p id="cch-farming_warnings">&nbsp;</p>

## هشدارهای معدن
- مشکل احتمالی شبکه را فهرست کنید
- مشکل احتمالی نشانه را فهرست کنید
- مشکل احتمالی جستجوی دیسک را فهرست کنید
- مشکل احتمالی کاهش تعداد نمودار را فهرست کنید

<p id="cch-daily_report">&nbsp;</p>

## گزارش روزانه
- خلاصه بلوک های یافت شده / سکه های دریافت شده در روز
- خلاصه هشدارهای معدن در روز

![English](../../images/daily_report-min.png)


<p id="cch-weekly_report">&nbsp;</p>

## گزارش هفتگی
- خلاصه بلوک های یافت شده / سکه های دریافت شده در هفته
- هشدارهای معدن را به صورت هفته خلاصه کنید

<p id="cch-node_sync">&nbsp;</p>

## همگام سازی گره
- Node به طور پیش فرض به طور خودکار همگام می شود
- برای بررسی وضعیت دقیق می توانید به تب Connections یا Blockchains بروید
- برای تسریع همگام سازی گره خود، [https://alltheblocks.net/](https://alltheblocks.net/) لیست گره ها و فایل پایگاه داده را ارائه می دهد (روی هر بلاک چین کلیک کنید و سپس می توانید آنها را در قسمت بالا سمت راست پیدا کنید)

<p id="cch-connections_management">&nbsp;</p>

## مدیریت اتصالات
- تمام اتصالات گره را فهرست کنید
- می توانید اتصالات را در تب Connections اضافه یا حذف کنید

![English](../../images/connections-min.png)


<p id="cch-wallets_management">&nbsp;</p>

## مدیریت کیف پول
- وضعیت کیف پول و موجودی حساب را فهرست کنید
- همچنین می توانید سکه ها را در تب کیف پول انتقال دهید

![English](../../images/wallets-min.png)


<p id="cch-hands_management">&nbsp;</p>

## مدیریت دست
- این هر کارگر فورک بلاک چین است
- زمانی که دیگر قصد کشاورزی ندارید، می توانید یک دست را بردارید


<p id="cch-transfer_coins">&nbsp;</p>

## انتقال سکه
- به تب کیف پول بروید و رمز عبور امن خود را برای انتقال سکه وارد کنید

<p id="cch-cold_wallet">&nbsp;</p>

## کیف پول سرد
- با رمز عبور امن خود به تب تنظیمات بروید
- صادرات حساب کیف پول سرد
  ```
  1. یک ماشین جدید (متفاوت با ماشین معدن) آماده کنید
  2. بازدید کنید https://www.coctohug.xyz و برای ایجاد پوشه های docker-compose روی Wallet Mode کلیک کنید
  3. پوشه های docker-compose را راه اندازی کنید [راه اندازی Coctohug در سیستم عامل لینوکس]
  4. در صفحه راه اندازی WebUI، این بار یک کلید جدید ایجاد کنید
  5. چند دقیقه صبر کنید تا فورک های بلاک چین راه اندازی مجدد شوند
  6. به هر پوشه بروید و اسکریپت را اجرا کنید docker-compose stop && docker-compose up -d
  7. بازدید کنید http://localhost:12630/, و به تنظیمات - تب سرد کیف پول بروید تا آدرس های کیف پول سرد را صادر کنید
  8. با مقایسه فایل دانلود شده با اطلاعات نشان داده شده در برگه کلیدها، صحت هر آدرس را به صورت دستی تأیید کنید
  9. با اسکریپت ترمینال مشابه، 24 کلمه یادگاری دریافت کنید
    docker exec -it coctohug-flora flora keys show --show-mnemonic-seed
    docker exec -it coctohug-covid covid keys show --show-mnemonic-seed
    docker exec -it coctohug-lucky lucky keys show --show-mnemonic-seed
  ```
- وارد کردن حساب کیف پول سرد
  ```
  1. در دستگاه ماینینگ خود، به تنظیمات - تب کیف پول سرد مراجعه کنید
  2. فایل json کیف پول سرد دانلود شده قبلی (توصیه شده در دستگاه های مختلف) را وارد کنید
  3. چند دقیقه صبر کنید و به تب کیف پول بروید تا ببینید آیا آدرس کیف پول سرد به روز شده است یا خیر
  4. نکته 1: توصیه می کنیم قبل از وارد کردن، از تنظیمات کیف پول خود نسخه پشتیبان تهیه کنید
  5. نکته 2: فقط چنگال های بلاک چین فعال می توانند کیف پول سرد وارد کنند. لطفاً قبل از انجام این کار بررسی کنید که آیا فورک های بلاک چین متوقف شده است یا خیر. مطمئناً می‌توانید بعداً با راه‌اندازی مجدد آنها دوباره وارد کنید
  6. نکته 3: در صورت وجود هر گونه مشکل، ممکن است لازم باشد همه پوشه ها را به ترتیب مجدد اجرا کنید:
    cd coctohug0 && docker-compose up -d
    cd ../coctohug1 && docker-compose up -d
    cd ../coctohug2 && docker-compose up -d
    cd ../coctohug3 && docker-compose up -d
  ```
![English](../../images/cold_wallet-min.png)



<p id="cch-secure_passphrase">&nbsp;</p>

## رمز عبور امن 24 کلمه یادگاری
- <a target='_blank' href='https://github.com/raingggg/coctohug-passphrase'>coctohug-passphrase</a> می توان برای ایمن سازی 24 کلمه یادداشتی خود استفاده کرد
- کلیدهای شما را با رمزی که فقط شما می دانید رمزگذاری می کند
- هنگام اضافه کردن فورک های بلاک چین جدید، می توانید آن را با رمز عبور رمزگشایی کنید

<p id="cch-forks">&nbsp;</p>

## فورک های بلاک چین
- هر چند روز یکبار گیتهاب کوکتوگ را چک کنید
- فورک های جدید بلاک چین به زودی پشتیبانی خواهند شد
  
<p id="cch-harvester">&nbsp;</p>

## دروگر
- بازدید کنید <a target='_blank' href='https://www.coctohug.xyz/'>https://www.coctohug.xyz</a> و برای ایجاد پوشه های docker-compose روی Harvester Mode کلیک کنید
- بازدید کنید <a target='_blank' href='http://localhost:12630/'>http://localhost:12630/</a> و روی Allow Harvester کلیک کنید تا پیوند بین کنترلر و دروگر ایجاد شود
- پوشه های docker-compose را راه اندازی کنید [راه اندازی Coctohug در سیستم عامل لینوکس](#cch-linux)
- چند دقیقه بعد، می‌توانید در برگه دست‌های WebUI، دروگر را ببینید

<p id="cch-upgrade">&nbsp;</p>

## ارتقا دهید
- اسکریپت یک خطی
  ```
  docker-compose stop && docker-compose rm -f && docker-compose pull && docker-compose up -d --force-recreate
  ```
- همچنین می توانید اسکریپت های بالا را مرحله به مرحله اجرا کنید
  ```
  docker-compose stop
  docker-compose rm -f
  docker-compose pull
  docker-compose up -d --force-recreate
  ```
- در صورت بروز مشکل db ناسازگار، می توانید فایل پایگاه داده موجود را قبل از اجرای اسکریپت شروع docker-compose حذف کنید.
  ```
  rm ~/.coctohug-web/db/coctohug.sqlite
  ```

<p id="cch-local_language">&nbsp;</p>

## زبان محلی
- در سمت راست بالای WebUI، هر زبانی را که بیشتر دوست دارید انتخاب کنید
- در صورت تمایل می توانید بعداً به هر زبان دیگری تغییر دهید
  
  
<p id="cch-hardware_requirements">&nbsp;</p>

## الزامات سخت افزاری
- پس از همگام سازی، پردازنده های نسل دهم Intel® Core™ i7 باید برای پرورش بیش از 50 فورک بلاک چین کافی باشد.
- با این حال، برای مرحله همگام سازی گره اولیه، واقعا CPU را می خورد. بنابراین توصیه می کنیم برای هر گروه 5 فورک بلاک چین راه اندازی کنید و گروه به گروه شروع کنید
- حافظه مورد نیاز برابر است با: تعداد فورک های استخراج بلاک چین، ضربدر 1.8G RAM
- دیسک معمولی باید برای فورک های بلاک چین بیش از 50 مناسب باشد



# پروژه های منبع باز ما در Github
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


## اعلامیه علامت تجاری
CHIA NETWORK INC، CHIA™، CHIA BLOCKCHAIN™، CHIA PROTOCOL™، CHIALISP™ و &#34;لوگوی برگ&#34; (شامل لوگوی برگ به تنهایی هنگامی که به Chia اشاره یا نشان می دهد)، علائم تجاری یا علائم تجاری ثبت شده Chia Network, Inc هستند. .، یک شرکت دلاور. *هیچ وابستگی بین این پروژه Coctohug و پروژه اصلی Chia Network وجود ندارد.*