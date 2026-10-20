إدارة الحرمين — حزمة واجهة PWA مجانية
====================================

مهم جدًا:
هذه الحزمة واجهة تثبيت واختصار إلى رابط Google Apps Script الحالي. لا تنقل كود النظام نفسه إلى GitHub Pages، ولا تغيّر Google Sheets أو Code.gs. النظام الحالي يستخدم google.script.run، وهي ميزة تعمل داخل واجهة Apps Script ولا تعمل مباشرة من صفحة GitHub Pages خارجية. لذلك لا تعتبر هذه الحزمة تحويلًا كاملًا للنظام إلى PWA مستقل؛ إنها خطوة أولى آمنة قابلة للتثبيت.

طريقة النشر المجاني باستخدام GitHub Pages:
1) افتح https://github.com وسجّل الدخول أو أنشئ حسابًا مجانيًا.
2) اضغط New repository.
3) سمِّ المستودع: alharamain-pwa
4) اجعله Public ثم اضغط Create repository.
5) من Add file اختر Upload files.
6) ارفع محتويات هذا المجلد كلها (لا ترفع ملف ZIP وحده): index.html وmanifest.webmanifest وsw.js ومجلد icons.
7) اضغط Commit changes.
8) افتح Settings ثم Pages.
9) في Build and deployment اختر Deploy from a branch، ثم branch: main والمجلد /(root)، ثم Save.
10) انتظر حتى يظهر رابط Pages في نفس صفحة Pages. افتح الرابط واختبر زر «فتح نظام الإدارة».

التثبيت:
- على Android/Chrome: افتح رابط Pages، ثم قائمة ⋮، ثم Install app أو Add to Home screen.
- على الكمبيوتر/Chrome أو Edge: افتح رابط Pages، ثم استخدم أيقونة التثبيت في شريط العنوان إن ظهرت، أو قائمة المتصفح.
- على iPhone: افتح الرابط في Safari ثم مشاركة ثم Add to Home Screen.

البيانات والأمان:
- تظل البيانات داخل Google Sheets عبر رابط Apps Script الحالي.
- يلزم الإنترنت لفتح النظام وحفظ التعديلات.
- لا تضع كلمات مرور أو مفاتيح سرية في ملفات GitHub العامة.
- لا تحذف أو تستبدل مشروع Apps Script الحالي.

لتحويل كامل حقيقي لاحقًا:
يجب إعادة تصميم طبقة الاتصال الخلفية لأن الواجهة الحالية تستدعي google.script.run. لا يكفي نسخ Index.html إلى GitHub Pages، وقد تتطلب إعادة التصميم API آمنًا وتعديلات في Code.gs قبل نقل الواجهة بالكامل.
