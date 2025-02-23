# فرایند نوشتن RFC

## مقدمه

هر هفته در جلسات تصمیم‌گیری ساختاری برنامه CS Internship، مسائل مختلفی به منظور بهبود مکانیزم‌ها، فرآیندها و سیاست‌های برنامه مطرح می‌شوند و مورد بحث و بررسی قرار می‌گیرند. این مسائل می‌تواند در قالب سوال، پیشنهاد و یا ابهام باشند. هر کدام از این مسئله‌ها توسط یکی از منتورها و یا کاندیدمنتورها در جلسه ساختاری مطرح می‌شوند. در این جلسات، فرد مطرح کننده مسئله به همراه بقیه شرکت کننده‌گان، تیمی را برای بررسی آن موضوع تشکیل می دهد تا به صورت دقیق تر موضوع مورد نظر را جوانب مختلف بررسی و پیگیری کنند و آنرا به سرانجام برسانند.

هر موضوع باز مطرح شده در جلسات ساختاری، مشخصاتی دارد که آن را از بقیه موضوعات متمایز می‌کند. بعلاوه افراد مختلفی در جلسات تشکیل شده برای آن موضوع باز شرکت می‌کنند که ایده‌های متفاوتی برای حل مسئله مطرح‌شده ارائه و بقیه ایده‌ها را نیز مورد بحث و بررسی قرار می‌دهند. بنا بر این در هرجلسه شامل یکسری نتیجه‌گیری‌ها از مسائل مطرح شده و یکسری موضوعات باز برای بررسی‌های بعدی تشکیل خواهد شد. همچنین ممکن از خلال بحث و بررسی‌های انجام شده تعداد کار ایجاد شود تا توسط افراد شرکت کننده انجام شود. این سلسه از جلسات تا زمانی که به جمع بندی نهایی از موضوع اصلی برسند ادامه خواهد داشت و نهایتا یک راه حل به عنوان نتیجه‌گیری نهایی مطرح خواهد شد. این نتیجه‌گیری کلی می‌تواند به اصلاح فرآیند فعلی، ایجاد یک فرآیند جدید یا حذف و جایگزینی فرآیندهای غیرقابل استفاده منجر شود.

پیگیری موضوعات مطرح شده در این جلسات تنها در صورتی موثر خواهد بود که ابتدا تعریف دقیقی از موضوع باز مطرح شده و دلیل مطرح شده آن را در صفحه ای مخصوص به این کار در سیستم OneNote برنامه ثبت کنیم. یادداشت برداری از مسائل، ایده و نتیجه گیری‌های انجام شده در هر کدام از جلسات به مدون بود بحث و گفت گوها حول محور اصلی کمک خواهد کرد و نهایتا تمام اطلاعات مربوط به این موضوع باز برای افرادی که به صورت مستقیم یا غیر مستقیم با این موضوعات درگیر هستند، قابل دسترس خواهد بود. بنا بر این نیاز هست که صفحه‌ای برای این دست از مستندات در OneNote ایجاد کنیم. این صفحه شامل عنوان موضوع باز، فرد مطرح کننده اولیه، تیم پیگیری کننده، افراد شرکت کننده در هر جلسه و خلاصه‌ای از تحلیل و بررسی موضوع در جلسات مختلف است که در قالبی به نام RFC جمع آوری شوند. این قالب در هر لحظه آخرین وضعیت بررسی‌ها انجام شده بر روی آن فرآیند را اطلاع رسانی می‌کند. بنا بر این نیاز هست تا به صورت دقیق و کامل، نوشته و تکمیل شود. در این مستند به نحوه ایجاد قالب RFC در OneNote برای موضوعات باز جلسات ساختاری پرداخته می‌شود.

## مخاطب

مخاطب اصلی این مستند، منتور‌ها و کاندید منتورهایی هستند که در جلسات ساختاری شرکت می‌کنند و نیاز دارند تا بدانند چگونه یک قالب RFCبرای موضوع باز مورد نظر خود ایجاد کنند. همچنین مطالعه این مستند می‌تواند برای آن دسته از دستیار منتور‌ها و کارآموز منتورهایی که به صورت داوطلبانه و منظم در جلسات ساختاری شرکت می‌کنند و نیاز دارند تا به آخرین اطلاعات مربوط موضوعات باز دسترسی داشته باشند نیز مفید است.

