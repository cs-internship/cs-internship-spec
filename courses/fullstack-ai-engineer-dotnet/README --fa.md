# دوره‌ی Full-Stack AI Engineer (.NET)

[English version](README.md)

## مقدمه

دوره‌ی Full-Stack AI Engineer (.NET) مسیری یکپارچه است که اینترن را از نخستین برنامه‌های زبان C# تا ساخت اپلیکیشن‌های وب مبتنی بر هوش مصنوعی در دات‌نت همراهی می‌کند. در این مسیر، اینترن زبان C#، توسعه‌ی بک‌اند با ASP.NET Core، توسعه‌ی فرانت‌اند با Blazor و افزودن قابلیت‌های هوش مصنوعی به اپلیکیشن‌ها با Microsoft Extensions AI و Microsoft Agent Framework را فرا می‌گیرد. هم‌زمان، استفاده از خود هوش مصنوعی برای پژوهش، یادگیری، تولید محتوا و توسعه‌ی نرم‌افزار آموزش داده می‌شود؛ به‌گونه‌ای که اینترن خروجی مدل‌ها را راستی‌آزمایی کند و مسئولیت تصمیم‌ها همواره بر عهده‌ی انسان باقی بماند.

این دوره برای اینترن‌های جدید جایگزین دوره‌های C# و Machine Learning می‌شود. اینترن‌هایی که پیش‌تر یکی از آن دو دوره را آغاز کرده‌اند، همان دوره را تا پایان ادامه می‌دهند.

## مخاطب

این مستند برای اینترن‌هایی نوشته شده است که دوره‌ی Full-Stack AI Engineer (.NET) را آغاز می‌کنند و همچنین برای منتورهایی که این دوره را هدایت و بازبینی می‌کنند. محتوای استپ‌ها به زبان انگلیسی نوشته شده است، زیرا منابع آموزشی دوره انگلیسی‌اند؛ فرایندهای برنامه در مستندات فارسی CS Internship توضیح داده شده‌اند.

## معرفی دوره