## معرفی موضوع

از ابتدای ایجاد برنامه CS Internship، موضوعاتی که برای طراحی، اصلاح و یا حذف یکی از فرآیندها، مکانیزم‌ها و سیاست‌های برنامه موضوعات مختلفی مطرح می‌شد، در یک صفحه مجزا با نام Open Topic در قسمت جلسات هفتگی ایجاد و تکمیل می‌شد. این صفحه شامل قسمت‌های مختلف اعم از عنوان موضوع، جدول حضور غیاب منتورها به تفکیک اسپرینت، شرح موضوع، تاریخ مطرح شدن، فرد مطرح کننده و نتیجه‌گیری می‌شد.

در جدول حضور غیاب منتورها، ردیفی مجزا به ازای هر منتور که در برنامه CS Internship حضور داشت ایجاد می‌شد. در حین اصلاح و طراحی فرآیندهای مختلف اعم از طراحی فرآیند آنبوردینگ منتور جدید و فرآیند خروج منتور از برنامه، متوجه شدیم به ازای ورود یا خروج هر منتور، بایستی یک نفر مسئول اصلاح کردن جدول موجود در صفحه تمپلیت موضوعات باز باشد. بعلاوه در صورتی که تعداد منتورها زیاد باشند، لیست اسامی منتورها، منجر به اتلاف فضای اضافه زیادی از صفحه موضوعات باز می‌شد. از طرفی با بروز رسانی فرآیند مربوط به حضور و شرکت در جلسات ساختاری و ایجاد کارت‌های تسک حضور و غیاب افراد در جلسات بر روی برد Azure برنامه، وجود جدولی طولانی در قالب موضوعات باز عملا بی‌استفاده بود، چون در هر لحظه با مراجعه به اسپرینت مورد نظر بر روی برد، امکان دسترسی به لیست افراد شرکت کننده درجلسه وجود داشت.

بنا بر این اولین تغییری که برای بهینه‌تر کردن قالب موضوعات باز پیشنهاد شد، خذف شدن جدول حضور و غیاب از قالب صفحات مربوط به موضوع باز بود. از طرفی ماهیت موضوع باز به درستی و تنهایی تمام منظور مسائل مطرح شده در قالب موضوع باز را نمی‌رساند. هر موضوع بازی که مطرح می‌شود یکی از فرآیندها ، ممکن است طی مراحل مختلف به روز بررسی و بایستی برای بروز نگه داشتن این جدول، تسکی جداگانه برای که اگر برای منتورها سوال‌هایی در مورد فرایند‌ها یا موضوعاتی که برای آنها فرایندی نداشتیم پیش می‌آمد این سوالات برای بررسی در جلسات ساختاری مطرح می‌شد که در برخی موارد نیاز بود فرایندی تغییر کند یا فرایند جدید ایجاد شود که بعنوان موضوع باز(Open Topic) در One Note ایجاد می‌شد و تمپلیت هر موضوع باز شامل موضوعی که راجع به آن صحبت می‌شد، شرکت‌کنندگان که شامل لیست کاملی از افرادی که می‌بایست در جلسات ساختاری شرکت کنند بود و حضور یا عدم حضور افراد با نوشتن حاضر و غایب مقابل اسم شان مشخص می‌شد. ، توضیح و جزئیات موضوع، تاریخچه موضوع، نظرات شرکت کنندگان در جلسه، نظرات غایبین در جلسه و نتیجه‌گیری بود.

حین طراحی فرایند خروج منتور از دوره نیاز بود، اطلاعات منتوری که قصد خروج را دارد از مستندات برنامه CS Internship حذف شود یکی از این موارد لیست حاضرین جلسات ساختاری در تمپلیت موضوع باز بود. باتوجه به اینکه در حال حاضر برای حضور افراد در جلسات تسک‌های بخصوصی در بک لاگ Governance Meeting Participation در هر جلسه اسپرینت ایجاد و ثبت می‌شود بنابراین وجود این لیست در تمپلیت موضوع باز نیاز نیست.

از لیست حاضرین جلسات ساختاری برای پیگیری حضور و غیاب افراد در جلسه استفاده می‌شده که با توجه به فرآیندهایی که بعد از ایجاد این لیست شکل گرفته و پیاده‌سازی شدند (پیگیری حضور شرکت‌کننده‌ها از طریق بُرد)، پیشنهاد این که این لیست را از این بخش حذف کنیم و قالب را سامان‌دهی کنیم، داده شد و در ادامه تغییر این فرایند تمپلیت موضوع باز (Open Topic) به تمپلیت RFC تغییر کرد.

موضوعات Open Topic سوال، ابهام و پیشنهاد بود که با تغییر تمپلیت به RFC (مخفف Request For Comments)، موضوعاتی که در این قالب مطرح می‌شوند، موضوعاتی هستند که در برنامه CS Internship فرایندی برای آنها نداریم و برای بررسی اینگونه مسائل از تمپلیت RFC استفاده می‌کنیم و گاهی ممکن است برای حل این مسائل چندین فرایند عوض شود یا چندین داکیومنت به‌روزرسانی شود.

در حال حاضر تمپلیت موضوع باز با توجه به تغییراتی که نیاز بود اعمال شود به تمپلیت RFC تغییر یافت که خیلی مرتب‌تر و بهینه تر شد.

## شرح جزئیات

تمپلیت RFC دارای بخش‌های زیر می‌باشد:

### شناسنامه

![Picture1](https://github.com/Ali-Sdg90/cs-internship-spec/assets/115698554/e3ddb909-6b42-41dd-a60b-35d3f18b2ddc)

تصویر ۱

- **مطرح کننده اولیه:** فردی که برای اولین بار موضوع RFC مربوطه را مطرح می‌کند. مطرح کننده اولیه می‌تواند از افراد شرکت کننده در جلسات عملیاتی باشد که برای موضوعی که مطرح کرده است، باید یکی از منتورها یا کاندید منتورها متقاعد کند تا موضوع مورد نظر را در جلسه ساختاری مطرح کند و یا می‌تواند منتور یا کاندید منتوری باشد که مسئله مورد نظرش را در جلسه ساختاری مطرح می‌کند.
- **تاریخ مطرح شدن:** تاریخی که موضوع در جلسات ساختاری مطرح می‌شود(تاریخ باید شمسی باشد).
- **تیم طراحی:** تیمی که برای پیگیری و پیاده سازی فرایند ایجاد شده تشکیل می‌شود.
- **لینک صفحه طراحی:** گاهی نیاز هست که برای طراحی برخی فرایند‌ها از ابزارهایی مانند Miro برای طراحی نمودار فرآیند و یا صفحه‌ای جدید در سیستم OneNote برای مستند سازی استفاده شود که لینک آن‌ها در این بخش قرار می‌گیرد.
- **لینک بک لاگ:** لینک بک لاگی که در آن تسک‌های این فرایند ایجاد شده است.

### شرح موضوع

در این قسمت توضیحات RFC ای که در جلسه ساختاری مطرح و مورد بحث و بررسی قرار می‌گیرد بیان می‌شود.

### جلسه۱ – اسپرینت \[شماره اسپرینت\]

محتوای جلسه می‌تواند شامل قسمت‌های زیر باشد:

- **شرکت کنندگان:** نام همه افرادی که در جلسه ساختاری و هنگام مطرح شدن این موضوع حضور داشتند.
- **خلاصه صحبت‌ها و نحوه رسیدن به نتیجه:** جمع بندی صحبت‌ها و موارد مطرح شده‌ و نتیجه‌گیری از انها.
- **نتیجه جلسه:** نتیجه جلسه شامل قسمت‌های زیر است:

1. **موارد قطعی شده:** مواردی که بعد از بحث و بررسی نتیجه‌گیری شده و قطعی شده است.
2. **تسک‌هایی که باید انجام شود:** برای مواردی که قطعی شده ممکن است تسک‌هایی ایجاد شود که در قالب جدول (تصویر ۲) است.

![Picture2](https://github.com/Ali-Sdg90/cs-internship-spec/assets/115698554/2d99c1c6-b1f9-49c7-a2dc-864234acd5da)

تصویر ۲

در قسمت تسک عنوان تسک‌ها نوشته می‌شود.

در قسمت مسئول اسم فردی نوشته می‌شودکه مسئول انجام تسک است.

1. **موضوع باز برنامه جلسه بعد:** ممکن است RFC مطرح شده در یک اسپرینت موجب ایجاد RFC های جدید شود که در جلسات بعدی مورد بررسی قرار گیرد.

ممکن است RFC ای در یک اسپرینت بصورت کامل مورد بحث و بررسی قرار نگیرد و تمام نشود و نیاز باشد در اسپرینت‌های بعدی ادامه یابد در اینصورت باید تایتل **جلسه۲ – اسپرینت \[شماره اسپرینت\]** استفاده شود.

## نحوه ایجاد بک لاگ RFC

برای ایجاد بک لاگ RFC ایتدا در azure DevOps در بخش Boards روی backlogs کلیک کرده و مطمن شوید Team Backlogs روی CS Internship Program Team باشد(در تصویر ۳ با دایره قرمز مشخص شده است).

![Picture3](https://github.com/Ali-Sdg90/cs-internship-spec/assets/115698554/2ae721d5-fd8f-4f5f-a0af-5a4b717b4d34)

تصویر ۳

میتوانید از تصویر برای پیدا کردن ادرس بک لاگ ها استفاده کنید.

در ادامه روند ایجاد کردن بک لاگ بعد از رفتن به صفحه مربوطه میتوانید از بخش CS Internship Governance به بخش RFCs بروید و روی بک لاگ \[TEMPLATE\] RFC: \[TITLE\] کلیک کنید که با تصویر زیر مواجه می شوید (تصویر ۴).

![Picture4](https://github.com/Ali-Sdg90/cs-internship-spec/assets/115698554/8693a40a-49b6-4bac-ab16-842408315f4e)


تصویر ۴

در مرحله اول شما باید در قسمت بالا سمت راست گزینه سه نقطه را کلیک کرده و در بین گزینه هایی که میبیند بخش create a copy of work item را کلیک کنید تا یک کپی از تمپلیت بسازد(قسمت قرمز تصویر ۴) . هنگامی که روی این گزینه کلیک کرده اید یک صفحه ای باز می‌شود که باید سه تا گزینه که در تصویر(تصویر ۵) را فعال کنید تا کپی ایجاد شده شامل تمامی لینک‌های موجود، ضمیمه‌های موجود و تمامی زیر آیتم‌های کاری شود. (با دایره قرمز مشخص شده است ) :

![Picture5](https://github.com/Ali-Sdg90/cs-internship-spec/assets/115698554/8ce917d3-e6f6-4e61-98ef-2c4647e5c41b)

تصویر ۵

سپس مراحل زیر را برای ایجاد RFC جدید انجام دهید:

ایتدا باید قسمت \[TEMPLATE\] را حذف کرده و در قسمت \[TITLE\] موضوع RFC را بنویسید و قسمت Unassigned را به کسی که این RFC را مطرح کرده اساین کنید.

بخش state را روی گزینه Committed قرار دهید و بخش iteration هم باید اسپرینتی که این بک لاگ ایجاد شده باشد و قسمت Area را روی گزینه Governance قرار دهید.

## آموزش‌دهنده‌ها

تمامی منتور‌ها و کاندید منتور‌هایی که حداقل یکبار این فرایند را انجام داده باشند.

## نحوه آموزش

منتورها و کاندید منتورهایی که نوشتن RFC را آموزش می‌دهند باید از خوانده شدن مستند‌های [شرکت در جلسات ساختاری‌](https://mehransystems.sharepoint.com/sites/CSInternship/MentorDocs/Processes/Mentoring%20Intern%20Processes/CSI%20-%20Process%20-%20Attend%20and%20Observe%20Structural%20Meetings%20-%20Farsi.pdf) و‌ همچنین [مدیریت جلسات ساختاری](https://mehransystems.sharepoint.com/sites/CSInternship/MentorDocs/Processes/Mentor%20Processes/CSI%20-%20Process%20-%20Managing%20Governance%20Meeting%20-%20Farsi.pdf) توسط فرد یادگیرنده مطمئن شوند.

## واژه‌نامه

**• موضوع باز:** ایرادات، ابهامات و یا ایده‌های جدیدی که در خلال انجام وظایف هفتگی در ذهن کارآموزمنتورها، دستیارمنتورها و منتورها ایجاد می‌شود که هدف از رسیدگی به آن‌ها، بهینه‌سازی فرآیندهای موجود در برنامه CS Internship است.

**• کاندیدمنتور:** فردی که منتور نشده ولی می‌تواند یکسری از کارهای منتوری مثل شرکت در جلسات ساختاری و پیش بردن RFC را انجام دهد.