این دوره از دو منبع ساخته شده است: [دوره‌ی C#](../csharp/README.md) همین مخزن و [CrystaCode Full-Stack AI Bootcamp](https://github.com/CrystaCode/full-stack-ai-bootcamp) که تحت مجوز MIT منتشر شده است. بوت‌کمپ برای افرادی طراحی شده بود که دوره‌ی C# را پیش‌تر گذرانده‌اند؛ به همین دلیل، در این دوره مطالب C# در کنار موضوعات بوت‌کمپ و به ترتیبی چیده شده‌اند که پیش‌نیاز هر موضوع پیش از خود آن آموزش داده شود.

اینترن در طول دوره یک اپلیکیشن نمونه‌کار (portfolio) را از استپ اول تا پروژه‌ی پایانی می‌سازد و گسترش می‌دهد. این رویکرد مهارتی را تمرین می‌دهد که در محیط کار واقعی اهمیت دارد: توسعه‌ی تدریجی یک محصول واحد، مستندسازی تصمیم‌ها و ارائه‌ی شواهد قابل‌بررسی برای هر تغییر.

## ساختار دوره

دوره چهارده استپ دارد. سه استپ نخست بر زبان C# تمرکز دارند و هم‌زمان پژوهش و تولید محتوا با هوش مصنوعی و نیز HTML و CSS را آغاز می‌کنند. کار با ASP.NET Core از استپ چهارم، کار با Blazor از استپ پنجم و افزودن هوش مصنوعی به اپلیکیشن‌های دات‌نت از استپ نهم آغاز می‌شود.

| استپ | عنوان | تمرکز اصلی |
|---|---|---|
| ۱ | [Introduction, AI Foundations, and HTML](01-Introduction-AI-Foundations.md) | مقدمات C# و Git، مبانی هوش مصنوعی مولد و راستی‌آزمایی خروجی مدل‌ها، صفحه‌ی HTML محصول |
| ۲ | [Types, Generics, and Learning with AI](02-Types-Generics-Learning-With-AI.md) | انواع داده و جنریک‌ها، اشکال‌زدایی، یادگیری و پژوهش با ابزارهای هوش مصنوعی |
| ۳ | [Collections, Inheritance, and Verified Content](03-Collections-Inheritance-Content.md) | کالکشن‌ها و وراثت، تولید محتوای راستی‌آزمایی‌شده، استایل‌دهی با CSS |
| ۴ | [Delegates, Lambdas, and the First Web API](04-Delegates-Lambdas-Web-API.md) | دلیگیت‌ها و لامبداها، مقدمه‌ی async و await، نخستین اپلیکیشن ASP.NET Core، میان‌افزارها و Minimal API |
| ۵ | [Object Lifetime, Exceptions, and the First Blazor App](05-Object-Lifetime-Exceptions-Blazor.md) | چرخه‌ی عمر اشیا و استثناها، مسیریابی و اعتبارسنجی، چیدمان با Flexbox و Grid، نخستین صفحات Blazor |
| ۶ | [LINQ, Asynchronous Programming, and Component Architecture](06-LINQ-Async-Components.md) | LINQ و برنامه‌نویسی ناهمگام، تزریق وابستگی و پیکربندی، کامپوننت‌های Blazor، مهندسی زمینه (context) |
| ۷ | [Modern C# and Persistent Applications](07-Modern-CSharp-Persistence.md) | ویژگی‌های جدید C#، ذخیره‌سازی داده با EF Core، مستندسازی API، طراحی واکنش‌گرا |
| ۸ | [Controllers, Rendering, Identity, and Navigation](08-Controllers-Rendering-Identity.md) | کنترلرها و فیلترها، احراز هویت و مجوزدهی، رندر و مسیریابی در Blazor |
| ۹ | [Forms, Observability, and the First AI Feature](09-Forms-Observability-First-AI-Feature.md) | فرم‌ها و اعتبارسنجی، لاگ‌برداری ساختاریافته، نخستین قابلیت هوش مصنوعی |
| ۱۰ | [Agent-Assisted Integration](10-Agent-Assisted-Integration.md) | توسعه با کمک ایجنت‌ها، فراخوانی APIهای خارجی، JavaScript Interop، نخستین ایجنت محصول |
| ۱۱ | [Reliable and Automated Workflows](11-Reliable-Automated-Workflows.md) | پردازش پس‌زمینه، آزمون خودکار، گردش‌کارهای چندمرحله‌ای ایجنت |
| ۱۲ | [Agent Tools, Skills, and Coordination](12-Agent-Tools-Skills-Coordination.md) | ابزارهای ایجنت و MCP، مهارت‌های قابل‌استفاده‌ی مجدد، هماهنگی چند ایجنت |
| ۱۳ | [Production AI Applications](13-Production-AI-Applications.md) | آماده‌سازی برای محیط عملیاتی، امنیت، .NET Aspire، رابط کاربری مولد |
| ۱۴ | [Integrated Capstone](14-Integrated-Capstone.md) | انتشار نسخه‌ی نهایی، گردآوری شواهد نمونه‌کار، ارائه و دفاع از محصول |

## نحوه‌ی انجام هر استپ

هر استپ دو بخش دارد: منابع مطالعه (Study Items) و تسک‌ها (Tasks). تسک‌های برگرفته از بوت‌کمپ هدف (Goal)، خروجی (Deliverable)، الزامات (Requirements)، معیارهای پذیرش (Acceptance criteria) و شواهد ارسالی (Submission) را مشخص می‌کنند. چنین تسکی زمانی کامل است که همه‌ی معیارهای پذیرش آن برآورده شده باشد. اینترن در هر استپ لینک کامیت مربوط به آن استپ در مخزن اپلیکیشن نمونه‌کار را نیز ارسال می‌کند.

این دوره از همان فرایندهای سایر دوره‌های CS Internship پیروی می‌کند:

- **کارگاه‌های مربی‌گری:** استپ‌های ۱ تا ۹ با دو ویدئوی مسیر Mentor Training آغاز می‌شوند. روش تماشای ویدئوها، نوشتن گزارش و شرکت در کارگاه‌ها در مستند [شرکت در کارگاه‌های مربی‌گری](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Mentoring%20Workshops%20--%20fa.md) توضیح داده شده است.
- **پست در شبکه‌های اجتماعی:** برای هر Study Item و هر تسک، پست‌های لازم مطابق مستند [پست‌نویسی و پست‌گذاری در شبکه‌های اجتماعی](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Writing%20and%20Publishing%20Posts%20on%20Social%20Media%20--%20fa.md) منتشر می‌شود. هشتگ‌های این دوره `#fullstack_ai #dotnet` هستند و در هر جایی که مستندات برنامه نام دوره را می‌خواهند با هم به کار می‌روند؛ برای نمونه `#cs_internship #fullstack_ai #dotnet #step1` در پست‌ها، پیام تعهد و معرفی‌های [استپ صفر](../Step%200.md) و `#cs_internship #fullstack_ai #dotnet #step_1` در کپشن ارائه.
- **تخمین مهلت استپ:** مهلت هر استپ با روش مستند [روش پیشنهادی برنامه CS Internship برای تخمین و مدیریت زمان انجام استپ‌ها](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Proposed%20Method%20of%20Estimating%20Steps%20in%20the%20CS%20Internship%20Program%20--%20fa.md) برآورد و اعلام می‌شود.
- **گزارش روزانه:** گزارش کار روزانه مطابق مستند [نوشتن و ارسال گزارش کار روزانه](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Writing%20Daily%20Report%20--%20fa.md) ارسال می‌شود.
- **جلسه‌ی فنی و ارائه:** پیش از هر ارائه، اینترن مطابق مستند [شرکت در جلسات فنی و همیاری فنی](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Attending%20Technical%20and%20Technical%20Assistance%20Sessions%20--%20fa.md) در یک جلسه‌ی فنی شرکت می‌کند. هر استپ با یک ارائه‌ی زنده در لینکدین پایان می‌یابد که روش آن در مستند [ارائه آنلاین](https://github.com/cs-internship/cs-internship-spec/blob/master/processes/Intern%20documents/Delivering%20an%20Online%20Presentation%20--%20fa.md) آمده است.

## استفاده از هوش مصنوعی

در این دوره، هوش مصنوعی ابزاری برای پژوهش، یادگیری، تولید محتوا و توسعه است و جایگزین قضاوت انسانی نیست. اینترن خروجی‌های مهم مدل را با منابع معتبر راستی‌آزمایی می‌کند، بررسی‌ها و اصلاحات خود را ثبت می‌کند و مسئولیت هر تصمیم و هر تغییری را که می‌پذیرد بر عهده دارد. اطلاعات محرمانه، کلیدها و داده‌های خصوصی نباید در اختیار ابزارهای هوش مصنوعی قرار گیرد.

رابط محصولات، طرح‌های اشتراک، دسترسی منطقه‌ای و کتابخانه‌های هوش مصنوعی به‌سرعت تغییر می‌کنند. اگر محصولی که در یک استپ نام برده شده است در دسترس نباشد، اینترن با تأیید منتور فنی خود از جایگزینی معادل استفاده می‌کند و این جایگزینی را مستند می‌کند. در کارهای حساس به نسخه در حوزه‌ی هوش مصنوعی دات‌نت، ویدئوها نمایش مفهومی به شمار می‌روند و APIها، وضعیت بسته‌ها و نمونه‌کدها باید پیش از پیاده‌سازی با مستندات رسمی و به‌روز تطبیق داده شوند.

## منابع و انتساب

- [Programming C# 12.0](https://www.oreilly.com/library/view/programming-c-12/9781098158354/)
- [ASP.NET Core in Action, Third Edition](https://www.manning.com/books/asp-net-core-in-action-third-edition)
- [Blazor University](https://blazor-university.com/) و [مستندات Blazor در Microsoft Learn](https://learn.microsoft.com/en-us/aspnet/core/blazor/?view=aspnetcore-10.0)
- [Microsoft Extensions AI](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai) و [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/?pivots=programming-language-csharp)

بخش‌هایی از این دوره از [CrystaCode Full-Stack AI Bootcamp](https://github.com/CrystaCode/full-stack-ai-bootcamp) با حق نشر ۲۰۲۶ متعلق به CrystaCode و تحت مجوز MIT اقتباس شده است. متن مجوز و نسخه‌ی مبنای اقتباس در [ATTRIBUTION.md](ATTRIBUTION.md) و نگاشت هر استپ به منابع آن در [course-map.md](course-map.md) آمده است.
