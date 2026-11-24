---
name: seo
description: רושם את המערכת בגוגל, ומכין את הדפים הציבוריים שלה לגוגל ולמנועי הבינה. רק הדפים הציבוריים (דף האודות, מדיניות הפרטיות, תנאי השימוש, הצהרת הנגישות, ודפי החיפוש אם נבנו) יכולים להיכנס לחיפוש, וכל המסכים הפנימיים נשארים בחוץ. כותרת ותיאור לכל דף ציבורי, robots.txt, מפת אתר ו־llms.txt, ואחר כך רישום ב־Search Console דרך Playwright, שליחת מפת האתר, בקשה להוסיף את דף האודות, וייבוא ל־Bing. ובשלב נוסף, לא חובה, דפים ציבוריים שעוזרים למצוא את העסק בחיפוש, דף לכל שירות אמיתי ודף של שאלות נפוצות, רק מהפרטים שהיא נותנת. להשתמש כשמדברים על SEO, רישום האתר בגוגל, Search Console, להופיע בגוגל, מפת אתר, מנועי בינה, ChatGPT או llms.txt, וכשנוסף דף ציבורי ("נעדכן את גוגל") או כשמבקשים שוב מגוגל ("נבקש שוב מגוגל להוסיף את דף האודות"). וגם כשמבקשים דפים לחיפוש, דף לשירות, דף לסוג אירוע או שאלות נפוצות, וכשנוסף שירות ("נבנה דפים שעוזרים לחיפוש", "נוסף שירות").
---

# המערכת בגוגל ובמנועי הבינה

אתה עושה עם המשתמשת שני דברים: מכין את הדפים הציבוריים של המערכת שלה לגוגל ולמנועי הבינה, ורושם את האתר בגוגל. ואם היא רוצה, בונה איתה גם כמה דפים שעוזרים למצוא את העסק בחיפוש (שלב ה). היא בוגרת מגמת תכנות. היא מכירה קוד, ו־Claude עושה את העבודה. זו הפעם הראשונה שהיא עושה דבר כזה.

## מה הסקיל עושה, בכנות

- **רק הדפים הציבוריים הולכים לגוגל.** דף האודות (`/about`), שהוא דף הזהות של המערכת, ואיתו מדיניות הפרטיות (`/privacy`), תנאי השימוש (`/terms`) והצהרת הנגישות (`/accessibility`), אם הם קיימים, וגם דפי החיפוש של שלב ה (`/faq`, ו־`/services/<שם>` לכל שירות), אם נבנו. כל שאר המסכים הם העבודה הפנימית של העסק, והם נשארים מחוץ לחיפוש.
- **מה היא מקבלת:** אחרי שגוגל תוסיף את דף האודות, מי שמחפשת בגוגל את שם המערכת יחד עם שם העסק יכולה להגיע אליו, וגוגל ומנועי הבינה יכולים להבין מה המערכת ושל מי היא. מערכת ניהול היא לא אתר תוכן: הסקיל לא מבטיח תנועה, מקום ראשון או לקוחות. בשלבים א עד ד הוא לא כותב תוכן חדש על העסק. שלב ה, רק אם היא רוצה, בונה כמה דפים על מה שהעסק נותן, מהפרטים שהיא נותנת. גם הם לא מבטיחים תנועה.
- **מה זה לא:** הסימון "לא לחיפוש" (noindex) מבקש מגוגל לא להכניס מסך לחיפוש. הוא לא נועל את המסך. מה שנועל הוא הכניסה עם גוגל וכללי הגישה במסד.
- **כמה זמן:** גוגל סורקת דפים חדשים בדרך כלל בתוך כמה ימים עד כמה שבועות, ובקשה להוספה לא מבטיחה הוספה. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl ו־https://support.google.com/webmasters/answer/9012289)

ארבעה שלבים:
1. **שלב א, האתר קריא:** כותרת ותיאור לכל דף ציבורי, קובץ מוכן מראש לכל אחד, robots.txt, מפת אתר, llms.txt, וסימון "לא לחיפוש" על כל המסכים הפנימיים.
2. **שלב ב, רישום בגוגל:** Search Console, קובץ אימות, מפת האתר, ובקשה להוסיף את דף האודות.
3. **שלב ג, מנועי הבינה ו־Bing:** ייבוא מ־Search Console ל־Bing, והודעה ב־IndexNow.
4. **שלב ד, בדיקה:** מה Claude בודק באינטרנט, ומה רואים ב־Search Console עכשיו ובעוד שבוע.

ואחריהם, לא חובה, בשיעור או בבית: **שלב ה, דפים שעוזרים לחיפוש.** דף לכל שירות אמיתי ודף של שאלות נפוצות, מהפרטים שהיא נותנת, ואיתם הכלל של "לא לחיפוש", מפת האתר, llms.txt, Search Console ו־IndexNow. חוזרים אליו בכל פעם שנוסף שירות. בהתחלה לא מציגים לה אותו: הוא מגיע ב"בסוף", ב"מה הלאה".

אומרים לה בהתחלה: "ארבעה שלבים. אפשר לעצור אחרי כל אחד, ולהמשיך בפעם אחרת."

## איך מדברים איתה

- עברית פשוטה, בלשון נקבה, חם וענייני. משפטים קצרים.
- **שאלה אחת בכל פעם.** שואלים, ומחכים לתשובה.
- מה שכבר כתוב באחד הקבצים לא שואלים מחדש: אומרים מה מצאת, ושואלים "נכון?". זו השאלה היחידה באותה הודעה, בסופה.
- בלי מונחים טכניים. כל מונח מקבל משפט אחד, מתוך "משפט לכל מונח", כדי שכל התלמידות ישמעו אותו הסבר.
- **Claude עושה את העבודה:** הקבצים, הקוד, השמירה, הבדיקות, ורוב הלחיצות בדפדפן. היא מתחברת לחשבון שלה, נותנת הרשאה כשמבקשים ממנה, ובודקת בעיניים. לא נותנים לה פקודות להריץ, ולא קוד להדביק.
- **לפני כל שלב:** אומרים בשלוש שורות מה עומד לקרות, ומחכים לאישור. הכול בהודעה אחת: יש לשלב שאלה? היא בסוף אותה הודעה, וכך התשובה שלה היא גם האישור. ואומרים: "Claude Code ישאל אותך כמה פעמים אם להריץ פקודה או ללחוץ בדפדפן. אלה הפעולות של השלב שאישרת, ואפשר לאשר. מופיע משהו שלא דיברנו עליו? שאלי אותי קודם."
- **מי לוחץ:** בכל צעד כתוב מי עושה אותו: **Claude** או **את**.
  - לפני ש־Claude עובד בחלון של Playwright, אומרים לה: "עכשיו אני עובד בחלון הדפדפן. אל תלחצי בו עד שאכתוב שזה תורך. שימי אותו ליד VS Code, כדי לראות גם את החלון וגם את השיחה."
  - כשתורה: רשימה ממוספרת בלשון נקבה יחידה (לחצי, בחרי, כתבי). כל כפתור כתוב בדיוק כמו במסך, וכפתור באנגלית נשאר באנגלית. בסוף אומרים לה מה לכתוב כשהיא מסיימת ("התחברתי", "אישרתי", "סיימתי"), ולא נוגעים בדפדפן עד שהיא כותבת.
- **מצב או הודעה במסך:** אומרים לה אותם כמו שהם כתובים במסך, ואחר כך משפט אחד: מה זה אומר, והאם זה תקין.
- **מסכים של גוגל ושל Bing:** המסלול נבדק בהרצה מלאה על אתר הדמו של הקורס, בחשבון הגוגל של הדמו (19.11.2026). Search Console ומסכי הכניסה וההסכמה של גוגל היו בעברית, ו־Bing Webmaster Tools באנגלית. לכן בשלב ב השמות בסקיל כתובים כמו במסך בעברית, ובסוגריים השם באנגלית, מהמסמכים של גוגל. בשלב ג השמות של Bing באנגלית, והמסכים של גוגל בתוכו בעברית. בשלב ב, שם שכתוב בסקיל רק באנגלית לא נראה בהרצה, חוץ מ־Sitemaps, שנשאר באנגלית גם במסך בעברית. מסך בשפה אחרת, או כפתור שלא כתוב בסקיל: מוצאים אותו לפי המשמעות, ואומרים לה את שמו כמו שהוא מופיע. שם בעברית לא מנחשים: מצלמים את המסך, ומעתיקים ממנו.
- **"נעצור כאן, ורות תבדוק":** בשיעור, אומרים לרות. בבית, **Claude** כותב לה הודעה קצרה לשלוח לרות במייל: באיזה צעד עצרנו, ומה ראינו במסך. בלי שום ערך של מפתח, ובלי קוד.
- **לא ממציאים פרטים:** כל טקסט שיוצא לגוגל או למנועי הבינה לקוח מהדפים שלה ומהקבצים שלה, ובשלב ה גם מהתשובות שלה. לא מוסיפים תיאור, פרטי קשר, שירות, מחיר או אזור שלא כתובים שם ושהיא לא אמרה. פרט שלא ידוע לא מוחלף בהערכה או בטקסט לדוגמה.
- בלי אימוג'ים, ובלי המילים "קטן" ו"קטנה", בשום הקשר. בדוגמאות רק מייל או טופס.
- Playwright הוא קונקטור: כלי שנותן ל־Claude דפדפן. לא "מחבר".
- **אין כאן סודות.** קובץ האימות של גוגל ומפתח IndexNow הם לא סוד: הם יושבים באתר, וכל אחד יכול לקרוא אותם. מותר לראות אותם במסך ולשמור אותם בגרסה. בכל זאת לא פותחים את `.env`, ולא מכניסים אותו לגרסה.

### משפט לכל מונח

| מונח | ההסבר שאומרים לה |
|---|---|
| SEO | כל מה שעוזר לגוגל ולמנועי הבינה למצוא את הדפים הציבוריים שלך, ולהבין אותם |
| מנועי הבינה | כלים כמו ChatGPT, Claude ו־Gemini, שעונים על שאלות, ולפעמים קוראים אתרים כדי לענות |
| סורק | התוכנה של גוגל, של Bing או של מנוע בינה, שעוברת בין דפים באינטרנט וקוראת אותם |
| בנייה מראש (prerender) | בכל בנייה, המערכת שומרת לכל דף ציבורי קובץ מוכן עם הטקסט שלו, כדי שגם סורק שלא מריץ קוד יקרא אותו |
| האינדקס של גוגל | הרשימה של גוגל. רק דף שנמצא בה יכול להופיע בחיפוש |
| Search Console | הכלי החינמי של גוגל שבו רושמים אתר, מראים שהוא שלך, ורואים מה גוגל יודעת עליו |
| נכס | האתר שלך, כמו שהוא רשום ב־Search Console: הכתובת המלאה שלו |
| קובץ האימות | קובץ שגוגל נותנת, ששמים באתר כדי להראות שהאתר שלך. הוא לא סוד, והוא נשאר באתר תמיד |
| מפת האתר | רשימת הדפים שאת רוצה בגוגל, עם התאריך שבו כל אחד השתנה |
| robots.txt | שלט בכניסה לאתר, שאומר לסורקים של גוגל ושל מנועי הבינה שמותר להם להיכנס |
| "לא לחיפוש" (noindex) | בקשה לגוגל לא להכניס מסך לחיפוש. היא לא נועלת את המסך |
| llms.txt | קובץ טקסט בשביל מנועי הבינה, עם עיקר הדפים הציבוריים: מה המערכת, של מי, ואיך יוצרים קשר, ואם נבנו דפים בשלב ה, גם השירותים והשאלות הנפוצות. חלק מהכלים קוראים אותו |
| נתונים מובנים | פרטי העסק בצורה מסודרת שגוגל קוראת. הם כבר בדף האודות, מהסקיל about-page, ובדפים של שלב ה, אם נבנו |
| Bing | מנוע החיפוש של מיקרוסופט. לפי Bing, הוא עומד מאחורי חיפושים ותשובות של כלים אחרים, כמו ChatGPT |
| Bing Webmaster Tools | הכלי של Bing לבעלות אתרים, כמו Search Console של גוגל |
| IndexNow | הודעה ל־Bing ולמנועים נוספים: הדפים האלה חדשים, או השתנו. גוגל לא ברשימה שלו |
| מה מי שמחפשת רוצה | מה היא רוצה לעשות כשהיא כותבת חיפוש: ללמוד, למצוא עסק מסוים בשמו, להשוות ולבחור, או לפנות ולהזמין |
| קישור פנימי | קישור מדף אחד באתר לדף אחר באותו אתר. כך גוגל, מנועי הבינה ומי שקוראת מגיעות לדפים החדשים |
| דף שאלות נפוצות | דף עם שאלות אמיתיות שלקוחות שואלות, ותשובה קצרה לכל אחת. גוגל כבר לא מציגה שאלות מתחת לתוצאה, אבל הדף עצמו יכול להופיע בחיפוש |

## ענפים

עובדים לפי צורת העבודה בענפים בסקיל המערכת שלנו (`build-my-system`). לכל שינוי בקבצים ענף משלו, ו־Pull Request משלו:

1. **לפני השינוי הראשון בקבצים:** בודקים שאין שינויים שלא נשמרו, עוברים ל־`main`, מושכים מ־GitHub, ופותחים ענף: `feature/seo` בשלב א, `feature/google-verification` לקובץ האימות בשלב ב, `fix/seo` לתיקון אחרי בדיקה באינטרנט, ו־`feature/seo-changelog` ל־CHANGELOG ב"בסוף". כבר בענף של אותה עבודה? ממשיכים בו. אומרים לה במשפט באיזה ענף אנחנו, ולמה.
2. **שומרים גרסה בענף**, ודוחפים אותו ל־GitHub.
3. **Pull Request:** נותנים לה קישור ל־Pull Request, עם כותרת ותיאור בעברית: מה השתנה, ואיך בדקנו. היא ממזגת ב־GitHub, וכותבת "מיזגתי". לא ממזגים בשבילה.
4. **אחרי "מיזגתי":** חוזרים לענף הראשי (`main`, או `master` אם כך הוא נקרא), מושכים, ומוחקים את הענף, במחשב וב־GitHub.

Vercel מעלה לייצור רק את `main`. לכן כל בדיקה באינטרנט, וגם הלחיצה על **אמת** בשלב ב, באות אחרי "מיזגתי".

## לפני שמתחילים

1. **קוראים מה כבר ידוע:**
   - `תכנון המערכת.md`: שם המערכת, מה היא עושה, ולמי.
   - סקיל המותג, אם יש: שם העסק.
   - סקיל המערכת (`build-my-system`), אם יש: הכתובת של המערכת, וכללי המסכים.
   - `CLAUDE.md`, אם יש.
   - **דף האודות:** הקובץ של הדף (בדרך כלל `app/src/pages/AboutPage.tsx`), התגיות ב־`app/index.html` (`title`, `description`, תגיות ה־`og:`, ותגית `robots` או `googlebot` אם יש), ובלוק הנתונים המובנים בדף.
   - הדפים המשפטיים והצהרת הנגישות, אם יש: תאריך העדכון בכל דף.
   - קובץ הנתב, או המקום בקוד שבוחר דף לפי הכתובת (בדרך כלל `app/src/App.tsx`): אילו כתובות ציבוריות, ואילו מסכים פנימיים. ואם כבר יש `app/src/public-pages.tsx` (שלב א, צעד 2), גם הכתובות שבו: משם הנתב מקבל את הדפים הציבוריים.
   - התיקייה `app/public`, והקובץ `app/vercel.json`: יש בו כבר כלל עם `X-Robots-Tag`?
   - התיקייה `.github/workflows`: יש בה `backup.yml`? אז הגיבוי לדרייב כבר הוקם, והאפליקציה בגוגל כבר פתוחה, בחשבון גוגל מסוים (שלב ב).
   - **מה נכנס לטיוטה:** תגית `canonical` ב־`app/index.html`, תגית `robots` או `googlebot` עם noindex ב־`app/index.html`, או כלל ישן ב־`vercel.json` שנותן `X-Robots-Tag` גם לדף ציבורי. כל אחד מהם מקבל שורה בטיוטה (שלב א, צעד 1). (גוגל: דף שרוצים בחיפוש, בלי noindex בקוד המקורי שלו. נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics)
2. **הכתובת של המערכת באינטרנט:** הכתובת הקבועה והקצרה ב־Vercel, למשל `https://<שם>.vercel.app`, מסקיל המערכת, מדף האודות או מהריפו. לא מצאת? שואלים: "באיזו כתובת המערכת נפתחת באינטרנט? אפשר להעתיק אותה משורת הכתובת בדפדפן."
   - לא כתובת ארוכה של Vercel, עם שם הצוות או עם רצף אותיות: הן נעולות מאחורי כניסה.
   - **המערכת עוד לא באינטרנט:** עוצרים. אומרים לה במשפט שאת האתר רושמים בגוגל רק כשהוא באינטרנט. ונותנים לה בקשה לפעם הבאה: «כשהמערכת באינטרנט, כתבי לי: "נרשום את האתר בגוגל".»
   - **בתגיות של דף האודות או בנתונים המובנים כתובה כתובת אחרת,** `localhost` או כתובת מנוחשת: את זה מתקן הסקיל about-page. אומרים לה במשפט מה מצאת, ומציעים לתקן עכשיו, איתו. ממשיכים אחרי התיקון.
3. **אילו דפים ציבוריים יש:**
   - קודם בקוד: כתובת ציבורית היא כתובת ברמה העליונה של הנתב, לפני כל בדיקת כניסה ומחוץ למסגרת של המסכים הפנימיים, כמו שהסקילים about-page ו־legal-pages בונים, או כתובת ב־`PUBLIC_PAGES`, שב־`app/src/public-pages.tsx`.
   - אחר כך באינטרנט, ב־Playwright, בחלון שלא מחובר למערכת: כל דף ציבורי נפתח עם הטקסט שלו, ולא מסך כניסה.
   - **תשובה 200 לא מוכיחה שדף קיים.** במערכת של הקורס, הכלל ב־`vercel.json` מפנה כל כתובת לאפליקציה, ולכן גם כתובת שאין בה כלום מחזירה 200. (נבדק ב־19.11.2026 באתר הדמו של הקורס, בקריאה בלבד: `/nonexistent-xyz`, וגם `/robots.txt` כשעוד אין קובץ כזה, החזירו 200 עם דף האפליקציה.) ההוכחה היא הטקסט של הדף.
   - **404 על דף שקיים בקוד:** זה לא דף חסר, ולא מפעילים שוב את הסקיל שבנה אותו. בודקים לפי הסדר, כמו בסקיל backup-and-keep-alive: יש `vercel.json` עם `rewrites` בתיקייה ש־Vercel בונה ממנה (בדרך כלל `app`)? הגרסה החדשה עלתה? הבנייה ב־Vercel נכשלה? מתקנים אחרי שהיא מאשרת, בענף `fix/seo`, מעלים לפי "ענפים", ואחרי "מיזגתי" בודקים שוב.
   - **אין דף אודות:** עוצרים. הוא הדף שגוגל ומנועי הבינה מכירים בו את המערכת. מציעים לבנות אותו עכשיו, עם הסקיל about-page, ומחכים לתשובה.
   - **אין מדיניות פרטיות, תנאי שימוש או הצהרת נגישות:** ממשיכים עם מה שיש. בסוף מזכירים את הסקיל legal-pages או accessibility, ואומרים לה: «כשהדף מוכן, כתבי לי: "נעדכן את גוגל".»
   - הסקיל לא מותקן אצלה? מתקינים אותו רק מהמאגר `https://github.com/ruthprissman/ai-dev-course`, עם כל הקבצים שבתיקייה שלו. לא נמצא שם? אומרים לה, ולא כותבים אותו מהזיכרון.
4. **הכתובות בלי `#`:** הכתובות של הדפים נראות כמו `/about`, ולא `/#/about`. גוגל קוראת כתובות רגילות. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics) במערכות של הקורס זה כבר כך. לא כך? עוצרים, ואומרים לה שרות תבדוק את זה איתה.
5. **חוזרות באמצע, ובכל הרצה:** שיחה חדשה לא זוכרת מה נעשה. בודקים מה כבר קיים, ואומרים לה במשפט איפה עצרנו:
   - **ענף ו־Pull Request:** בודקים באיזה ענף אנחנו, ואם נשאר ענף של הסקיל הזה (השמות ב"ענפים"). יש? בודקים את ה־Pull Request שלו: `gh pr list --state all --head <הענף>`. אין Pull Request? ממשיכים לפי "ענפים", צעדים 2 ו־3. פתוח, והיא עוד לא מיזגה? נותנים לה שוב את הקישור, ומחכים ל"מיזגתי". מוזג? ממשיכים לפי "ענפים", צעד 4.
   - ב־`app/public`: `robots.txt`, `sitemap.xml`, `llms.txt`, קובץ מפתח של IndexNow, וקובץ אימות של גוגל (`google….html`).
   - ב־`app/vercel.json`: הכלל של "לא לחיפוש" (`X-Robots-Tag`).
   - הבנייה מראש: `app/src/public-pages.tsx`, `app/src/PublicPageMeta.tsx`, `app/src/entry-server.tsx`, `app/scripts/prerender.mjs`, והפקודה `build` ב־`app/package.json` (שלב א, צעד 2). אין? בונים אותה בשלב א, צעד 2, גם כששאר שלב א כבר נעשה, בענף `feature/seo`.
   - **הרשימה מול הנתב:** משווים את `PUBLIC_PAGES` (`app/src/public-pages.tsx`), את הרשימה שבכלל של "לא לחיפוש" ואת הכתובות ב־`sitemap.xml` לכתובות הציבוריות שבנתב היום. גם הדפים של שלב ה, מהקובץ `app/src/content/search-pages.ts`, הם כתובות ציבוריות, ובודקים אותם באותה צורה (שלב ה, צעד 5, סעיף 1). נוסף דף ציבורי אחרי הריצה הקודמת, למשל מדיניות פרטיות מהסקיל legal-pages? הסקילים האלה מוסיפים `<Route>` ישר לנתב, ולכן הדף לא נבנה מראש. אומרים לה במשפט, ואחרי שהיא מאשרת: מעבירים אותו מהנתב ל־`PUBLIC_PAGES`, עם כותרת ותיאור משלו (צעד 2), מוסיפים אותו לרשימה שבכלל ולמפת האתר, עם התאריך שלו (שלב א, צעדים 5 ו־8), בענף `feature/seo`, מעלים לפי "ענפים", ואחרי "מיזגתי" בודקים באינטרנט (צעד 10), ושולחים את הכתובת ל־IndexNow (שלב ג, צעד 2).
   - ב־Search Console, אחרי שהיא מחוברת: הנכס כבר קיים? מאומת? מפת האתר נשלחה?
   - **דף האודות, בכל הרצה חוזרת:** **Claude** בודק את `https://<הדומיין>/about` בבדיקת הדף של Search Console (שלב ב, צעד 6). כתוב בפרטים "כתובת האתר לא ידועה ל-Google"? מבקשים פעם אחת. המצב הזה לא מבדיל בין בקשה שגוגל לא קיבלה, למשל בגלל המכסה היומית, לבין בקשה שהתקבלה, וגוגל עוד לא סרקה את הדף. לכן לא אומרים לה שהבקשה הקודמת לא התקבלה. כתוב שם משהו אחר? גוגל כבר מכירה את הדף, ולא מבקשים שוב. הבקשה הזו קיבלה "חרגת מהמכסה"? אומרים לה רק את ההודעה, כמו בשלב ב, צעד 6, סעיף 4, ואחריה «מחר כתבי לי: "נבקש שוב מגוגל להוסיף את דף האודות".», בלי לומר משהו על הבקשה הקודמת. כך גם כשהיא כותבת "נבקש שוב מגוגל להוסיף את דף האודות". (בקשה חוזרת ביום שאחרי, ומה כתוב בבדיקה אחרי בקשה שהתקבלה: לא נבדק עדיין בהרצה.)
   - ב־Bing Webmaster Tools: האתר כבר ברשימה?
   - מה שקיים ונכון, לא בונים שוב. ממשיכים מהצעד הבא.
6. **Playwright מחובר?** בלעדיו אי אפשר לעבוד בשבילה ב־Search Console. לא מחובר: אומרים לה במשפט מה הוא, ושהיא יכולה לבקש: "תתקין לי MCP של Playwright ותפתח דפדפן". אחרי ההתקנה: "פתחי שיחה חדשה, וכתבי: נמשיך את הרישום בגוגל." Playwright נטען רק בשיחה חדשה.
7. **אין עדיין כניסה במערכת?** אומרים לה פעם אחת: "המסכים הפנימיים יסומנו 'לא לחיפוש', אבל זה לא נועל אותם. מה שנועל אותם הוא הכניסה עם גוגל." (גוגל: כדי להוציא דף מהחיפוש, noindex. כדי לנעול אותו, הגנה בסיסמה. נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/robots/intro)
8. **אומרים בשלוש שורות מה הולך לקרות,** ומחכים לאישור. ההודעה הזו היא גם הפתיחה של שלב א: אחרי האישור ממשיכים ישר לטיוטה.
   - "קודם אכין את הדפים הציבוריים לגוגל: כותרת ותיאור לכל דף, קובץ מוכן מראש לכל דף, בשביל סורקים שלא מריצים קוד, מפת אתר וקובץ למנועי הבינה, וסימון 'לא לחיפוש' על המסכים הפנימיים. אראה לך את הטקסטים לפני שהם עולים."
   - "אחר כך נרשום את האתר ב־Search Console, בחשבון הגוגל שלך. את מתחברת ומאשרת כשצריך, ואני עושה את השאר בדפדפן."
   - "בסוף נוסיף את Bing, ואבדוק שהכול עובד באינטרנט."

## שלב א: האתר קריא לגוגל ולמנועי הבינה

מה אומרים לה, כשממשיכים לשלב הזה בשיחה חדשה (בהתחלה, ההודעה של "לפני שמתחילים", סעיף 8, היא הפתיחה): "בשלב הזה אני מכין את הדפים הציבוריים לגוגל ולמנועי הבינה, ומסמן את המסכים הפנימיים 'לא לחיפוש'. ממך צריך רק אישור לטקסטים."

**הדפים הציבוריים בנויים מראש.** בלי בנייה מראש, הדפים של המערכת נכתבים בדפדפן, רק אחרי שהקוד רץ. גוגל מריצה את הקוד וקוראת את הדף כמו שהוא נראה, אבל לא כל הסורקים מריצים קוד. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics) סורק שלא מריץ קוד רואה בכתובת כזו רק את מה שב־`app/index.html`, בלי הטקסט של הדף. (לפי ai-seo: תוכן שמופיע רק אחרי שהקוד רץ, סוכנים עלולים לראות כדף ריק.) לכן בצעד 2 כל דף ציבורי מקבל קובץ מוכן מראש, עם הטקסט שלו, השם, התיאור והנתונים המובנים, וגם סורק שלא מריץ קוד קורא אותו. המסכים הפנימיים לא נבנים מראש. `llms.txt` מרכז את עיקר הטקסט של הדפים הציבוריים בשביל סורק שקורא אותו. הוא לא מחליף את הדפים. (llms.txt הוא הצעה, לא תקן, ואף מנוע לא כתוב שם כמי שקורא אותו לבד: נבדק ב־https://llmstxt.org, 19.11.2026. לפי ai-seo, מנועי בינה שאינם גוגל קוראים אותו כשהוא קיים. וגוגל כותבת שהחיפוש שלה מתעלם ממנו: נבדק במסמך הרשמי, 24.11.2026, https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)

### צעד 1: טיוטה של הטקסטים

**Claude** מכין, ומראה לה בהודעה אחת:

1. **כותרת ותיאור לכל דף ציבורי**, בטבלה: הדף, השם בלשונית ושגוגל עשויה להציג, והתיאור שגוגל עשויה להציג.
   - `/about`: השם והתיאור שכבר ב־`app/index.html`, מהסקיל about-page. לא משנים אותם.
   - כל דף ציבורי אחר: הכותרת `<שם הדף> | <שם המערכת>`, למשל "מדיניות פרטיות | <שם המערכת>". התיאור: משפט אחד, מתוך מה שכתוב בדף עצמו.
   - לכל דף כותרת משלו ותיאור משלו. (גוגל: כותרת ותיאור שונים לכל דף, ושם האתר בתחילת הכותרת או בסופה. נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/appearance/title-link ו־https://developers.google.com/search/docs/appearance/snippet)
2. **מה ייכתב ב־`llms.txt`**, במשפטים רגילים, בלי הסימנים של הקובץ: שם המערכת, משפט הסיכום, השורה על העסק, והמייל. ובמשפט: "זה הטקסט של דף האודות שלך, בקובץ בשביל מנועי הבינה." (הקובץ עצמו: צעד 6.)
3. **מה עוד ישתנה**, רק אם נמצא ב"לפני שמתחילים" (סעיף 1). שורה פשוטה לכל דבר:
   - `canonical`: "יש בקוד שורה שאומרת לגוגל שכל הדפים הם דף אחד. אוריד אותה, כדי שגוגל תכיר כל דף בנפרד."
   - תגית `robots` או `googlebot` עם noindex: "יש בקוד שורה שמבקשת מגוגל לא להכניס שום דף לחיפוש, גם לא את דף האודות. אוריד אותה, ואת המסכים הפנימיים אסמן 'לא לחיפוש' בדרך אחרת."
   - כלל ישן ב־`vercel.json` שמסמן גם דף ציבורי: "יש הגדרה שמסמנת גם את <הדף> 'לא לחיפוש'. אתקן אותה, כך שרק המסכים הפנימיים יסומנו."
4. משפט אחד: "הטקסטים האלה לקוחים מהדפים שלך. לא נוסף שום פרט חדש על העסק."

ומחכים לאישור. האישור הזה הוא גם האישור לשינויים שבסעיף 3. תיקנה משהו? מראים שוב את מה שהשתנה, ומחכים. רק אחרי האישור בונים.

### צעד 2: כל דף ציבורי: כותרת, תיאור, וקובץ מוכן מראש

**מה זה, ולמה.** הדפים של המערכת נכתבים בדפדפן, רק אחרי שהקוד רץ. גוגל מריצה את הקוד, אבל לא כל הסורקים מריצים קוד, וסורק כזה רואה בכל כתובת רק את `app/index.html`, בלי הטקסט של הדף. בנייה מראש (prerender) פותרת את זה: בכל בנייה של המערכת נשמר לכל דף ציבורי קובץ HTML מוכן, עם הטקסט של הדף, השם שלו בלשונית, התיאור שלו והנתונים המובנים שבו. כל דפדפן וכל סורק שמבקשים את הכתובת מקבלים קודם את הקובץ הזה, ואחר כך הקוד נטען, והדף ממשיך לעבוד כרגיל. המסכים הפנימיים לא נבנים מראש, וממשיכים לקבל את `app/index.html`, כמו היום. (גוגל: "server-side or pre-rendering is still a great idea", כי "not all bots can run JavaScript". נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics. כך גם באתר של רות, ב־`scripts/prerender.mjs`.)

אומרים לה, במשפט מ"משפט לכל מונח": "בנייה מראש: בכל בנייה, המערכת שומרת לכל דף ציבורי קובץ מוכן עם הטקסט שלו, כדי שגם סורק שלא מריץ קוד יקרא אותו." לא מראים לה קוד, ולא שואלים אותה על זה: היא אישרה את השלב.

**בלי ספרייה חדשה.** הכול נבנה ממה שכבר בפרויקט: הבנייה לשרת של Vite (`vite build --ssr`), `prerenderToNodeStream` של `react-dom/static`, ו־`StaticRouter` של `react-router-dom`. (נבדק במסמכים הרשמיים, 24.11.2026: https://vite.dev/guide/ssr, בחלקים "Building for Production" ו־"Pre-Rendering / SSG". https://react.dev/reference/react-dom/static/prerenderToNodeStream: מחכה שכל הדף ייטען, כולל Suspense ו־`lazy`, ולכן לא `renderToString`. https://reactrouter.com/api/declarative-routers/StaticRouter: נתב שעומד בכתובת אחת, בשביל השרת. הדף מפנה למסמך של גרסה 8, ולכן גם הורץ: עם react-router-dom 7.18.5, 24.11.2026.)

#### 1. רשימה אחת של הדפים הציבוריים: `app/src/public-pages.tsx`

מהרשימה הזו נבנים שלושה דברים: הכתובות בנתב, השם בלשונית והתיאור, והקבצים המוכנים. כל דף ציבורי שנמצא ב"לפני שמתחילים" (סעיף 3) נכנס אליה, עם השם והתיאור שהיא אישרה בטיוטה (צעד 1).

```tsx
import type { ReactNode } from 'react'
import { AboutPage } from './pages/AboutPage.tsx'
import { PrivacyPage } from './pages/PrivacyPage.tsx'
import { TermsPage } from './pages/TermsPage.tsx'

// הדפים הציבוריים (הסקיל seo). מהרשימה הזו נבנים הכתובות בנתב, השם בלשונית והתיאור לגוגל,
// וגם קובץ HTML מוכן לכל דף, בזמן הבנייה (scripts/prerender.mjs).
// דף ציבורי חדש נכנס לכאן, ולא ישר לנתב. מסך פנימי לא נכנס לכאן אף פעם.
// הדפים עצמם לא מייבאים מהקובץ הזה.

// הכתובת הקצרה של המערכת בייצור, בלי / בסוף.
export const SITE_URL = 'https://<הדומיין>'

// השם והתיאור שב־app/index.html, מילה במילה (מהסקיל about-page). הם גם של כל מסך פנימי.
// הבנייה עוצרת אם הם שונים מ־app/index.html.
export const SITE_META = {
  title: '<ה־title שב־app/index.html>',
  description: '<ה־description שב־app/index.html>',
}

export type PublicPage = {
  path: string // הכתובת, כמו במפת האתר: אותיות a עד z, ספרות ומקפים, בלי / בסוף
  title: string // השם בלשונית
  description: string // התיאור לגוגל: משפט אחד, מתוך הדף
  element: ReactNode // הדף עצמו
}

export const PUBLIC_PAGES: PublicPage[] = [
  { path: '/about', ...SITE_META, element: <AboutPage /> },
  {
    path: '/privacy',
    title: 'מדיניות פרטיות | <שם המערכת>',
    description: '<משפט אחד, מתוך הדף>',
    element: <PrivacyPage />,
  },
  {
    path: '/terms',
    title: 'תנאי שימוש | <שם המערכת>',
    description: '<משפט אחד, מתוך הדף>',
    element: <TermsPage />,
  },
]

// הדף הציבורי של הכתובת, או undefined במסך פנימי. כמו הנתב: גם באותיות גדולות, וגם עם / בסוף.
export function findPublicPage(pathname: string): PublicPage | undefined {
  const path = pathname.toLowerCase().replace(/\/+$/, '') || '/'
  return PUBLIC_PAGES.find((page) => page.path === path)
}
```

- **רק הדפים שקיימים אצלה,** בשמות ובמקומות של הקבצים כמו אצלה. הצהרת הנגישות נכנסת באותה צורה (`/accessibility`).
- **`SITE_URL`:** הכתובת הקצרה, בדיוק כמו בתגית `og:url` שב־`app/index.html` (בלי `/about` שבסופה). הבנייה עוצרת אם הן שונות.
- **`SITE_META`:** ה־`<title>` וה־`description` שב־`app/index.html`, מילה במילה. **Claude** מעתיק אותם משם, ולא מנסח. הם של `/about`, כמו בטיוטה (צעד 1), וגם של כל מסך פנימי. הבנייה עוצרת אם הם שונים.
- **`path`:** בדיוק כמו במפת האתר (צעד 5) וברשימה שבכלל (צעד 8). בלי אותיות גדולות, בלי נקודה, ובלי `/` בסוף.
- **הדפים לא מייבאים מהקובץ הזה.** הוא מייבא אותם, ולכן ייבוא בכיוון ההפוך יוצר מעגל. דף שצריך את הכתובת, כמו בנתונים המובנים, כותב אותה אצלו, כמו `SITE_URL` שבדף האודות.

#### 2. הנתב קורא מהרשימה: `app/src/App.tsx`

```tsx
import { PUBLIC_PAGES } from './public-pages.tsx'
import { PublicPageMeta } from './PublicPageMeta.tsx'

// ...
      <BrowserRouter>
        <PublicPageMeta />
        <Routes>
          {PUBLIC_PAGES.map((page) => (
            <Route key={page.path} path={page.path} element={page.element} />
          ))}

          {/* המסכים הפנימיים, כמו קודם */}
        </Routes>
      </BrowserRouter>
```

- **ה־`<Route>` של כל דף ציבורי יוצא מהנתב,** יחד עם ה־`import` של הדף, ובמקומם השורות של הרשימה. באותו מקום שבו הם היו: ברמה העליונה, לפני כל בדיקת כניסה, ומחוץ למסגרת של המסכים הפנימיים, כמו בסקילים about-page ו־legal-pages.
- **`<PublicPageMeta />`** בתוך `BrowserRouter`, לפני `<Routes>` (סעיף 3).
- **`app/src/main.tsx` לא משתנה.** `createRoot` נשאר (סעיף 4.6).
- **אין נתב** (כמו במערכת הדמו של הקורס): ברכיב העליון, לפני בדיקת הכניסה, `const publicPage = findPublicPage(window.location.pathname)`, ואם יש דף: `return publicPage.element`. במקום הבדיקה הישנה של `/about`, `/privacy` ו־`/terms`. בלי `PublicPageMeta`: בלי נתב, כל מעבר לכתובת טוען את הדף מחדש, והקובץ המוכן כבר מביא את השם והתיאור של הדף. המסכים הפנימיים מקבלים את אלה של `app/index.html`. לכן במחשב, ב־`npm run dev`, דף ציבורי מראה בלשונית את השם של `app/index.html`. את השם של הדף בודקים ב־`vite preview`, בכתובת עם `/` בסוף (סעיף 6.4). ובסעיף 4.1, הגרסה בלי נתב.

#### 3. השם בלשונית והתיאור: `app/src/PublicPageMeta.tsx`

הקובץ המוכן של כל דף כבר מביא את השם והתיאור שלו (סעיף 4). הרכיב הזה מעדכן אותם כשעוברים בין מסכים בלי לטעון את הדף מחדש: בדף ציבורי, השם והתיאור שלו מהרשימה. בכל מסך אחר, אלה של `app/index.html`.

```tsx
import { useEffect } from 'react'
import { useLocation } from 'react-router-dom'
import { findPublicPage, SITE_META } from './public-pages.tsx'

// השם בלשונית והתיאור לגוגל, בכל מעבר בין מסכים: של הדף הציבורי שפתוח, מ־public-pages.tsx,
// ובכל מסך אחר אלה של app/index.html. משנה את התגיות שכבר יש, ולא מוסיף תגית.
// את canonical לא משנים: הוא נכתב בבנייה, בקובץ של כל דף ציבורי.
export function PublicPageMeta() {
  const { pathname } = useLocation()

  useEffect(() => {
    const meta = findPublicPage(pathname) ?? SITE_META
    document.title = meta.title
    document.querySelector('meta[name="description"]')?.setAttribute('content', meta.description)
  }, [pathname])

  return null
}
```

- **השם והתיאור באים מהרשימה, ולא מהדף.** אין `usePageMeta` בכל דף, ואין עוד מקום שבו כתובים השם והתיאור. (גוגל: מותר לכתוב את הכותרת ואת התיאור מהקוד. נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics)
- **לא כותבים `<title>` או `<meta>` בתוך ה־JSX של הדף, ולא מוסיפים תגית description שנייה.** React שם `<title>` כזה ב־head, ליד זה שכבר יש, ואז בדף יש שתי כותרות. (React: כשיש יותר מ־`<title>` אחד, ההתנהגות של דפדפנים ושל מנועי חיפוש לא מוגדרת. נבדק במסמך הרשמי, 19.11.2026: https://react.dev/reference/react-dom/components/title. נבדק גם בהרצה של React 19 על דף לדוגמה, ולא באתר חי, 19.11.2026: `<title>` ו־`<meta name="description">` בתוך הדף השאירו ב־head שתי כותרות ושני תיאורים, והתיאור של דף האודות היה הראשון.)
- **שלב א כבר נעשה לפני הצעד הזה** (למשל באתר הדמו של הקורס, 19.11.2026)? בדפים הציבוריים יש קובץ עזר לכותרת ולתיאור, כמו `usePageMeta`, שמחזיר כשיוצאים מהדף את הערכים שהיו קודם. **Claude** מוריד אותו ואת הקריאות אליו, באותה גרסה. ליד הקובץ המוכן הוא טועה: הערכים שהיו קודם הם של הדף שנטען, ולא של `app/index.html`, ומסך פנימי שעוברים אליו היה מקבל את השם של הדף הציבורי.
- **יש בפרויקט ספרייה שמנהלת את ה־head** (כמו react-helmet)? עובדים דרכה, עם הערכים מהרשימה, ובודקים גם איתה שלא נשארו לידה התגיות של `app/index.html`: בסוף יש כותרת אחת ותיאור אחד. אין ספרייה? לא מוסיפים ספרייה חדשה, כמו בסקיל about-page.
- **ב־`app/index.html` אין שום דבר שמתאים רק לדף אחד:** לא noindex ולא `canonical`. הקובץ הזה נשלח לכל המסכים הפנימיים, ולכן תגית כזו תחול על כולם. יש שם `canonical`, או תגית `robots` או `googlebot` עם noindex? מורידים אותה אחרי שהיא אישרה את הטיוטה (צעד 1, סעיף 3). הבנייה עוצרת אם היא נשארה.
- **`canonical` רק בקבצים המוכנים, ולא משתנה במעבר בין מסכים.** גוגל לא ממליצה לשנות אותו מהקוד, ומבקשת שבדף יהיה רק אחד. סורק טוען כל כתובת מחדש, ומקבל את הקובץ של הכתובת הזו. (נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics, בחלק על `rel="canonical"`.)
- לא משנים שום טקסט שרואים בדפים, ולא שום מסך.

#### 4. הבנייה מראש

**4.1. `app/src/entry-server.tsx`:** מה שהבנייה מציירת. רק הדפים הציבוריים, בלי `App`, בלי בדיקת הכניסה, ובלי ה־Providers של המסכים הפנימיים.

```tsx
import { prerenderToNodeStream } from 'react-dom/static'
import { Route, Routes, StaticRouter } from 'react-router-dom'
import { PUBLIC_PAGES } from './public-pages.tsx'

// הבנייה מראש (הסקיל seo): רק הדפים הציבוריים, בלי שום מסך פנימי ובלי הנתונים של המערכת.
// scripts/prerender.mjs קורא לקובץ הזה בזמן הבנייה, ולא בדפדפן.
export { PUBLIC_PAGES, SITE_META, SITE_URL } from './public-pages.tsx'

export function render(path: string, onError: (error: unknown) => void) {
  return prerenderToNodeStream(
    <StaticRouter location={path}>
      <Routes>
        {PUBLIC_PAGES.map((page) => (
          <Route key={page.path} path={page.path} element={page.element} />
        ))}
      </Routes>
    </StaticRouter>,
    { onError },
  )
}
```

אין נתב? אותו קובץ, בלי `StaticRouter`:

```tsx
export function render(path: string, onError: (error: unknown) => void) {
  const page = PUBLIC_PAGES.find((p) => p.path === path)
  return prerenderToNodeStream(<>{page?.element}</>, { onError })
}
```

(אזהרה של oxlint על הקובץ הזה, "Fast refresh only works when a file only exports components", צפויה: הקובץ רץ רק בבנייה. לא מתקנים אותה.)

**4.2. `app/scripts/prerender.mjs`:** כותב את הקבצים. כמו `scripts/prerender.mjs` באתר של רות: מתבנית `dist/index.html`, ובכל דף קובץ `dist/<הכתובת>/index.html`.

```js
// הבנייה מראש של הדפים הציבוריים (הסקיל seo). רץ בסוף npm run build, אחרי שתי הבניות של Vite.
// לכל דף ב־src/public-pages.tsx נכתב קובץ dist/<הכתובת>/index.html: הקובץ dist/index.html, עם הדף עצמו
// בתוך #root, ועם השם, התיאור ו־canonical של הדף. מסך פנימי לא מקבל קובץ, וממשיך לקבל את dist/index.html.
// בלי cleanUrls ב־vercel.json: איתו הכלל ששולח כל כתובת ל־index.html מפסיק לעבוד.
// כל בעיה עוצרת את הבנייה. ב־Vercel הגרסה החדשה אז לא עולה, והגרסה הקודמת נשארת בייצור.
import { mkdir, readFile, rm, writeFile } from 'node:fs/promises'
import path from 'node:path'
import { text } from 'node:stream/consumers'
import { fileURLToPath, pathToFileURL } from 'node:url'

const root = path.resolve(path.dirname(fileURLToPath(import.meta.url)), '..')
const dist = path.join(root, 'dist')
const ssr = path.join(root, 'dist-ssr')

const ROOT_DIV = '<div id="root"></div>'
const TITLE = /<title>([\s\S]*?)<\/title>/g
const DESCRIPTION = /<meta\s[^>]*name=["']description["'][^>]*>/gi

const escapeHtml = (value) =>
  value.replace(/&/g, '&amp;').replace(/"/g, '&quot;').replace(/</g, '&lt;').replace(/>/g, '&gt;')
const unescapeHtml = (value) =>
  value.replace(/&quot;/g, '"').replace(/&#39;/g, "'").replace(/&lt;/g, '<').replace(/&gt;/g, '>').replace(/&amp;/g, '&')
const count = (html, pattern) => (html.match(pattern) ?? []).length
const contentOf = (tag) => (tag.match(/content=(?:"([^"]*)"|'([^']*)')/) ?? [])[1] ?? ''

class PrerenderError extends Error {}
const fail = (message) => {
  throw new PrerenderError(message)
}

async function main() {
  const template = await readFile(path.join(dist, 'index.html'), 'utf8')

  // הקובץ שממנו בונים: #root ריק אחד, כותרת אחת ותיאור אחד, ובלי תגית שהייתה חלה על כל הכתובות.
  if (template.split(ROOT_DIV).length !== 2) fail(`dist/index.html must contain exactly one ${ROOT_DIV}`)
  if (count(template, TITLE) !== 1) fail('dist/index.html must contain exactly one <title>')
  if (count(template, DESCRIPTION) !== 1) fail('dist/index.html must contain exactly one meta description')
  if (/rel=["']canonical["']/i.test(template)) fail('app/index.html has a canonical tag, which applies to every address: remove it')
  if (/<meta[^>]*name=["'](?:robots|googlebot)["'][^>]*noindex/i.test(template)) fail('app/index.html has a noindex meta tag: remove it')

  let server
  try {
    server = await import(pathToFileURL(path.join(ssr, 'entry-server.js')).href)
  } catch (error) {
    fail(
      'loading the public pages crashed. A file that a public page imports touches window, document or ' +
        `localStorage, or reads a missing setting, as soon as it loads:\n${error?.stack ?? error}`,
    )
  }
  const { render, PUBLIC_PAGES, SITE_META, SITE_URL } = server

  // SITE_META זהה ל־app/index.html, כי הוא חוזר בכל מסך פנימי.
  const indexTitle = unescapeHtml(template.match(/<title>([\s\S]*?)<\/title>/)[1].trim())
  const indexDescription = unescapeHtml(contentOf(template.match(DESCRIPTION)[0]))
  if (indexTitle !== SITE_META.title) fail(`SITE_META.title is not the <title> of app/index.html ("${indexTitle}")`)
  if (indexDescription !== SITE_META.description) fail('SITE_META.description is not the meta description of app/index.html')

  // SITE_URL: הכתובת הקצרה, כמו ב־og:url שכתב הסקיל about-page.
  if (!/^https:\/\/[a-z0-9.-]+$/.test(SITE_URL) || SITE_URL.includes('localhost')) {
    fail(`SITE_URL must be the short production address, with https:// and without / at the end ("${SITE_URL}")`)
  }
  const ogUrl = template.match(/<meta\s[^>]*property=["']og:url["'][^>]*>/i)
  if (ogUrl && !contentOf(ogUrl[0]).startsWith(`${SITE_URL}/`)) {
    fail(`SITE_URL (${SITE_URL}) is not the address in og:url in app/index.html (${contentOf(ogUrl[0])})`)
  }

  // לכל דף כתובת, כותרת ותיאור משלו.
  for (const key of ['path', 'title', 'description']) {
    const values = PUBLIC_PAGES.map((page) => page[key])
    const twice = values.find((value, i) => values.indexOf(value) !== i)
    if (twice) fail(`two public pages have the same ${key}: "${twice}"`)
  }

  for (const page of PUBLIC_PAGES) {
    if (!/^\/[a-z0-9-]+(?:\/[a-z0-9-]+)*$/.test(page.path)) {
      fail(`${page.path}: a public path is lowercase a-z, digits and hyphens, without / at the end`)
    }

    const errors = []
    let body
    try {
      const { prelude } = await render(page.path, (error) => {
        errors.push(error)
      })
      body = await text(prelude)
    } catch (error) {
      errors.unshift(error)
    }
    if (errors.length) fail(`${page.path} crashed while rendering:\n${errors[0]?.stack ?? errors[0]}`)
    if (!body.trim()) fail(`${page.path} rendered empty: is it in PUBLIC_PAGES with the same path?`)

    // פונקציות ולא מחרוזות, כדי ש־$ בטקסט של הדף לא ייקרא כסימן מיוחד.
    const html = template
      .replace(ROOT_DIV, () => `<div id="root">${body}</div>`)
      .replace(TITLE, () => `<title>${escapeHtml(page.title)}</title>`)
      .replace(DESCRIPTION, () => `<meta name="description" content="${escapeHtml(page.description)}" />`)
      .replace('</head>', () => `  <link rel="canonical" href="${SITE_URL}${page.path}" />\n  </head>`)

    const file = path.join(dist, ...page.path.split('/').filter(Boolean), 'index.html')
    await mkdir(path.dirname(file), { recursive: true })
    await writeFile(file, html, 'utf8')
  }

  return PUBLIC_PAGES.map((page) => page.path)
}

// יציאה מפורשת: טיימר שקובץ כלשהו הפעיל כשנטען לא יעצור את הבנייה.
main()
  .then(async (paths) => {
    await rm(ssr, { recursive: true, force: true })
    process.stdout.write(`prerendered ${paths.length} public pages: ${paths.join(', ')}\n`)
    process.exit(0)
  })
  .catch(async (error) => {
    await rm(ssr, { recursive: true, force: true })
    process.stderr.write(`\nprerender failed: ${error instanceof PrerenderError ? error.message : error?.stack ?? error}\n\n`)
    process.exit(1)
  })
```

- **הקובץ כמו שהוא.** הבדיקות שבו הן הכללים של השלב: כותרת ותיאור לכל דף, שונים זה מזה, ו־`app/index.html` בלי `canonical` ובלי noindex. לא מורידים בדיקה כדי שהבנייה תעבור.
- **מה שהוא לא כותב:** קובץ לכתובת `/`, או לכל מסך פנימי. הם ממשיכים לקבל את `dist/index.html`, עם `<div id="root"></div>` ריק.
- **`dist-ssr`** הוא הבנייה לשרת. הסקריפט מוחק אותו בסוף, גם כשהבנייה נכשלת. הוא לא עולה לייצור, ולא נשמר בגרסה.

**4.3. `app/package.json`:** בסוף הפקודה `build` נוספות שתי פקודות. מה שכבר כתוב בה נשאר בהתחלה, בלי שינוי:

```json
"build": "tsc -b && vite build && vite build --ssr src/entry-server.tsx --outDir dist-ssr --sourcemap && node --enable-source-maps scripts/prerender.mjs"
```

- `--sourcemap` ו־`--enable-source-maps`: כשדף מפיל את הבנייה, ההודעה מראה את הקובץ ואת השורה בקוד המקורי (`src/...`), ולא שורה בקובץ הבנוי (סעיף 5). המפות נשארות ב־`dist-ssr`, ונמחקות איתו. הקוד שעולה לדפדפן לא משתנה.
- Vercel מריץ את `npm run build`. בהגדרות הפרויקט ב־Vercel יש Build Command אחר? אז הבנייה מראש לא רצה שם (צעד 10 יגלה). אומרים לה במשפט, ורות תבדוק.

**4.4. `app/.gitignore`:** יש בו שורה `dist-ssr`? בתבנית של Vite היא כבר שם. אין? מוסיפים אותה.

**4.5. `app/vercel.json`: לא משתנה, ובלי `cleanUrls`.** Vercel מגיש קובץ שקיים לפני כלל ה־`rewrites` (צעד 8), ולכן `/about` מחזיר את `dist/about/index.html`, וכל כתובת אחרת ממשיכה ל־`index.html`. (Vercel: "precedence is given to the filesystem prior to rewrites being applied". נבדק במסמך הרשמי, 24.11.2026: https://vercel.com/docs/project-configuration/vercel-json. נבדק גם באתר חי, 24.11.2026, למטה.)
- **לא מוסיפים `"cleanUrls": true`.** בבדיקה באתר חי (24.11.2026), עם `cleanUrls` והקבצים בשם `dist/about.html`: הכלל ששולח כל כתובת ל־`/index.html` הפסיק לעבוד, ו־`/today`, `/nonexistent-xyz`, `/ABOUT` ו־`/services/test-xyz` החזירו 404. כל המסכים הפנימיים היו נשברים בכניסה ישירה. וגם קובץ האימות של גוגל חזר עם הפניה, 308, ל־`/google…` בלי `.html`, וגוגל כותבת: "Search Console does not follow redirects when looking for this file". (Vercel: עם `cleanUrls`, כתובת שנגמרת ב־`.html` מקבלת 308. גוגל: https://support.google.com/webmasters/answer/9008080. שני המסמכים נבדקו ב־24.11.2026. באותו מסמך של גוגל, בפתרון בעיות, כתוב גם שהפניה בתוך אותו דומיין כן נבדקת. בגלל שני הנוסחים, לא סומכים על זה.)
- לא מוסיפים `trailingSlash`. באתר של רות הוא `true`, כי שם כל הכתובות נגמרות ב־`/`. כאן `/about` היה עובר ל־`/about/`, שמסומן "לא לחיפוש" בכלל של צעד 8.

**4.6. הדפדפן: `createRoot` נשאר.** כשהקוד נטען, React מוחק את מה שבתוך `#root` בקובץ המוכן, ומצייר את אותו דף מחדש. (React: "The first time you call root.render, React will clear all the existing HTML content inside the React root". נבדק במסמך הרשמי, 24.11.2026: https://react.dev/reference/react-dom/client/createRoot.)
- באותו מסמך React כותבת שעל HTML שנבנה מראש משתמשים ב־`hydrateRoot`. כאן לא, בכוונה: `hydrateRoot` דורש שהציור הראשון בדפדפן יהיה זהה לגמרי לקובץ המוכן, וכל הבדל, כמו תאריך, ערך מהדפדפן או Provider של המערכת, נותן שגיאות. ובמסכים הפנימיים `#root` ריק. עם `createRoot` הדף פשוט מצויר מחדש. לא מחליפים ל־`hydrateRoot`. (נבדק ב־24.11.2026, במחשב ובאתר חי: בלי שום הודעה ב־console, ובקובץ המוכן היה ב־`#root` תגית שהבנייה הוסיפה, `<link rel="preload">` ללוגו, ובדף אחרי הטעינה כבר לא. כך רואים ש־React צייר מחדש.)

#### 5. דף ציבורי שמפיל את הבנייה

בבנייה מראש הדפים הציבוריים רצים ב־Node, ולא בדפדפן. אין שם `window`, `document` ו־`localStorage` של דפדפן, ואין Providers של המערכת. דף ציבורי, או קובץ שהוא מייבא, שנוגע באחד מהם, מפיל את הבנייה. ההודעה מתחילה ב־`prerender failed:`, ואחריה הקובץ והשורה. ב־Vercel הבנייה נכשלת, והגרסה הקודמת נשארת בייצור. במחשב **Claude** מריץ את הבנייה לפני כל שמירה (צעד 9), ולכן כמעט תמיד זה נתפס שם.

| מה כתוב בהודעה | מה זה | מה Claude עושה |
|---|---|---|
| `loading the public pages crashed`, ואחריו `window is not defined`, `document is not defined` או `localStorage is not defined` | קובץ שדף ציבורי מייבא נוגע בדפדפן ברגע שהוא נטען, בשורה מחוץ לפונקציה | מעביר את השורה לתוך פונקציה, שנקראת מ־`useEffect` או מלחיצה, ולא כשהקובץ נטען |
| `/<כתובת> crashed while rendering`, עם `window`, `document` או `localStorage` | הדף עצמו נוגע בדפדפן כשהוא מצויר | מעביר את זה ל־`useEffect`, או שומר עליו ב־`typeof window !== 'undefined'` |
| `/<כתובת> crashed while rendering`, עם `חייב לפעול בתוך ...` או `must be used within` | הדף משתמש ב־hook של המסכים הפנימיים, כמו התפקיד, הנתונים או הכניסה | הדף הציבורי לא משתמש בנתונים של המערכת. מה שהוא צריך עובר לקבוע בדף או לקובץ תוכן. לא עוטפים את הדף ב־Providers של המערכת בבנייה: כך נתונים פנימיים היו נכנסים לקובץ ציבורי |
| `supabaseUrl is required`, או הגדרה אחרת שחסרה | דף ציבורי מייבא, ישר או דרך רכיב, את הקובץ שמתחבר ל־Supabase, וההגדרה שלו לא קיימת בבנייה | דף ציבורי לא מייבא את הקובץ של Supabase. רכיב משותף שמייבא אותו מתפצל: החלק שהדף הציבורי צריך עובר לקובץ בלי Supabase |
| `rendered empty` | הדף לא צייר כלום, למשל כש־`element` ריק, או, בלי נתב, כשהכתובת ב־`render` לא זהה לרשימה | מתקן את הרשומה ברשימה, או את הכתובת |
| `two public pages have the same title` או `description` | שני דפים עם אותה כותרת או אותו תיאור | חוזר לטיוטה (צעד 1): לכל דף משלו, והיא מאשרת |
| `SITE_META.title`, `SITE_META.description` או `SITE_URL` | הרשימה לא תואמת ל־`app/index.html` | מעתיק שוב מ־`app/index.html`. הכתובת ב־`og:url` עצמה שגויה? את זה מתקן הסקיל about-page ("לפני שמתחילים", סעיף 2) |
| `must contain exactly one <div id="root"></div>` | ב־`app/index.html` יש משהו בתוך `#root`, כמו טקסט של טעינה | אומר לה במשפט מה נמצא, ומוציא אותו אחרי שהיא מאשרת |
| `has a canonical tag` או `has a noindex meta tag` | נשארה ב־`app/index.html` תגית שחלה על כל הכתובות | מוריד אותה (סעיף 3) |

- **`typeof window`, ולא `typeof localStorage`.** ב־Node, `localStorage` מתנהג אחרת בכל גרסה. במחשב, ב־Node 22, הוא לא קיים. בבנייה ב־Vercel, ב־Node v26.13.1, הוא נתן אזהרה ("ExperimentalWarning: localStorage is not available because --localstorage-file was not provided"), ו־`localStorage.getItem` זרק שגיאה. ולפי המסמך של Node, מגרסה 26 כבר הגישה עצמה זורקת שגיאה. `window` לא קיים בשום גרסה של Node. (נבדק ב־24.11.2026: https://nodejs.org/api/globals.html, ובבנייה ב־Vercel.)
- **נתונים שהדף טוען מהמסד** ב־`useEffect` לא נכנסים לקובץ המוכן, כי `useEffect` לא רץ בבנייה. בקובץ יהיה מה שהדף מציג לפני שהנתונים הגיעו. הטקסט של דף ציבורי כתוב בקוד או בקובץ תוכן, כמו בסקילים about-page ו־legal-pages ובשלב ה. דף ציבורי שכל הטקסט שלו מגיע מהמסד? אומרים לה במשפט, ורות תבדוק.
- **טיימר שקובץ הפעיל כשנטען** לא עוצר את הבנייה: הסקריפט יוצא בעצמו בסוף. (נבדק במחשב, 24.11.2026.)
- **איך Claude מתקן:** קורא בהודעה את הקובץ ואת השורה, ומתקן רק שם. מריץ שוב את הבנייה. אחר כך פותח ב־Playwright, במחשב, את המסך הפנימי שמשתמש באותו קובץ, ובודק שהוא עובד כמו קודם. **לא מוציאים דף מהרשימה, ולא מוציאים את הבנייה מראש מ־`build`, כדי שהבנייה תעבור.** התיקון ישנה את מה שמסך פנימי עושה? עוצרים, אומרים לה במשפט מה נמצא, ורות תבדוק.
- (נבדק במחשב, 24.11.2026, בבנייה אמיתית של המערכת: כל שורה בטבלה, חוץ מ־`supabaseUrl is required`, הופעלה בכוונה, בשינוי של שורה אחת, ובכל אחת הבנייה נעצרה עם ההודעה שבטבלה. בשלוש שורות הדף הפיל את הבנייה: גישה ל־`window.localStorage` כשהקובץ נטען, ושם ההודעה הראתה רק את הקובץ ואת השורה ב־`src`, בלי הכתובת של הדף. וגישה ל־`localStorage` בזמן הציור, ו־hook של התפקיד בלי ה־Provider שלו, ושם ההודעה הראתה גם את הכתובת של הדף. `supabaseUrl is required.` נבדק רק ב־supabase-js 2.107.0, ב־Node, מחוץ לבנייה: בלי הכתובת של Supabase, `createClient` עצר בהודעה הזו. עם כתובת הוא עבד גם ב־Node, בלי `window`, ולא השאיר את Node פתוח.)

#### 6. בודקים במחשב (בצעד 9)

1. **הבנייה:** `npm run build` עובר, ובסופו השורה `prerendered <מספר> public pages:`, עם כל הכתובות שברשימה, ורק אותן.
2. **הקבצים:** לכל דף ציבורי, **Claude** קורא את `app/dist/<הכתובת>/index.html` (ל־`/about`: `app/dist/about/index.html`), ובודק:
   - הטקסט של הדף, כולל הכותרת הראשית, בתוך `<div id="root">`.
   - בדיוק `<title>` אחד, עם השם של הדף, ובדיוק `meta[name="description"]` אחד, עם התיאור שלו.
   - בדיוק `<link rel="canonical">` אחד: `<SITE_URL><הכתובת>`.
   - בדף האודות, בלוק ה־`application/ld+json` מסוג `Organization`, עם אותו טקסט כמו בדף. בכל דף שמצייר בלוק כזה, הבלוק בקובץ.
3. **אין קובץ למסך פנימי:** ב־`app/dist` יש רק `index.html`, תיקייה לכל דף ציבורי, `assets`, והקבצים של `app/public`. וב־`app/dist/index.html`, `<div id="root"></div>` ריק.
4. **ב־Playwright, על `vite preview`:** במחשב הקובץ המוכן נפתח בכתובת עם `/` בסוף, כמו `/about/`. `/about`, בלי `/`, מחזיר במחשב את `app/index.html`, והקוד מצייר את הדף. זה צפוי: בייצור `/about` מחזיר את הקובץ (סעיף 7). בכל דף ציבורי, ב־`/<הכתובת>/`:
   - ב־console אין שגיאות ואין אזהרות.
   - ב־head בדיוק כותרת אחת, תיאור אחד ו־`canonical` אחד, של הדף הזה.
   - הדף עובד אחרי הטעינה: קישור בתוכו עובר לדף אחר בלי לטעון מחדש.
   - מעבר מדף ציבורי למסך פנימי מחזיר את השם והתיאור של `app/index.html`, וחזרה לדף הציבורי מחזירה את שלו.
5. **`npm run dev` עובד כמו קודם,** והמסכים הפנימיים נפתחים. בזמן פיתוח אין בנייה מראש, וזה בסדר.

#### 7. בודקים בייצור (בצעד 10)

אחרי "מיזגתי", בכתובת הקצרה, בלי להיות מחוברת:

1. **הקוד שחוזר, לפני שהוא רץ.** לכל דף ציבורי, **Claude** מוריד את הכתובת, בלי דפדפן (`curl -s https://<הדומיין>/<הכתובת>`), ובודק בקוד שחזר את כל מה שבסעיף 6.2: הטקסט, השם, התיאור, `canonical`, והנתונים המובנים. כך רואה את הדף סורק שלא מריץ קוד.
2. **הכותרות:** `curl -sI` לכל דף ציבורי: 200, `text/html`, בלי `X-Robots-Tag`, ובלי `Location`, כלומר בלי הפניה.
3. **מסך פנימי, `/` ו־`/nonexistent-xyz`:** 200, עם `X-Robots-Tag: noindex, nofollow`, ו־`<div id="root"></div>` ריק. בלי 404: 404 במסך פנימי אומר ש־`cleanUrls` נכנס ל־`vercel.json` (סעיף 4.5).
4. **קובץ האימות של גוגל, אם כבר יש (שלב ב):** 200, בלי הפניה, בלי `X-Robots-Tag`, והתוכן זהה לקובץ.
5. **משהו לא עבר:**
   - **בקוד שחזר מדף ציבורי `#root` ריק:** בודקים ב־Vercel, ביומן הבנייה של הגרסה, את השורה `prerendered`. אין אותה? Vercel לא מריץ את `npm run build` (סעיף 4.3), או שהגרסה עוד לא עלתה. יש אותה? בודקים ש־`vercel.json` בלי `cleanUrls`, ושהקבצים בצורה `dist/<הכתובת>/index.html`. מתקנים בענף `fix/seo`, מעלים לפי "ענפים", ואחרי "מיזגתי" בודקים שוב.
   - **מסך פנימי מחזיר 404:** `cleanUrls` ב־`vercel.json`. מורידים אותו, באותה דרך. זה דחוף: המסכים לא נפתחים מכתובת ישירה.

**נבדק ב־24.11.2026 באתר חי,** בפרויקט בדיקה נפרד ב־Vercel (`ofek-prerender-test`, בחשבון של הדמו), עם עותק של מערכת אופק של הקורס, React 19.3, react-router-dom 7.18, Vite 8.3, ובנייה ב־Node v26.13.1. לא באתר הדמו של הקורס, ולא מול גוגל.
- `/about`, `/privacy` ו־`/services/consulting`: 200, בלי `X-Robots-Tag`, ובקוד שחזר הטקסט, השם, התיאור ו־`canonical` של כל דף, ובלוק הנתונים המובנים בדף האודות ובדף השירות.
- `/`, `/today`, `/clients`, `/index.html`, `/about.html`, `/ABOUT`, `/nonexistent-xyz`, `/services`, `/services/` ו־`/services/test-xyz`: 200, עם `X-Robots-Tag: noindex, nofollow`, ו־`#root` ריק.
- `/about/`: הקובץ המוכן, עם `X-Robots-Tag` (כמו ב־19.11, צעד 8), ו־`canonical` לכתובת בלי `/`. `/about?x=1`: הקובץ המוכן, בלי `X-Robots-Tag`.
- קובץ אימות לדוגמה של גוגל, `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/logo.png` וקבצי `/assets`: 200, בלי `X-Robots-Tag`, וקובץ האימות זהה לקובץ.
- ב־Playwright, על הגרסה האחרונה בייצור: `/privacy` נפתח בלי שום הודעה ב־console, עם כותרת אחת, תיאור אחד ו־`canonical` אחד. קישור ל־`/about` עבר בלי לטעון מחדש, ומשם מסך פנימי (`/today`) וחזרה ל־`/about` החזירו כל פעם את השם והתיאור הנכונים. חזרה מהמסך הפנימי לדף ציבורי נבדקה גם במחשב, ב־`vite preview`.
- (מה שעוד לא נבדק: הבנייה מראש באתר הדמו של הקורס, במערכת בלי נתב באתר חי (נבדקה רק בנייה במחשב), ואיך Search Console מציג את הדף ב"בדיקה של כתובת אתר פעילה".)

### צעד 3: הנתונים המובנים ותגיות השיתוף: רק בודקים

את אלה כתב הסקיל about-page, וכאן לא כותבים אותם שוב:
- בדף `/about`, אחרי שהוא נטען: בלוק `application/ld+json` מסוג `Organization`, עם השם, הכתובת, הלוגו והמייל שבדף.
- ב־`app/index.html`: תגיות ה־`og:` עם הכתובת הקצרה, והלוגו נפתח בכתובת שכתובה בהן.
- משהו חסר או שונה? מתקנים עם הסקיל about-page, אחרי שהיא מאשרת.

### צעד 4: `app/public/robots.txt`

כמו באתר של רות: כל הסורקים מוזמנים, וכל סורק של חיפוש ושל בינה גם בשמו. בראש הקובץ הפניה ל־`llms.txt`, ובסוף הפניה למפת האתר.

```
# llms.txt: https://<הדומיין>/llms.txt

User-agent: *
Allow: /

User-agent: Googlebot
User-agent: Bingbot
User-agent: OAI-SearchBot
User-agent: ChatGPT-User
User-agent: GPTBot
User-agent: PerplexityBot
User-agent: Perplexity-User
User-agent: ClaudeBot
User-agent: Claude-User
User-agent: Claude-SearchBot
User-agent: anthropic-ai
User-agent: Google-Extended
User-agent: Applebot
User-agent: Applebot-Extended
User-agent: CCBot
User-agent: DuckAssistBot
User-agent: MistralAI-User
Allow: /

Sitemap: https://<הדומיין>/sitemap.xml
```

- `<הדומיין>`: הכתובת הקצרה, בלי `https://` ובלי `/` בסוף.
- **אין כאן `Disallow` למסכים הפנימיים.** robots.txt לא מוציא דף מגוגל: דף חסום עדיין יכול להופיע בחיפוש, וגוגל לא רואה את הסימון "לא לחיפוש" של דף שהיא לא נכנסת אליו. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/robots/intro ו־https://developers.google.com/search/docs/crawling-indexing/block-indexing) את המסכים הפנימיים מוציאים בצעד 8. (אם הסורקים של מנועי הבינה מכבדים את הסימון הזה: לא נבדק עדיין.)
- **Google-Extended** קובע אם גוגל משתמשת בתוכן לאימון Gemini ולתשובות שלו. הוא לא משפיע על ההופעה בחיפוש של גוגל. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/google-common-crawlers)
- כמה שורות `User-agent` ברצף הן קבוצה אחת, עם אותו כלל. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/robots/robots_txt)

### צעד 5: `app/public/sitemap.xml`

רק הדפים הציבוריים שנפתחים, כל אחד עם התאריך שבו השתנה.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url><loc>https://<הדומיין>/about</loc><lastmod>YYYY-MM-DD</lastmod></url>
  <url><loc>https://<הדומיין>/privacy</loc><lastmod>YYYY-MM-DD</lastmod></url>
  <url><loc>https://<הדומיין>/terms</loc><lastmod>YYYY-MM-DD</lastmod></url>
  <url><loc>https://<הדומיין>/accessibility</loc><lastmod>YYYY-MM-DD</lastmod></url>
</urlset>
```

- רק דפים שקיימים אצלה. בלי מסכים פנימיים, וגם בלי הכתובת `/`, שהיא המסך הראשון של המערכת.
- כל כתובת מלאה, עם `https://`, בדיוק כמו הכתובת שבה הדף נפתח (בלי `/` בסוף).
- **התאריך (`lastmod`):** בדפים המשפטיים ובהצהרת הנגישות, תאריך העדכון שכתוב בדף. בדף האודות, התאריך של הגרסה האחרונה ששינתה את הקובץ שלו. בלי `priority` ובלי `changefreq`: גוגל מתעלמת מהם. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap)

### צעד 6: `app/public/llms.txt`

לפי הפורמט של llmstxt.org, ובסגנון של `llms.txt` באתר של רות: כותרת עם שם המערכת, משפט סיכום, ואחריהם רשימות של קישורים עם הערה. (הפורמט נבדק ב־https://llmstxt.org, 19.11.2026.)

```
# <שם המערכת>

> <התיאור מדף האודות, מילה במילה>

המערכת של <שם העסק>. <המשפט על העסק, רק אם הוא כתוב בדף האודות>

## אודות

- [<שם המערכת>](https://<הדומיין>/about): <התיאור מדף האודות>

## יצירת קשר

- [יצירת קשר](https://<הדומיין>/about): מייל: <המייל מדף האודות>.
```

- רק מה שכתוב בדף האודות. בלי מחירים, בלי מסכים פנימיים, ובלי שום מידע מתוך המערכת. (נבנו דפים בשלב ה? הם מוסיפים לקובץ את הטקסט שלהם, ורק אותו: שלב ה, צעד 4.)
- הקובץ בעברית, ונשלח כטקסט UTF-8 (צעד 8).
- בדפדפן הקובץ נראה כמו קוד: משמאל לימין, עם `#`, `>` וקישורים. זה תקין. לכן בטיוטה היא רואה את המילים במשפטים (צעד 1), ובסוף השלב היא בודקת דף אחר.

### צעד 7: קובץ המפתח של IndexNow

כמו באתר של רות: **Claude** מייצר מפתח של 32 אותיות וספרות (hex), ושומר קובץ `app/public/<המפתח>.txt`, שיש בו רק את המפתח. המנועים קוראים את הקובץ כדי לדעת שההודעה באה מהאתר. המפתח לא סוד. (נבדק במסמך הרשמי, 19.11.2026: https://www.indexnow.org/documentation) את ההודעה עצמה שולחים בשלב ג.

### צעד 8: `app/vercel.json`: "לא לחיפוש" על המסכים הפנימיים

כמו באתר של רות, שבו האזור הפנימי מקבל את הכותרת `X-Robots-Tag: noindex, nofollow` מ־`vercel.json`. כאן היא חלה על **כל כתובת, חוץ מהדפים הציבוריים, מקובץ האימות של גוגל ומקבצים אמיתיים, לפי הסוג שלהם**. (גוגל: noindex אפשר לתת בכותרת הזו. נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/block-indexing)

מוסיפים ל־`app/vercel.json` את `headers`, ולא נוגעים ב־`rewrites` שכבר שם:

```json
{
  "rewrites": [{ "source": "/(.*)", "destination": "/index.html" }],
  "headers": [
    {
      "source": "/((?!about$|privacy$|terms$|accessibility$)(?!google[0-9a-f]+\\.html$)(?!.*\\.(?:txt|xml|png|jpe?g|svg|ico|webp|js|css|woff2?|map|webmanifest)$).*)",
      "headers": [{ "key": "X-Robots-Tag", "value": "noindex, nofollow" }]
    },
    {
      "source": "/llms.txt",
      "headers": [{ "key": "Content-Type", "value": "text/plain; charset=utf-8" }]
    }
  ]
}
```

- **הרשימה שבסוגריים הראשונים**, `(?!about$|privacy$|terms$|accessibility$)`, היא בדיוק הדפים הציבוריים שנמצאו ב"לפני שמתחילים", כל אחד עם `$` אחריו. דף שלא קיים אצלה לא נכנס לרשימה. (בשאר הסקיל: "הרשימה שבכלל".)
- **שתי החריגות שאחריה** הן הקבצים שבאמת יושבים באתר, והן לא תלויות בדפים: קובץ האימות של גוגל (`google<אותיות וספרות>.html`), וכל קובץ שנגמר באחת הסיומות שברשימה (טקסט, מפת אתר, תמונות, קוד וגופנים). קובץ כזה לא מקבל את הכותרת. ב־JSON כל `\` כתוב פעמיים (`\\.`): כך צריך להיות, ולא מתקנים את זה.
- **כל ה־`(?!...)` בתוך זוג הסוגריים החיצוני**, `/(...)`, כמו בדוגמה. מחוץ לו Vercel לא מקבל את הכלל. (נבדק בספרייה של Vercel, 19.11.2026: `/(?!about$).*` נדחה ככלל לא תקין, ו־`/((?!about$).*)` עבר.)
- **הסיומות מול הקבצים שלה:** משווים את רשימת הסיומות לקבצים שב־`app/public` ולקבצים שהבנייה יוצרת (בדרך כלל `app/dist/assets`). קובץ עם סיומת שלא ברשימה, כמו `.gif`, `.pdf`, `.ttf` או `.json`, יקבל את הכותרת: מוסיפים את הסיומת שלו לרשימה, באותה צורה (`|gif`). רק לא את `html`: אז גם `/index.html` ו־`/about.html` היו יוצאים מהסימון.
- **כתובת עם נקודה שאין מאחוריה קובץ**, כמו `/index.html`, `/about.html` או `/customers.json`, מחזירה את המערכת, ולכן מקבלת את הכותרת, כמו כל מסך פנימי. (בנוסח הקודם של הכלל, שבו כל כתובת עם נקודה יצאה מהכלל, כתובות כאלה החזירו את המערכת בלי הכותרת. נמצא באתר הדמו של הקורס, 19.11.2026.)
- **הפער שנשאר:** כתובת שנגמרת באחת הסיומות שברשימה, או שנראית כמו קובץ האימות של גוגל, ואין מאחוריה קובץ, כמו `/x.png`, `/x.js` או `/google0.html`, מחזירה את המערכת בלי הכותרת. כלל בכותרות לא יודע אם הקובץ קיים. (נבדק באתר הדמו, 19.11.2026.)
- כתובת של דף ציבורי עם `/` בסוף (`/about/`), או באותיות גדולות (`/ABOUT`), כן מקבלת אותה. זה בסדר: במפת האתר הכתובת בלי `/`, ובאותיות כמו בנתב. `/about/` מחזירה את הקובץ המוכן של הדף (צעד 2), עם `canonical` לכתובת בלי `/`, ו־`/ABOUT` מחזירה את `app/index.html`. (נבדק באתר חי, בפרויקט בדיקה, 24.11.2026.)
- כלל ה־`Content-Type` של `llms.txt` הוא כמו באתר של רות. (באתר של רות גם קבצי `.txt` שאין עליהם כלל כזה, כמו `robots.txt` וקובץ המפתח, חוזרים מ־Vercel כ־`text/plain; charset=utf-8`: נבדק ב־19.11.2026, באתר אחד.)
- כבר יש ב־`vercel.json` עוד `headers`? מוסיפים לצידם, לא מוחקים. כלל ישן שנותן `X-Robots-Tag` גם לדף ציבורי מתקנים לפי הטיוטה (צעד 1, סעיף 3). אין `vercel.json` בכלל? אז גם הדפים הציבוריים לא נפתחים באינטרנט (404), כמו בסקילים about-page ו־legal-pages. אומרים לה את זה במשפט, ואחרי שהיא מאשרת יוצרים אותו בתיקייה ש־Vercel בונה ממנה (בדרך כלל `app`), עם כלל ה־`rewrites` ועם `headers`, כמו בדוגמה.
- **בלי `cleanUrls`.** איתו הכלל של `rewrites` מפסיק לעבוד, המסכים הפנימיים מחזירים 404 בכניסה ישירה, וקובץ האימות של גוגל מקבל הפניה (צעד 2, סעיף 4.5). יש כבר `cleanUrls` ב־`vercel.json`? אומרים לה במשפט, ומורידים אותו אחרי שהיא מאשרת.
- **מה נבדק במסמכים ובספרייה:** ש־Vercel מגיש קובץ שקיים בתיקייה לפני כלל ה־`rewrites` (נבדק במסמך הרשמי, 19.11.2026: https://vercel.com/docs/project-configuration/vercel-json, וב־19.11.2026 באתר הדמו של הקורס: `/logo.png` חזר כתמונה). שהתחביר `(?!...)` נכתב בתוך סוגריים (אותו מסמך, בדוגמה של `rewrites`). ושהכלל הזה, עם ארבעת הדפים, מסמן את `/`, `/customers`, `/about/`, `/index.html` ו־`/about.html`, ולא את `/about`, `/privacy`, `/terms`, `/accessibility` והקבצים (נבדק בספרייה של Vercel שקוראת את `vercel.json`, `@vercel/routing-utils` 5.3.3, 19.11.2026).
- **נבדק ב־19.11.2026 באתר חי:** באתר הדמו של הקורס, עם שלושה דפים ציבוריים (שם אין הצהרת נגישות, ולכן ברשימה אין `accessibility$`), בכותרות שחזרו מ־curl. קיבלו `X-Robots-Tag: noindex, nofollow`: `/`, `/customers`, `/index.html`, `/about.html`, `/customers.json`, `/today.php`, `/privacy.`, `/a.b/c`, `/about/` ו־`/ABOUT`. חזרו 200 בלי `X-Robots-Tag`: `/about`, `/privacy` ו־`/terms` (גם `/about?x=1`), `/robots.txt`, `/sitemap.xml`, `/llms.txt`, `/logo.png`, קובץ האימות של גוגל, קובץ המפתח של IndexNow, וקבצי ה־`.js` וה־`.css` שב־`/assets`, ש־`index.html` טוען. בכל זאת, באתר שלה הבדיקה בצעד 10 היא תנאי להמשך.

### צעד 9: בדיקה במחשב, ושמירה

1. **Claude** בודק שאין שגיאות טיפוסים ושהבנייה עוברת. בהרבה פרויקטים הבנייה עצמה בודקת גם את הטיפוסים. בסוף הבנייה השורה `prerendered`, עם כל הדפים הציבוריים, ואחריה הבדיקות של הקבצים המוכנים (צעד 2, סעיף 6). הבנייה נעצרה ב־`prerender failed`? צעד 2, סעיף 5.
2. מריצים את המערכת במחשב, ובודקים ב־Playwright:
   - כל דף ציבורי: הכותרת שלו בלשונית, והתיאור שלו בתגית. ב־head יש **בדיוק `<title>` אחד ובדיוק `meta[name="description"]` אחד**, ושניהם עם הטקסט של הדף הזה.
   - הקובץ המוכן של כל דף, ב־`vite preview`, בכתובת עם `/` בסוף, כמו `/privacy/`: צעד 2, סעיף 6.4. בלי `/` בסוף, במחשב הדף מצויר מהקוד, וזה צפוי.
   - מסך פנימי אחד: הכותרת והתיאור של `app/index.html`, כמו קודם, גם אחרי שעוברים אליו מדף ציבורי.
   - `/robots.txt`, `/sitemap.xml` ו־`/llms.txt`: הטקסט של הקובץ, ולא המערכת.
   - **העברית ב־`llms.txt` יכולה להיראות במחשב שבורה,** סימנים במקום אותיות: השרת שמריץ את המערכת במחשב לא אומר לדפדפן שהקובץ ב־UTF-8. זה צפוי, ולא נוגעים בקובץ. את העברית בודקים באינטרנט (צעד 10), שם `vercel.json` שולח אותו עם `charset=utf-8`. (נבדק בהרצה על אתר הדמו, 19.11.2026: במחשב סימנים, ובאינטרנט אותו קובץ חזר כ־`text/plain; charset=utf-8`.)
   - את הכלל של "לא לחיפוש" אפשר לבדוק רק באינטרנט: `vercel.json` פועל רק ב־Vercel.
3. **שומרים גרסה בענף `feature/seo`, ומעלים ל־GitHub ב־Pull Request**, לפי "ענפים".
   - מוסיפים לגרסה כל קובץ שהשלב יצר או שינה, ורק אותם, לפי השם: הקבצים החדשים ב־`app/public`, `app/vercel.json`, `app/index.html` אם השתנה, קבצי הדפים ששונו, ושל הבנייה מראש: `app/src/public-pages.tsx`, `app/src/PublicPageMeta.tsx`, `app/src/entry-server.tsx`, `app/scripts/prerender.mjs`, `app/src/App.tsx`, `app/package.json`, ו־`app/.gitignore` אם השתנה. `app/dist` ו־`app/dist-ssr` לא נכנסים. לפני ששומרים, בודקים ב־`git status` שלא נשאר בחוץ קובץ של השלב: קובץ שהקוד צריך ולא עלה ל־GitHub מפיל את הבנייה ב־Vercel. בלי `app/scripts/prerender.mjs`, למשל, הבנייה שם נעצרת.
   - `.env`, התיקייה "בדיקות" ו־`.playwright-mcp` לא נכנסים. אומרים לה במשפט מה בדקת.
   - דוחפים את הענף, ונותנים לה קישור ל־Pull Request. מחכים ל"מיזגתי", חוזרים ל־`main`, מושכים, ומוחקים את הענף. רק אז הבדיקה באינטרנט.

### צעד 10: בודקים באינטרנט, ורק אז ממשיכים

1. אחרי "מיזגתי" מחכים שהגרסה החדשה תעלה לייצור, בדרך כלל דקה או שתיים. בודקים בכתובת הקצרה, ולא בכתובת ארוכה של גרסה אחת.
2. **הקבצים:** לכל אחד מ־`/robots.txt`, `/sitemap.xml`, `/llms.txt` ו־`/<המפתח>.txt`, **Claude** בודק גם את סוג התשובה וגם את התוכן:
   - הסוג לא `text/html`. ב־`llms.txt` הוא `text/plain; charset=utf-8`.
   - התוכן שחזר זהה לקובץ.
   - חזר דף המערכת (`text/html`)? הקובץ לא בתיקייה שממנה Vercel בונה, או שהגרסה עוד לא עלתה.
3. **הכלל של "לא לחיפוש":** בודקים את הכותרות (headers) של התשובה:
   - ב־`/`, ב־`/index.html`, ובמסך פנימי נוסף מהנתב, אם יש: `X-Robots-Tag: noindex, nofollow`.
   - בכל דף ציבורי: אין `X-Robots-Tag`. וגם בקוד שחוזר מהכתובת, ולא רק בכותרות: אין תגית `robots` או `googlebot` עם noindex.
   - בקבצים של סעיף 2, בלוגו, ובקבצי הקוד ש־`index.html` טוען: תשובה 200, בלי `X-Robots-Tag`. קובץ עם `X-Robots-Tag`? הסיומת שלו חסרה ברשימה (צעד 8).
4. **בקוד שחוזר, ואחר כך ב־Playwright, בלי להיות מחוברת:** קודם הבדיקות של צעד 2, סעיף 7: בקוד שחוזר מכל דף ציבורי, לפני שהוא רץ, הטקסט שלו, השם, התיאור, `canonical` והנתונים המובנים, ובמסך פנימי `#root` ריק. אחר כך, ב־Playwright, כל דף ציבורי נפתח עם הטקסט שלו ועם הכותרת שלו בלשונית, וב־head שלו בדיוק כותרת אחת, תיאור אחד ו־`canonical` אחד.
5. **אין סוד בקוד של האתר.** (מהקטגוריה Security בבדיקה של רות, audit-website.) **Claude** מוריד את קבצי הקוד ש־`index.html` טוען, וגם כל קובץ `/assets/….js` שהשם שלו מופיע בתוך הקוד שהורד, וכך הלאה, עד שאין שם חדש: כשהקוד מחולק לכמה קבצים, חלק מהם נטענים רק כשעוברים למסך. בכולם הוא בודק, בלי להדפיס שום ערך:
   - `sb_secret_` ואחריו אותיות: מדפיסים רק כמה נמצאו.
   - `sbp_` ואחריו רצף ארוך של אותיות וספרות: מדפיסים רק כמה נמצאו. זו הצורה של הטוקן של Supabase, אחד הסודות שבסקיל backup-and-keep-alive. (נבדק במסמכים של Supabase, 19.11.2026: https://supabase.com/docs/reference/api/introduction ו־https://supabase.com/docs/guides/platform/personal-access-tokens)
   - מפתח בשלושה חלקים, `eyJ….eyJ….…`: מפענחים רק את החלק האמצעי, ומדפיסים רק את התפקיד שכתוב בו (`role`). `anon` תקין: זה המפתח הציבורי. מחרוזת בלי `role` לא נחשבת.
   - **נמצא `service_role`, `sb_secret_` או `sbp_`:** עוצרים. אומרים לה: "בקוד של האתר, שכל אחד יכול לקרוא, יש מפתח שלא אמור להיות שם. זה לא משהו שעשית לא נכון. נעצור כאן, ורות תבדוק." לא מדביקים את הערך לשיחה, ולא ממשיכים לשלב ב. המפתח כבר גלוי באתר החי, ולכן זה צריך להגיע לרות עוד היום: בבית, **Claude** כותב לה עכשיו את ההודעה לרות (ראו "איך מדברים איתה").
6. **משהו לא עבר:** עוצרים, ולא ממשיכים לשלב ב. רישום בגוגל מזמין את הסורקים של גוגל לאתר, ולכן קודם הסימון "לא לחיפוש" צריך לעבוד. מפתח בקוד של האתר חשוף לכל מי שפותחת את הכתובת, גם בלי גוגל, ולכן עוצרים גם עליו.
   - **דף ציבורי עם `X-Robots-Tag`, מכל כלל שהוא, או עם תגית noindex בקוד** הוא הדחוף ביותר: הדף הזה לא ייכנס לגוגל. זה תיקון של מה שנבנה בשלב שהיא אישרה: מתקנים (את הרשימה בכלל, את הכלל הישן, או את התגית) בענף `fix/seo`, מעלים לפי "ענפים", אחרי "מיזגתי" בודקים שוב, ואומרים לה במשפט מה תוקן.
   - **מסך פנימי בלי `X-Robots-Tag`, והגרסה עלתה:** הכלל לא עובד באתר שלה. אומרים לה: "הסימון של המסכים הפנימיים לא עבד אצלך. זה לא משהו שעשית לא נכון. נעצור כאן, ורות תבדוק." לא ממשיכים.
   - **דף ציבורי שבקוד שחוזר ממנו `#root` ריק,** או **מסך פנימי שמחזיר 404:** הבנייה מראש לא עלתה, או ש־`cleanUrls` נכנס ל־`vercel.json`. מה בודקים ואיך מתקנים: צעד 2, סעיף 7.5. 404 במסך פנימי דחוף כמו דף ציבורי עם `X-Robots-Tag`: המסכים לא נפתחים מכתובת ישירה.

בסוף השלב: "הדפים הציבוריים מוכנים לגוגל ולמנועי הבינה, והמסכים הפנימיים מסומנים 'לא לחיפוש'. אפשר לבדוק בעיניים: פתחי את <הדומיין>/<דף>, ותראי בלשונית את השם החדש שלו." (`<דף>`: דף ציבורי שאינו דף האודות, למשל `privacy`. אין כזה? `about`, עם השם שלו בלשונית.)

היא פותחת בכל זאת את `llms.txt`? אומרים לה: "הקובץ נכתב בשביל מנועי הבינה, ולכן בדפדפן הוא נראה כמו קוד. זה תקין."

ואומרים לה: "אפשר לעצור כאן. בפעם הבאה פתחי שיחה חדשה וכתבי: נמשיך את הרישום בגוגל."

## שלב ב: רישום בגוגל, ב־Search Console

מה אומרים לה, בהודעה אחת:
1. "עכשיו נרשום את האתר ב־Search Console, הכלי של גוגל לבעלות אתרים. גוגל תבקש הוכחה שהאתר שלך, ונשים באתר קובץ שהיא נותנת."
2. "אחר כך נשלח לגוגל את מפת האתר, ונבקש להוסיף את דף האודות."
3. "גוגל מוסיפה דפים לאט, בדרך כלל אחרי כמה ימים עד כמה שבועות. היום רושמים ומבקשים, ובעוד שבוע בודקים." (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl)

ובסוף ההודעה, השאלה היחידה בה, לפי מה שנמצא ב"לפני שמתחילים":
- יש בריפו `.github/workflows/backup.yml`: "נרשום את האתר באותו חשבון גוגל של הגיבוי, נכון?"
- אין: "כדאי לרשום את האתר בחשבון הגוגל של האפליקציה בגוגל, בשביל הגיבוי. אם היא עוד לא פתוחה, נפתח אותה אחר כך באותו חשבון. באיזה חשבון גוגל לרשום את האתר?"
  - בלי `backup.yml` האפליקציה בגוגל עדיין יכולה להיות פתוחה, ולכן לא אומרים לה שהיא לא פתוחה.

התשובה שלה היא גם האישור לשלב.

**למה זה טוב גם לאפליקציה בגוגל:** בתנאים של גוגל לאישור האפליקציה יש גם דומיין מאומת ב־Search Console, וגוגל בודקת את זה באימות המותג, בהמשך (כך כתוב בסקיל about-page). אם נכס URL-prefix על כתובת של Vercel מספיק לבדיקה הזו: לא נבדק עדיין. לפרסום האפליקציה בשביל הגיבוי הוא לא היה נחוץ (נבדק ב־19.11.2026, בסקיל backup-and-keep-alive).

### צעד 1: נכנסים ל־Search Console, בחשבון שלה

הסדר חשוב: קודם בודקים אילו חשבונות גוגל כבר מחוברים בחלון, ורק אם החשבון שלה לא ביניהם, מתחברים. בחלון אחד יכולים להיות כמה חשבונות, ו־Search Console נפתח בכל פעם באחד מהם.

1. **Claude: אילו חשבונות מחוברים.** פותח ב־Playwright את `https://search.google.com/u/0/search-console`, ואחריו `/u/1/`, `/u/2/` וכן הלאה, וקורא בכל אחד את המייל שבכפתור החשבון בפינה ("חשבון Google: <השם> (<המייל>)"). כך הוא מוצא את המספר של החשבון שהיא אמרה. (שיטת המעבר על המספרים, ואיך נראית כתובת עם מספר שאין מאחוריו חשבון: לא נבדק עדיין. נבדק ב־19.11.2026 רק ש־`/u/<n>/search-console` של החשבון של הדמו נפתח ישר, בלי סיסמה, עם המייל שלו בכפתור.)
   - **דף ההסבר של Search Console** (`/search-console/about`) לא אומר שאין חשבון מחובר. בהרצה של 19.11.2026 הכתובת `https://search.google.com/search-console` עברה אליו כששלושה חשבונות היו מחוברים בחלון, וגם החשבון של הדמו ביניהם.
2. **החשבון שלה מחובר:** **Claude** ממשיך ב־`https://search.google.com/u/<n>/search-console` שלו, ומוודא לפי הכפתור בפינה (כך עובדים אצל רות). המייל לא ברור? שואלים פעם אחת: "זה החשבון <המייל>, נכון?". ממשיכים לסעיף 5.
3. **החשבון שלה לא מחובר:** רק אז **Claude** לוחץ בדף ההסבר על כפתור ההתחלה, לפי השם שלו במסך: **קדימה, מתחילים** (בדף באנגלית: **Start now**).
   - **במסך שמראה מייל של מישהו אחר לא מקלידים סיסמה.** בהרצה, הכפתור הוביל למסך "זה החשבון שלך?" של החשבון הראשון בחלון, ולא של החשבון שנבחר, עם הכפתור **הבא**. מסך כזה **Claude** לא מעביר לה. הוא מחפש בו דרך לחשבון אחר, לפי השם במסך (בבחירת החשבון של גוגל היא נקראה **החלפת חשבון**). לא מצא? נעצור כאן, ורות תבדוק.
4. **מופיע מסך הכניסה של גוגל, בלי מייל או עם המייל שלה. את:**
   1. הקלידי את המייל ואת הסיסמה של חשבון הגוגל שלך. את הסיסמה רק את מקלידה.
   2. מופיע במסך מייל שאינו שלך? אל תקלידי סיסמה, וכתבי לי: מופיע מייל אחר.
   3. גוגל מבקשת לוודא שזו את? בחרי אימות במייל. לא SMS, ולא אימות דו־שלבי.
   4. כשמופיע Search Console, כתבי לי: התחברתי.

   אחרי הכניסה **Claude** מוצא את המספר של החשבון שלה, כמו בסעיף 1, וממשיך ב־`/u/<n>/` שלו. היא כתבה "מופיע מייל אחר"? ממשיכים לפי סעיף 3.
5. **מסך תנאים או הסכמה בכניסה הראשונה:** בהרצה של 19.11.2026 לא הופיע מסך כזה: החשבון נכנס ישר למסך "ברוכים הבאים ל-Google Search Console". (אם החשבון פתח את Search Console לפני כן: לא ידוע.) מופיע בכל זאת? **Claude** מצלם את המסך, וכותב לה את השמות כמו במסך.
   **את:**
   1. קראי.
   2. סמני את התיבה <השם שלה, כמו במסך>.
   3. לחצי על <הכפתור, כמו במסך>.
   4. כתבי לי: סיימתי.
6. **גוגל לא נותנת להתחבר בחלון של Playwright:** עוברים לתוכנית ב, בסוף השלב.

### צעד 2: הנכס

1. **Claude:** בודק ברשימת הנכסים אם הכתובת כבר שם.
   - כבר שם ומאומתת: ממשיכים לצעד 5.
   - כבר שם ולא מאומתת: ממשיכים מצעד 3, באותו נכס.
2. **Claude:** במסך "ברוכים הבאים ל-Google Search Console" לוחץ **הוספת אתר** (בחשבון שכבר יש בו נכסים: **+ Add property**, ברשימת הנכסים). בחלון **בחירת סוג הנכס** בוחר **קידומת של כתובת URL** (URL prefix), וכותב בשדה שלה את הכתובת בדיוק כך: `https://<הדומיין>/`. עם `https://`, הכתובת הקצרה, ו־`/` בסוף. לוחץ **המשך** (Continue) שמתחת לשדה הזה: לכל אחד משני הסוגים יש **המשך** משלו.
   - לא **דומיין** (Domain), גם כשהוא המסומן כשהחלון נפתח: הוא דורש רשומה אצל ספק הדומיין, ובכתובת של Vercel אין לה גישה לזה.
   - (נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/34592 ו־https://support.google.com/webmasters/answer/9008080. המסלול במסך נבדק בהרצה של 19.11.2026, בחשבון בלי נכסים: "הוספת אתר", "בחירת סוג הנכס", "קידומת של כתובת URL", "המשך". הדרך מרשימת הנכסים, בחשבון שכבר יש בו נכס: לא נבדק עדיין.)

### צעד 3: קובץ האימות

כמו באתר של רות, שבו קובץ האימות של גוגל יושב בתיקייה `public`.

1. **Claude:** בחלון **אימות בעלות** בוחר בשיטה **קובץ HTML** (HTML file). בהרצה של 19.11.2026 היא כבר הייתה פתוחה, תחת "שיטת אימות מומלצת". מוריד את הקובץ מהשורה "הורדת הקובץ". השם שלו במסך הוא `google<אותיות וספרות>.html`.
   - את המקום של הקובץ לוקחים מההודעה של Playwright על ההורדה. Playwright שומר הורדות לפעמים בשם אחר (כך קרה בסקיל backup-and-keep-alive. בהרצה של הסקיל הזה השם נשאר). מחזירים לקובץ את השם המדויק מהמסך, ומעבירים אותו ל־`app/public`. את התוכן לא משנים בכלל. (גוגל: לא משנים את השם ואת התוכן של הקובץ. נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/9008080)
   - את החלון של גוגל משאירים פתוח, עד הלחיצה על **אמת** (Verify).
   - ההורדה לא הגיעה גם בפעם השנייה? עוברים לשיטה **תג HTML** (HTML tag), תחת "שיטות אימות אחרות" באותו חלון: **Claude** מעתיק את התגית (`google-site-verification`, היא לא סוד) ל־head של `app/index.html`. גם היא נשארת שם תמיד. (שהתגית עובדת כש־`/` מסומן "לא לחיפוש", וגם אחרי שתתווסף כניסה עם גוגל: לא נבדק עדיין. גוגל דורשת שדף הבית ייפתח בלי כניסה, ובודקת את התגית מדי פעם. לכן קובץ ה־HTML הוא הדרך הראשונה. נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/9008080)
2. **Claude: שומרים גרסה ומעלים**, רק עם קובץ האימות, בענף `feature/google-verification`, לפי "ענפים": Pull Request, והיא ממזגת. את החלון של גוגל משאירים פתוח גם בזמן המיזוג.
3. **Claude: בודקים באינטרנט:** אחרי "מיזגתי" מחכים שהגרסה תעלה לייצור, ופותחים את `https://<הדומיין>/google….html`. **התוכן שחזר זהה לקובץ, ובלי `X-Robots-Tag`** (הכלל של שלב א, צעד 8, מוציא את הקובץ הזה מהסימון). חזר דף המערכת? הקובץ לא במקום, או שהגרסה עוד לא עלתה. (כאן סוג התשובה לא עוזר: גם הקובץ וגם דף המערכת הם `text/html`.) בשיטת התגית: בודקים שהתגית נמצאת בקוד שחוזר מ־`https://<הדומיין>/`.
4. **הקובץ נשאר באתר תמיד.** בלעדיו גוגל מבטלת את האימות. (נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/9008080) אומרים לה את זה במשפט.

### צעד 4: מאמתים

1. **Claude:** חוזר לחלון של גוגל, ולוחץ **אמת** (Verify).
2. בודקים בצילום מסך שכתוב **הבעלות אומתה** (Ownership verified), ומתחת "שיטת אימות: קובץ HTML". אומרים לה מה כתוב, כמו במסך, ובמשפט: "גוגל ראתה את הקובץ, ויודעת שהאתר שלך." אחר כך **Claude** לוחץ **מעבר לנכס** (Go to property). (נבדק בהרצה של 19.11.2026: כך נראה המסך, עם הכפתורים **בוצע** ו־**מעבר לנכס**.)
3. לא אומת? לפי "כשמשהו נכשל". גוגל לא עוקבת אחרי הפניה כשהיא מחפשת את הקובץ, ולכן הכתובת של הנכס צריכה להיות בדיוק הכתובת שבה הקובץ נפתח.

### צעד 5: שולחים את מפת האתר

מכאן והלאה, בכל דף של Search Console יכולה לקפוץ בועת הסבר שמסתירה חלק מהמסך. **Claude** סוגר אותה ב־**הבנתי**.

1. **Claude:** בתפריט של הנכס, תחת **הוספה לאינדקס** (Indexing), לוחץ **Sitemaps**. השם נשאר באנגלית גם במסך בעברית. בחלון צר התפריט מוסתר מאחורי הכפתור **התפריט הראשי**. בתיבה **הוספת sitemap חדש** (Add a new sitemap) כותב `sitemap.xml`, ולוחץ **שלח** (Submit). נפתח החלון "Sitemap נשלח בהצלחה", ו־**Claude** סוגר אותו ב־**סגור**.
2. מה רואים בטבלה, ומה אומרים לה:
   - **הצלחה** (Success), עם מספר ב"דפים שהתגלו": גוגל קיבלה את המפה. אומרים לה: "גוגל קיבלה את מפת האתר. זה עוד לא אומר שהדפים כבר בחיפוש." (בהרצה של 19.11.2026 המצב הופיע מיד, עם 3 דפים שהתגלו.)
   - **Couldn't fetch:** גוגל לא הצליחה להוריד את הקובץ. **Claude** בודק שוב את `https://<הדומיין>/sitemap.xml` (שלב א, צעד 10). הקובץ תקין? בודקים שוב מאוחר יותר, או מחר.
   - (נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/7451001. מפת אתר היא רמז לגוגל, לא התחייבות שתסרוק את כל הדפים.)

### צעד 6: בקשה להוסיף את דף האודות

1. **לפני הבדיקה**, אומרים לה במשפט: "עכשיו יופיע שדף האודות עוד לא בגוגל. באתר חדש זה רגיל, ובשביל זה מבקשים."
2. **Claude:** בשורה שבראש המסך ("ניתן לבדוק כל כתובת אתר ב-…"), או ב־**בדיקת דף** (URL inspection) שבתפריט, כותב `https://<הדומיין>/about`. נפתח הדף "בדיקת כתובת אתר".
   - **כתובת האתר לא נמצאת ב-Google** (URL is not on Google), ובפרטים "הדף לא נוסף לאינדקס: כתובת האתר לא ידועה ל-Google": באתר חדש זה רגיל.
3. **Claude:** לוחץ **הגש בקשה ליצירת אינדקס** (Request indexing). מופיע "מתבצעת בדיקה אם ניתן להוסיף לאינדקס את כתובת האתר הפעילה", לדקה או שתיים. מחכים שיופיע אישור שהבקשה התקבלה, ואומרים לה: "גוגל קיבלה את הבקשה. זה עוד לא אומר שהדף כבר בחיפוש." (איך נראה האישור: לא נבדק עדיין. בהרצה של 19.11.2026 הבקשה הראשונה קיבלה את ההודעה שבסעיף 4.)
4. **"חרגת מהמכסה":** זו המכסה היומית, והיא יכולה להופיע גם בבקשה הראשונה, בנכס חדש. במסך: "חרגת מהמכסה", ומתחת: "מצטערים, לא הצלחנו לעבד את הבקשה מפני שחרגת מהמכסה היומית. יש לנסות להגיש זאת שוב מחר.", עם הכפתור **סגור**. אומרים לה את ההודעה כמו שהיא, ובמשפט: "זו המכסה היומית של גוגל. זה לא משהו שעשית לא נכון, ונבקש שוב מחר." היום לא מנסים שוב. בסוף השלב אומרים לה את הנוסח של בקשה שלא התקבלה (למטה), ובפעם הבאה מבקשים פעם אחת ("לפני שמתחילים", סעיף 5). (גוגל: יש מכסה יומית לבקשות, בלי מספר. ברישום של רות כתוב "מכסה ~10 ליום", אבל בפועל, ב־14.10 וב־17.10, התקבלה אצלה בקשה אחת ביום, ולבקשה שאחריה הופיע "נסה שוב מאוחר יותר". ובהרצה על אתר הדמו, 19.11.2026, כבר הבקשה הראשונה, בנכס חדש ובחשבון בלי נכסים אחרים, קיבלה "חרגת מהמכסה". הסיבה לא ידועה.)
5. **רק `/about`.** שאר הדפים מגיעים לגוגל ממפת האתר, ובקשה חוזרת לאותה כתובת לא מזרזת. (נבדק במסמך הרשמי, 19.11.2026: https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl ו־https://support.google.com/webmasters/answer/9012289)
- **אפשר גם:** באותה בדיקה של `/about`, **בדיקה של כתובת אתר פעילה** (Test live URL) בודקת את הדף כמו שהוא עכשיו, ומראה אם הוא כנראה יכול להיכנס לגוגל, עם הדף כמו שגוגל רואה אותו. היא לא בקשה להוספה. (נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/9012289. המסך נבדק בהרצה של 19.11.2026, גם אחרי "חרגת מהמכסה": אחרי כחצי דקה הופיעו **כתובת האתר זמינה ל-Google** (URL is available to Google) ו־**ניתן להוסיף את הדף לאינדקס** (Page can be indexed), וב־**פתיחת הדף שנבדק** (View tested page) הקוד שגוגל ראתה, עם כותרת אחת ותיאור אחד.)

בסוף השלב: "האתר שלך רשום ב־Search Console, בחשבון <החשבון>. מפת האתר נשלחה, וביקשנו מגוגל להוסיף את דף האודות. גוגל תוסיף אותו לאט, ובעוד שבוע נבדוק. אפשר לראות את זה ב־Search Console, בחשבון שלך."

גוגל לא קיבלה היום את הבקשה (צעד 6, סעיף 4)? אז: "האתר שלך רשום ב־Search Console, בחשבון <החשבון>. מפת האתר נשלחה. את הבקשה להוסיף את דף האודות גוגל לא קיבלה היום, בגלל המכסה היומית. גוגל תוסיף את הדפים לאט, ובעוד שבוע נבדוק. אפשר לראות את זה ב־Search Console, בחשבון שלך." ומיד אחר כך: «מחר כתבי לי: "נבקש שוב מגוגל להוסיף את דף האודות".»

ואומרים לה: "אפשר לעצור כאן. בפעם הבאה פתחי שיחה חדשה וכתבי: נמשיך עם Bing."

### תוכנית ב: בדפדפן הרגיל שלה

כשגוגל לא נותנת להתחבר בחלון של Playwright. כמו בסקיל backup-and-keep-alive: היא עושה את הצעדים בדפדפן הרגיל שלה, ו־**Claude** כותב לה כל חלק ברשימה ממוספרת, עם הקישור המלא ועם שמות הכפתורים כמו בצעדים 2 עד 6. **Claude** לא רואה את הדפדפן שלה, ולכן אחרי כל חלק היא כותבת לו מה כתוב במסך:

1. **הנכס וקובץ האימות** (צעדים 2 ו־3): מוסיפים את הנכס, בוחרים **קובץ HTML** (במסך באנגלית: HTML file), ומורידים את הקובץ. בסוף: "כתבי לי: הורדתי."
2. **Claude:** מוצא את הקובץ בתיקיית ההורדות, מחזיר לו את השם המדויק (`google<אותיות וספרות>.html`) אם הדפדפן שינה אותו, מעביר אותו ל־`app/public` בלי שום שינוי בתוכן, שומר גרסה ומעלה כמו בצעד 3, ואחרי "מיזגתי" בודק באינטרנט (צעד 3). רק אחרי שהבדיקה עברה הוא כותב לה: "לחצי אמת (במסך באנגלית: Verify), וכתבי לי מה כתוב."
3. **מפת האתר** (צעד 5). בסוף: "כתבי לי מה כתוב."
4. **הבקשה להוסיף את דף האודות** (צעד 6). בסוף: "כתבי לי מה כתוב." כתוב "חרגת מהמכסה"? כמו בצעד 6, סעיף 4, ובסוף השלב הנוסח של בקשה שלא התקבלה.

אחרי כל תשובה שלה, **Claude** אומר לה במשפט אחד מה זה אומר, באותן מילים כמו בצעדים 4 עד 6.

## שלב ג: מנועי הבינה ו־Bing

מה אומרים לה, בהודעה אחת:
1. "מנועי הבינה כבר מוזמנים: ב־robots.txt כל אחד מהם בשמו. ו־llms.txt, קובץ שחלק מכלי הבינה קוראים, מספר מה המערכת ושל מי."
2. "נשאר Bing, מנוע החיפוש של מיקרוסופט. לפי Bing, הוא עומד גם מאחורי כלים אחרים, כמו ChatGPT. אצלו לא צריך קובץ אימות: מייבאים את האתר מ־Search Console."
3. "בסוף אשלח ל־Bing ולמנועים נוספים הודעה על הדפים שלך. זה נקרא IndexNow, ואת זה אני עושה לבד."

ובסוף ההודעה, השאלה היחידה בה: "Bing יבקש הרשאה לראות את האתרים שלך ב־Search Console. ככה הוא יודע שהאתר שלך, ולוקח משם את מפת האתר. זה בסדר?" התשובה שלה היא גם האישור לשלב.

(Bing על עצמו: נבדק בבלוג הרשמי של Bing, 19.11.2026: https://blogs.bing.com/webmaster/2025/6/Start-Using-Bing-Webmaster-Tools-to-Improve-Your-Site-Visibility/)

### צעד 1: Bing Webmaster Tools, בייבוא מ־Search Console

כמו אצל רות: ייבוא מ־Search Console, שמאמת את האתר ולוקח גם את מפת האתר. בהרצה של 19.11.2026 Bing היה באנגלית, והמסכים של גוגל בתוכו בעברית. כל המסכים, גם של גוגל, נפתחים **באותה לשונית**, ולא בחלון חדש.

1. **Claude:** פותח ב־Playwright את `https://www.bing.com/webmasters`. הכתובת עוברת לדף הפתיחה של Bing Webmaster Tools ("Want more users for your site?"). **Claude** לוחץ למעלה **Sign In**, ובחלון "Please sign in" על הכרטיס **Google**.
2. **את:**
   1. במסך של גוגל "עליך לבחור חשבון", בחרי את אותו חשבון גוגל. מבקשים סיסמה? הקלידי אותה, רק במסך שמראה את המייל שלך. את הסיסמה רק את מקלידה.
   2. במסך "כניסה אל bing.com" לחצי **המשך**.
   3. כתבי לי: התחברתי.
3. **Claude:** במסך "Welcome to Bing Webmaster Tools", תחת Google Search Console, לוחץ **Import**. בדף של Bing, "Import from Google Search Console", לוחץ **Continue**. (בחשבון שכבר יש בו אתרים, Import נמצא גם בדף **My Sites**: לא נבדק עדיין.)
4. **את:** במסך "עליך לבחור חשבון" בחרי שוב את אותו חשבון. במסך "מתבצעת התחברות מחדש אל bing.com" לחצי **המשך**, וכתבי לי: בחרתי.
5. **Claude:** מצלם את המסך, וכותב לה את הכפתור הבא, בדיוק כמו במסך. בהרצה זה היה המסך "האפליקציה bing.com מבקשת גישה לנתונים נוספים בחשבון Google שלך", בלי תיבה לסמן, והכפתור **המשך**. (בפוסט של Bing מ־2019 הכפתור נקרא **Allow**. במסך בעברית יש **המשך** פעמיים בייבוא: בסעיף 4, וכאן.)
   **את:**
   1. לחצי <הכפתור, כמו במסך>.
   2. כתבי לי: אישרתי.
6. **Claude:** ברשימת האתרים ("Please select the sites which you want to import.") האתרים מגיעים מסומנים. **Claude** מוריד את הסימון מכל אתר אחר, משאיר רק את הכתובת של המערכת, ולוחץ **Import**. (בהרצה היה בחשבון אתר אחד, והוא הגיע מסומן. גם אצל רות יובא רק האתר שהיה צריך.)
7. **אחרי Import חוזר מסך הפתיחה הריק, "Welcome to Bing Webmaster Tools", בלי שום אישור.** זה תקין: לא מייבאים שוב, ולא שואלים אותה. **Claude** טוען מחדש את הדף, ופותח את Sitemaps של האתר. בהרצה הגיעו לשם בכתובת `https://www.bing.com/webmasters/sitemaps?siteUrl=<כתובת האתר>`. (באיזו צורה בדיוק נכתבה שם כתובת האתר: לא נבדק שוב.) שם הוא בודק שמפת האתר ברשימה, במצב **Success**, או, כמו אצל רות בהתחלה, "Imported - Processing".

- נתוני תנועה של אתר שאומת עכשיו יכולים לקחת עד 48 שעות. אתר שיובא מאומת לבד, ו־Bing בודק מדי פעם מול Search Console שהוא עדיין שלה. (נבדק בבלוג הרשמי של Bing, 19.11.2026: https://blogs.bing.com/webmaster/2019/9/Import-sites-from-Search-Console-to-Bing-Webmaster-Tools/. זה פוסט מ־2019, ודף העזרה של Bing לא נטען. המסלול במסך נבדק בהרצה על אתר הדמו, 19.11.2026, בחשבון בלי אתרים ב־Bing: אחרי הטעינה מחדש, בדף Sitemaps הייתה מפת אתר אחת, במצב Success, עם 3 כתובות.)
- **מסך פתיחה ריק לפני הייבוא:** בחשבון חדש זו ההתחלה הרגילה, ומייבאים ממנו (סעיף 3). היא כבר פתחה בעבר חשבון ב־Bing Webmaster Tools, ובכל זאת המסך ריק לפני הייבוא? אולי אז נכנסה בדרך אחרת, למשל עם חשבון Microsoft. שואלים אותה פעם אחת איך נכנסה אז. (אצל רות הופיע מסך כזה, והסיבה לא בוררה. הייבוא עבד ממנו, בכניסה עם Google.) מסך ריק **אחרי** Import: סעיף 7.

### צעד 2: הודעה ב־IndexNow

את זה **Claude** עושה לבד, בלי לחיצות שלה. כמו אצל רות, אחרי שהגרסה עם קובץ המפתח בייצור (שלב א, צעד 10).

1. בודקים ש־`https://<הדומיין>/<המפתח>.txt` מחזיר בדיוק את המפתח.
2. שולחים בקשה אחת, `POST` עם JSON, ל־`https://api.indexnow.org/indexnow`:
   ```json
   {
     "host": "<הדומיין>",
     "key": "<המפתח>",
     "keyLocation": "https://<הדומיין>/<המפתח>.txt",
     "urlList": ["https://<הדומיין>/about", "https://<הדומיין>/privacy", "https://<הדומיין>/terms"]
   }
   ```
   - `urlList`: כל הכתובות שבמפת האתר, ורק הן.
   - שולחים מקובץ, כמו את ה־SQL בסקיל backup-and-keep-alive, ועם `Content-Type: application/json; charset=utf-8`.
3. **התשובה:** 200 או 202, ההודעה התקבלה. 403, המפתח לא נמצא או לא תואם. 422, כתובת שלא שייכת לאתר. 429, יותר מדי בקשות.
4. **אין תשובה בכלל:** אצל רות `api.indexnow.org` לא ענה מהמחשב שלה, ו־`https://www.bing.com/indexnow` ענה 200. שולחים לשם את אותה בקשה.
- בקשה לכתובת אחת מגיעה לכל המנועים שב־IndexNow. גוגל לא ברשימה שלהם. לא שולחים שוב כתובות שלא השתנו. (נבדק במסמכים הרשמיים, 19.11.2026: https://www.indexnow.org/documentation, https://www.indexnow.org/faq ו־https://www.indexnow.org/searchengines.json)

בסוף השלב: "האתר רשום עכשיו ב־Bing Webmaster Tools, ומנועים נוספים קיבלו הודעה על הדפים. זה עוד לא אומר שהדפים כבר בחיפוש של Bing. נתונים יכולים להתחיל להופיע שם אחרי עד יומיים, בכתובת https://www.bing.com/webmasters."

### מה לא בשלב הזה

הסקיל ai-seo של רות מדבר גם על ניסוח תוכן שמנועי בינה מצטטים, שאלות ותשובות, נתונים וציטוטים, נוכחות באתרים אחרים, ומעקב אחרי ציטוטים. במערכת ניהול, הדפים הציבוריים של שלבים א עד ד הם דף זהות ודפים משפטיים, ואין בהם תוכן כזה. לכן בשלבים האלה הסקיל לא משנה טקסט בדפים, ולא כותב תוכן חדש. דפים על מה שהעסק נותן, עם תשובה בראש כל חלק, ודף של שאלות נפוצות, הם שלב ה, לא חובה. נוכחות באתרים אחרים ומעקב אחרי ציטוטים לא בסקיל בכלל.

## שלב ד: בדיקה

### מה Claude בודק באינטרנט

בכתובת הקצרה, בלי להיות מחוברת. אלה הבדיקות מהקטגוריות של הבדיקה המלאה של רות (audit-website) שנוגעות לדפים הציבוריים:

| מה בודקים | איך | הקטגוריה אצל רות |
|---|---|---|
| לכל דף ציבורי כותרת ותיאור, שונים מהדפים האחרים, וב־head בדיוק כותרת אחת, תיאור אחד ו־`canonical` אחד | בקוד שחוזר (curl), ואחר כך ב־Playwright, אחרי שהדף נטען | Core SEO |
| הטקסט של כל דף ציבורי בקוד שחוזר, לפני שהקוד רץ, ו־`#root` ריק במסכים הפנימיים | curl (שלב א, צעד 2, סעיף 7) | Crawlability |
| תגיות ה־`og:` עם הכתובת הקצרה, והלוגו נפתח | הקובץ `app/index.html` בייצור | Social |
| הנתונים המובנים בדף האודות: JSON תקין, עם השם, הכתובת, הלוגו והמייל שבדף | בקוד שחוזר (curl), ואחר כך ב־Playwright, אחרי שהדף נטען | Schema |
| בדפים של שלב ה, אם נבנו: `Service` בכל דף שירות ו־`FAQPage` בדף השאלות, JSON תקין, עם אותו טקסט כמו בדף | בקוד שחוזר (curl), ואחר כך ב־Playwright, אחרי שהדף נטען | Schema |
| `robots.txt`, `sitemap.xml` ו־`llms.txt`: הסוג והתוכן, וכל כתובת במפת האתר נפתחת עם הטקסט שלה | curl ו־Playwright | Crawlability |
| "לא לחיפוש" על `/`, על `/index.html` ועל מסך פנימי, ולא על הדפים הציבוריים ועל הקבצים: לא בכותרות, ולא בתגית בקוד | הכותרות והקוד של התשובה | Crawlability |
| כותרת ראשית אחת בכל דף ציבורי, וטקסט חלופי ללוגו | Playwright | Content, Images |
| הקישורים בין הדפים הציבוריים הם קישורים רגילים, ונפתחים | Playwright | Links |
| הכול ב־`https`: הלוגו, התגיות והקישורים | הקובץ בייצור | Security |
| אין מפתח סודי של Supabase (`service_role`, `sb_secret_`) ולא הטוקן שלה (`sbp_`) בקוד שהאתר שולח לדפדפן | בודקים שוב, כמו בשלב א, צעד 10, בכל קבצי הקוד. רק הצורות של Supabase, לא כל הצורות שבודק audit-website | Security |

מה שהסקילים האחרים כבר בודקים (רוחב צר, בינוני ורחב, נגישות, הדפים המשפטיים) לא בודקים כאן שוב.

### ב־Search Console, עכשיו ובעוד שבוע

את המצב אומרים לה כמו שהוא כתוב במסך, ואחר כך משפט אחד מה הוא אומר. השמות כאן כמו במסך בעברית בהרצה של 19.11.2026, ובסוגריים כמו במסמכים של גוגל, באנגלית. מצב שכתוב כאן רק באנגלית לא נראה בהרצה: את השם בעברית מעתיקים מהמסך.

- **עכשיו:** הנכס מאומת, מפת האתר ב־**הצלחה** (Success), והבקשה ל־`/about` התקבלה, או מחכה למחר בגלל המכסה היומית (שלב ב, צעד 6).
- **כבר ביום הראשון, וגם אחר כך:** **נסרק אך לא נכלל באינדקס** (Crawled - currently not indexed). בפרטים של בדיקת הדף: "הדף לא נוסף לאינדקס: נסרק אך לא נכלל באינדקס". גוגל ראתה את הדף ועוד לא הוסיפה אותו. זה נפוץ, ואין מה לתקן. בודקים שוב מאוחר יותר. (בהרצה של 19.11.2026 זה הופיע ב־`/privacy` כבר באותו יום, אחרי שמפת האתר נשלחה, בלי בקשה להוספה. גם אצל רות רוב הדפים היו כך בהתחלה.)
- **בעוד שבוע בערך** (גוגל: אתר חדש מתחיל להיסרק בדרך כלל אחרי שבוע בערך):
  - **URL is on Google** בבדיקה של `/about`: הדף באינדקס, ויכול להופיע בחיפוש.
  - המסכים הפנימיים בדוח הדפים (**הוספה לאינדקס** ← **דפים**), בסיבה של noindex: כך צריך להיות.
  - (נבדק במסמך הרשמי, 19.11.2026: https://support.google.com/webmasters/answer/7440203)
- **מייל מגוגל על דפים שלא נכנסו לחיפוש בגלל noindex:** אם מייל כזה מגיע: לא נבדק עדיין. (במסמך של גוגל על דוח הדפים כתוב רק על הודעות אחרי תיקון.) היא שואלת על מייל כזה? אלה המסכים הפנימיים, כמו שתכננו.
- כשהיא כותבת "תבדוק אם האתר בגוגל": **Claude** פותח את Search Console ב־Playwright, בודק את `/about` ואת דוח הדפים, ואומר לה בשתי שורות מה מצא.
- כשהיא כותבת "נבקש שוב מגוגל להוסיף את דף האודות": **Claude** פותח את Search Console ב־Playwright, בחשבון שלה (שלב ב, צעד 1), ובודק את `/about` כמו ב"לפני שמתחילים", סעיף 5. עדיין "כתובת האתר לא ידועה ל-Google"? מבקש פעם אחת (שלב ב, צעד 6). ואומר לה במשפט מה כתוב במסך.
- היא יכולה גם לחפש בגוגל את שם המערכת יחד עם שם העסק, אחרי שגוגל תוסיף את הדף, או לשאול את ChatGPT על העסק (כמו הבדיקה הידנית בסקיל ai-seo). זה לוקח זמן, ולא מובטח.

### הבדיקה המלאה של רות (audit-website)

לרות יש סקיל משלה, audit-website, שעובד עם התוכנה squirrel של squirrelscan. היא סורקת אתר שלם מול יותר מ־230 כללים: תגיות, קישורים שבורים, נתונים מובנים, robots ומפת אתר, תמונות, אבטחה ועוד, ומחזירה ציון וממצאים. אצל רות היא מותקנת במחשב שלה, ומריצים אותה על כתובת חיה: קודם סריקה רדודה (surface), אחר כך עמוקה, ומתקנים בסבבים עד ציון 95 בכיסוי מלא (full).

**בסקיל הזה לא משתמשים בה אצל התלמידה.** למה:
- זו תוכנה נפרדת, שמורידים ידנית ל־Windows: קובץ של כ־130MB. (נבדק ב־https://squirrelscan.com/download, 19.11.2026.) אצל רות היא מותקנת מגרסה רשמית של squirrelscan, אחרי בדיקת checksum. זה לא צעד לפעם הראשונה של תלמידה.
- היא בנויה לאתר שלם. היעד שלה, 95 ומעלה בכיסוי מלא, לא מתאים לשלושה או ארבעה דפים ציבוריים.
- את הבדיקות שנוגעות לדפים האלה Claude עושה ישירות, בטבלה שלמעלה.

אם היא שואלת עליה: אומרים לה שזה כלי שרות משתמשת בו באתרים שלה, ושאצלה Claude עשה את אותן בדיקות על הדפים הציבוריים. לא מתקינים אותה.

## שלב ה: דפים שעוזרים לחיפוש

(השלב הזה נכתב ב־24.11.2026, ועוד לא נבדק בהרצה מלאה. מה שנבדק כתוב ליד כל דבר, עם התאריך. הבנייה מראש של דף שירות, בכתובת עם שתי רמות (`/services/<slug>`), נבדקה ב־24.11.2026 באתר חי, בפרויקט בדיקה נפרד ולא באתר הדמו של הקורס: שלב א, צעד 2.)

השלב הזה בא אחרי שלב ד, והוא לא חלק מהרישום. אפשר לעשות אותו בשיעור או בבית, ולחזור אליו בכל פעם שנוסף שירות. מתחילים אותו כשהיא כותבת "נבנה דפים שעוזרים לחיפוש" או "נוסף שירות", או כשהיא מבקשת דף לשירות או דף של שאלות נפוצות.

**מה הוא עושה:** עד כאן, בחיפוש רק דף האודות והדפים המשפטיים. הם אומרים מה המערכת ושל מי, ולא מה העסק נותן. בשלב הזה נבנים עוד שלושה עד שישה דפים ציבוריים, שעונים למי שמחפשת את מה שהעסק נותן: דף לכל שירות אמיתי (או לכל סוג אירוע, או לקהל שמקבל שירות אחר), ודף אחד של שאלות נפוצות. כל דף נבנה רק מפרטים שכתובים בקבצים שלה, או שהיא אמרה.

**מה זה לא:** זה לא מבטיח מקום בחיפוש, תנועה או לקוחות. זה נותן לגוגל ולמנועי הבינה משהו אמיתי לקרוא על העסק. (גוגל: תוכן מועיל, שנכתב בשביל אנשים, עם מידע מקורי וידע מכלי ראשון. נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/fundamentals/creating-helpful-content)

### לפני השלב

1. **שלב א נעשה, והבדיקה בייצור שלו עברה** (שלב א, צעד 10): ב־`app/vercel.json` יש הכלל של "לא לחיפוש", ב־`app/public` יש `sitemap.xml` ו־`llms.txt`, ויש בנייה מראש: `app/src/public-pages.tsx`, `app/scripts/prerender.mjs`, והשורה `prerendered` בסוף `npm run build` (שלב א, צעד 2). לא? עוצרים, ואומרים לה במשפט שקודם מכינים לגוגל את הדפים הקיימים (שלב א). הדפים החדשים נכנסים לאותה רשימה, לאותו כלל, לאותה מפת אתר ולאותו קובץ.
   - שלב א נעשה לפני שהבנייה מראש נכנסה לסקיל, ואין `app/scripts/prerender.mjs`? אומרים לה במשפט: "קודם אוסיף לדפים הקיימים קובץ מוכן מראש, בשביל סורקים שלא מריצים קוד." ואחרי שהיא מאשרת: שלב א, צעד 2, בענף `feature/seo`, עם הבדיקות של צעדים 9 ו־10. רק אחרי "מיזגתי" ממשיכים לשלב ה.
2. **שלבים ב ו־ג:** הנכס ב־Search Console מאומת? יש ב־`app/public` קובץ מפתח של IndexNow? מה שנעשה, ממשיכים ממנו בצעד 7. מה שעוד לא נעשה יכסה גם את הדפים החדשים כשיגיע תורו: שלב ב שולח את מפת האתר, ושלב ג שולח ל־IndexNow את כל הכתובות שבה.
3. **קוראים מה העסק עושה,** בלי לשאול:
   - קובץ על העסק בתיקיית הפרויקט, בכל שם, למשל "על העסק.txt".
   - `תכנון המערכת.md`: מה שכתוב בו על העסק ועל הלקוחות שלו. רוב הקובץ מתאר את המערכת, ולא את מה שהעסק נותן ללקוחות.
   - סקיל המותג: העסק, הקהל, והמין של שם העסק (כמו בסקיל about-page: "אופק הוא עסק": "אופק עובד").
   - דף האודות: שם העסק, המשפט על העסק, המייל, ובלוק ה־`Organization`.
   - סקיל המערכת (`build-my-system`): כללי המסכים. (את הגרסאות שומרים לפי "ענפים" למעלה.)
4. **כבר רץ פעם?** יש `app/src/content/search-pages.ts`? קוראים אותו, ואומרים לה במשפט אילו דפים כבר קיימים. ב"נוסף שירות" עובדים רק על השירות החדש ("כשנוסף שירות", בסוף השלב).
5. **הכתובות פנויות:** בנתב אין מסך פנימי בכתובת שמתחילה ב־`/services`, ב־`/events` או ב־`/faq`. יש? בוחרים מילה אחרת באנגלית, ואומרים לה במשפט.

### צעד 1: ההצעה, והבחירה שלה

**Claude** מכין רשימה של שלושה עד שישה דפים, כולל דף השאלות. אין בקבצים מספיק כדי להציע? שואלים שאלה אחת: "אילו שירותים העסק נותן? כתבי שורה לכל שירות." ורק אז מציעים.

**מה נכנס לרשימה:**
- **דף לכל שירות אמיתי** שהעסק נותן: כתוב בקבצים, או שהיא אמרה. בעסק של אירועים: דף לכל סוג אירוע (`/events/<שם>`), כמו באתר אירועים שרות בנתה. דף לקהל: רק כשהקהל הזה מקבל באמת שירות אחר, ולא אותו שירות בשם אחר.
- **דף אחד של שאלות נפוצות** (`/faq`), עם שאלות אמיתיות שלקוחות שואלות. שאלות שכתובות בקבצים, או שעולות מהם, מציעים. את השאלות היא בוחרת ומוסיפה, ואת התשובות היא נותנת (צעד 2).

**מה לא נכנס,** גם כשהיא מבקשת "עוד דפים לגוגל". אומרים לה במשפט למה, ומה כן:
- **דף לכל עיר או אזור עם אותו תוכן,** כמו "ייעוץ עסקי בירושלים" ו"ייעוץ עסקי בבני ברק". כך גוגל מתארת דפי מעבר (doorways), שהם הפרה של הכללים שלה נגד ספאם. האזור שבו העסק עובד הוא שורה בדף של השירות. (נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/essentials/spam-policies)
- **שני דפים שההבדל ביניהם רק בשם.** המבחן, מ־programmatic-seo: קוראים את שני הדפים זה ליד זה. אפשר להבדיל ביניהם רק לפי השם? מאחדים לדף אחד.
- **שני דפים שעונים על אותו חיפוש.** הם מתחרים זה בזה (seo-onpage). מאחדים.
- **דף לשירות שאין עליו פרטים משלו.** בלי מה כלול, למי ואיך מתחילים, לדף אין מה לומר. הוא מחכה לפרטים (צעד 2), ולא נבנה ממשפטים כלליים.
- **הרבה דפים "כדי שיהיו".** גוגל שואלת אם אתר מייצר הרבה תוכן על נושאים רבים בתקווה שחלק ממנו יצליח בחיפוש, וכללי הספאם שלה אוסרים דפים בכמויות שנועדו בעיקר לחיפוש ולא לעזור. (נבדק בשני המסמכים שלמעלה, 24.11.2026)

**ההצעה, בטבלה אחת:**

| הדף והכתובת | מה מי שמחפשת רוצה | מה יהיה בדף | למה זה עוזר לגוגל ולמנועי הבינה |
|---|---|---|---|

- **מה מי שמחפשת רוצה:** אחד מארבעת הסוגים של seo-keyword: ללמוד, למצוא את העסק בשמו, להשוות ולבחור, או לפנות ולהזמין. ליד הסוג, חיפוש אחד לדוגמה, במילים שלקוחה הייתה כותבת. את הסוג מסיקים ממה שהעסק עושה, בלי כלי ובלי נתונים על כמות החיפושים, ולכן לא כותבים "הרבה מחפשים".
- **מה יהיה בדף:** כמה מילים לכל חלק, לפי המבנה של צעד 3.
- **למה זה עוזר:** משפט אחד, שנכון לדף הזה. למשל: "הפסקה הראשונה עונה מה השירות, למי הוא ואיך מתחילים, ומנוע בינה יכול לקחת ממנה תשובה שלמה."
- מתחת לטבלה, שורה: "בדף האודות יתווסף חלק 'השירותים', עם קישור לכל דף."
- ושורה לכל דבר שנשאר בחוץ, עם הסיבה במשפט. למשל: "פרויקטים: בקבצים כתובה רק המילה. ספרי לי איזה פרויקטים, ואוסיף דף."

**ההודעה הראשונה של השלב** היא שלוש השורות, הטבלה והשאלה, בהודעה אחת, עם המשפט על השאלות של Claude Code (ראו "איך מדברים איתה"):
1. "בשלב הזה נבנה כמה דפים ציבוריים, שעוזרים למי שמחפשת את מה שהעסק נותן למצוא אותו, בגוגל ובמנועי הבינה."
2. "אני מציע את הדפים מתוך מה שכתוב על העסק. כל פרט שלא כתוב, אשאל אותך. לא ממציאים כלום."
3. "אחר כך אבנה אותם באותו עיצוב, אוסיף אותם למפת האתר ולקובץ של מנועי הבינה, ואבדוק בייצור."

ובסוף ההודעה: "אילו דפים לבנות? אפשר את כולם, רק חלק, או להוסיף שירות שלא הצעתי." התשובה שלה היא הבחירה, וגם האישור לשלב. זו ההחלטה שמחכים לה לפני הבנייה. את הטקסט של הדפים היא מאשרת אחרי שהם נבנו, במחשב, לפני שהם נשמרים ועולים לייצור (צעד 5, סעיף 4). השאלות של צעד 2 הן שאלות על פרטים, לא אישור.

### צעד 2: הפרטים שחסרים

לכל דף שהיא בחרה, **Claude** בודק מה כבר כתוב בקבצים, ושואל רק על מה שחסר. שאלה אחת בכל פעם. מה שכבר כתוב, אומרים ושואלים "נכון?", כמו בכל הסקיל.

1. **לכל שירות, שאלה פתוחה אחת:** "ספרי לי במילים שלך על <השירות>: מה כלול בו, למי הוא מתאים, איך הוא עובד, ואיך מתחילים." מה שחסר אחרי התשובה, ונחוץ לדף, שואלים אחר כך, בשאלה נפרדת.
2. **מה שהדף צריך כדי להיבנות:** מה כלול, למי, ואיך מתחילים. חסר אחד מהם? הדף הזה מחכה, ושאר הדפים ממשיכים.
3. **פרטים שנכנסים רק אם היא אמרה אותם:** מחיר, משך, אזור, פנים אל פנים או מרחוק, כשרות, שנות ניסיון, מספרים. שואלים עליהם פעם אחת, ביחד: "רוצה שיופיעו גם מחיר, משך או אזור? לא חובה." לא כתוב ולא נאמר? לא נכנס. אין משפט כללי במקום פרט, ואין "בקרוב".
4. **השאלות הנפוצות:** "אילו שאלות לקוחות שואלות אותך הכי הרבה?", וליד השאלה, השאלות שעלו מהקבצים, אם יש. חמש עד שמונה שאלות. את התשובה לכל שאלה היא נותנת במילים שלה. **Claude** מסדר אותה כך שהמשפט הראשון עונה, ולא מוסיף לה שום עובדה.
5. **היא לא יודעת?** למשל, כשהיא בונה את המערכת לעסק של מישהי אחרת: **Claude** כותב לה רשימה של השאלות הפתוחות, לשלוח לבעלת העסק במייל. הדפים שיש להם כל מה שהם צריכים נבנים עכשיו. וכשמגיעות התשובות: «כתבי לי: "יש תשובות מבעלת העסק".»

(באתר אירועים שרות בנתה, חלק מהטקסט נכתב בהתחלה כהערכה, עם הערה לבדוק מול הלקוחה: יתרונות, סיפור, מספרים ושעות פתיחה. אחר כך הכול תוקן מול הלקוחה. לכן כאן לא כותבים הערכה בכלל.)

### צעד 3: בונים את הדפים

**1. קובץ התוכן.** כל הטקסט של הדפים בקובץ אחד, עם טיפוסים: `app/src/content/search-pages.ts`. ממנו נבנים הדפים, הכותרות והנתונים המובנים, ולפיו נכתבים מפת האתר ו־`llms.txt` (צעד 4).

```ts
// דפים שעוזרים לחיפוש (הסקיל seo, שלב ה).
// כל הטקסט כאן מהקבצים של העסק ומהתשובות של בעלת העסק. לא מוסיפים פרט שלא נאמר.
// כשמשנים דף: מעדכנים את updated, את public/sitemap.xml ואת public/llms.txt, באותן מילים.
export type ServicePage = {
  slug: string          // באנגלית: אותיות a עד z, ספרות ומקפים. למשל 'monthly-support'
  name: string          // שם השירות: הכותרת הראשית בדף
  title: string         // השם בלשונית: '<שם השירות> | <שם העסק>'
  description: string   // התיאור לגוגל: משפט אחד, מתוך answer
  answer: string        // הפסקה הראשונה: מה השירות, למי, ואיך מתחילים
  sections: { heading: string; text?: string; items?: string[] }[] // רק חלקים שיש להם תוכן
  updated: string       // YYYY-MM-DD: היום שבו התוכן של הדף השתנה בפעם האחרונה
}

export type FaqItem = { question: string; answer: string }

export const SERVICE_PAGES: ServicePage[] = []
export const FAQ_ITEMS: FaqItem[] = []
export const FAQ_UPDATED = 'YYYY-MM-DD'
export const FAQ_TITLE = 'שאלות נפוצות | <שם העסק>' // השם בלשונית
export const FAQ_DESCRIPTION = '' // התיאור לגוגל: משפט אחד, מתוך משפט הפתיחה של הדף
```

- את הטקסט משנים בבקשה ל־Claude. אומרים לה את זה במשפט: «כדי לשנות טקסט, כתבי לי, למשל: "תוסיף לשאלות הנפוצות שאלה על..."». ועוד משפט: "מסך ניהול, שבו בעלת העסק משנה את הטקסט לבד, מחכה לכניסה ולהרשאות, במפגש הבא." (באתר האירועים שרות בנתה, השאלות נשמרות בטבלה במסד, עם מסך ניהול, ודפי האירועים עברו לשם אחר כך.)

**2. תבנית אחת לכל דפי השירות,** `app/src/pages/ServicePage.tsx`, ודף השאלות, `app/src/pages/FaqPage.tsx`. כמו באתר האירועים שרות בנתה, שבו שלושת דפי האירועים נבנו מאותה תבנית.
- **אותו מראה כמו דף האודות:** הגופן והצבעים לפי סקיל המותג, ולפי כללי המסכים בסקיל המערכת. אותה מסגרת של הדפים הציבוריים, בלי התפריט של המסכים הפנימיים.
- **בדף שירות:**
  1. כותרת ראשית אחת: שם השירות.
  2. מיד אחריה, הפסקה הראשונה (`answer`): משפט או שניים שעונים מה השירות, למי הוא ואיך מתחילים. בלי "ברוכים הבאים" ובלי הקדמה. (seo-aeo-geo ו־programmatic-seo: התשובה בראש הדף, כי ממנה גוגל ומנועי הבינה לוקחים.)
  3. כותרות משנה, בניסוח של שאלה כשזה טבעי: "מה כלול?", "למי זה מתאים?", "איך זה עובד?". מתחת לכל אחת, המשפט הראשון עונה. מה שיש בו כמה פריטים, ברשימה.
  4. חלק שאין לו תוכן לא מופיע. בלי כותרת ריקה.
  5. "איך מתחילים": המייל מדף האודות, כקישור (`mailto:`), או טופס, אם יש במערכת טופס ציבורי.
  6. קישורים לדפי השירות האחרים, לשאלות הנפוצות ולדף האודות, במילים שאומרות לאן מגיעים, ולא "לחצי כאן".
- **בדף השאלות:** כותרת ראשית "שאלות נפוצות", משפט פתיחה אחד, ואחריו כל שאלה ככותרת משנה, עם התשובה מתחתיה. **כל התשובות גלויות בדף,** בלי לפתוח ולסגור. בתשובה שמזכירה שירות, קישור לדף שלו. (גוגל: לא מסמנים בנתונים מובנים תוכן שלא רואים בדף. נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/appearance/structured-data/sd-policies)
- **בכתובת עם שתי רמות** (`/services/<slug>`), כל קישור, תמונה ולוגו כתובים מ־`/`: `/logo.png`, `/faq`. כתובת כמו `logo.png`, בלי `/`, לא תיטען שם.
- עברית, מימין לשמאל, ובקוד רק כיוונים לוגיים. מספרים, מיילים ואותיות לטיניות בתוך טקסט עברי נכנסים לתוך `<bdi>`, כמו בדף האודות. כותרת ראשית אחת, כותרות משנה בסדר, וטקסט חלופי לכל תמונה.
- פועל או תואר על העסק לפי המין של שם העסק בסקיל המותג, כמו בסקיל about-page.

**3. הכתובות: ברשימה של הדפים הציבוריים.** לא בנתב. הדפים החדשים נכנסים ל־`PUBLIC_PAGES` שב־`app/src/public-pages.tsx` (שלב א, צעד 2), אחרי הדפים שכבר שם. משם הם מקבלים כתובת בנתב, ברמה העליונה ולפני כל בדיקת כניסה, שם ותיאור, וקובץ מוכן מראש. כתובת אחת לכל דף שבקובץ התוכן, ולא כתובת אחת שמקבלת כל שם:

```tsx
{SERVICE_PAGES.map((page) => (
  <Route key={page.slug} path={`/services/${page.slug}`} element={<ServicePage page={page} />} />
))}
<Route path="/faq" element={<FaqPage />} />
```

- **אין נתב** (כמו במערכת הדמו של הקורס)? כמו בסקיל about-page: ברכיב העליון (בדרך כלל `app/src/App.tsx`), לפני בדיקת הכניסה, בודקים את `window.location.pathname`. `/faq` מציג את דף השאלות, ו־`/services/<slug>` של דף שבקובץ מציג את הדף שלו. כל כתובת אחרת ממשיכה למסכים הפנימיים.
- **`slug`:** באנגלית, אותיות a עד z, ספרות ומקפים. בלי אותיות גדולות, בלי נקודה, ובלי `/` בסוף. (seo-onpage: כתובת קצרה, באותיות רגילות, עם מקפים בין המילים.) כך הכתובת נכנסת לכלל של "לא לחיפוש" בלי שום שינוי בצורה שלו (צעד 4).
- בעסק של אירועים, `/events/<slug>` במקום `/services/<slug>`. לכל הדפים של השלב אותה מילה.
- לא בשום תפריט של המסכים הפנימיים. מגיעים אליהם מדף האודות, מהדפים עצמם, ומהחיפוש.

**4. כותרת ותיאור בכל דף,** באותה דרך כמו בשלב א, צעד 2: השם והתיאור נכתבים ברשימה, מקובץ התוכן (`page.title` ו־`page.description`, ובדף השאלות `FAQ_TITLE` ו־`FAQ_DESCRIPTION`). הבנייה מראש כותבת אותם בקובץ של הדף, ו־`PublicPageMeta` כותב אותם כשעוברים לדף בלי לטעון מחדש. הדף עצמו לא כותב שום דבר ב־head: לא `<title>` או `<meta>` ב־JSX, ולא `document.title`. לא מוסיפים ספרייה.
- **הכותרת:** `<שם השירות> | <שם העסק>`, ובדף השאלות `שאלות נפוצות | <שם העסק>`. כאן שם העסק ולא שם המערכת, כי מי שמחפשת שירות מחפשת את העסק. (כך גם באתר האירועים שרות בנתה.)
- **התיאור:** משפט אחד, מתוך הפסקה הראשונה של הדף.
- לכל דף כותרת ותיאור משלו, שונים מכל דף אחר באתר. (גוגל, כמו בשלב א, צעד 1: https://developers.google.com/search/docs/appearance/title-link ו־https://developers.google.com/search/docs/appearance/snippet)

**5. נתונים מובנים,** בתוך הדף, באותה צורה כמו בלוק ה־`Organization` בדף האודות (`<script type="application/ld+json">`). הבלוק נבנה מאותו קובץ תוכן שממנו נבנה הדף, וכך מה שכתוב בו זהה למה שרואים. (כך גם באתר האירועים שרות בנתה: בלוק השאלות נבנה מאותן שאלות שבדף.) גוגל קוראת בלוק כזה גם כשהקוד בדפדפן כותב אותו. (נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/appearance/structured-data/generate-structured-data-with-javascript) ועם הבנייה מראש, הבלוק כבר בקוד שחוזר מהכתובת, גם בשביל סורק שלא מריץ קוד. (נבדק ב־24.11.2026 באתר חי, בפרויקט בדיקה: בלוק `Service` בדף `/services/consulting`.)

בדף שירות, `Service`:

```json
{
  "@context": "https://schema.org",
  "@type": "Service",
  "name": "<שם השירות>",
  "description": "<התיאור>",
  "url": "https://<הדומיין>/services/<slug>",
  "provider": {
    "@type": "Organization",
    "name": "<שם העסק, כמו ב־Organization של דף האודות>",
    "url": "<הכתובת, כמו ב־Organization של דף האודות>"
  }
}
```

- `areaServed` (האזור) ו־`audience` (למי), רק אם היא אמרה אותם, ובאותן מילים כמו בדף. בלי מחיר, פרטי קשר או שעות שלא כתובים בדף.
- **מה זה נותן, בכנות:** `Service` מוגדר ב־schema.org ("שירות שארגון נותן"), אבל הוא לא ברשימה של הנתונים המובנים שמהם גוגל בונה תוצאה מיוחדת בחיפוש. (נבדק ב־24.11.2026: https://schema.org/Service, גרסה 30.1, ו־https://developers.google.com/search/docs/appearance/structured-data/search-gallery.) הוא מתאר את השירות בצורה מסודרת למנועים שקוראים schema.org (seo-aeo-geo, ai-seo). איזה מנוע משתמש בו בפועל: לא נבדק במסמך רשמי.

בדף השאלות, `FAQPage`:

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "<השאלה, כמו בדף>",
      "acceptedAnswer": { "@type": "Answer", "text": "<התשובה, כמו בדף>" }
    }
  ]
}
```

- **מה זה נותן, בכנות:** גוגל כבר לא מציגה שאלות ותשובות מתחת לתוצאה בחיפוש, לאף אתר, מאז 7.5.2026, ואת המסמך על זה הורידה ב־15.6.2026. מ־2023 עד אז היא הציגה אותן רק לאתרים מוכרים של ממשלה ובריאות. (נבדק ב־24.11.2026: https://developers.google.com/search/updates, ושם מגיעים גם מהכתובת של המסמך הישן, https://developers.google.com/search/docs/appearance/structured-data/faqpage. ועל 2023: https://developers.google.com/search/blog/2023/08/howto-faq-changes.) לכן לא אומרים לה שהשאלות יופיעו בגוגל מתחת לתוצאה.
- הבלוק נשאר, כי הוא מתאר את השאלות שבדף לפי schema.org. לגוגל הוא לא מזיק: לפי הבלוג של גוגל (8.8.2023, אותה כתובת), נתונים מובנים שלא בשימוש לא גורמים לבעיות בחיפוש, וגם לא משנים בו שום דבר שרואים. לפי ai-seo ו־seo-aeo-geo, מנועי בינה שאינם גוגל קוראים בלוק כזה. זה לא נבדק במסמך רשמי.
- מה שבאמת עוזר בדף הזה הוא הטקסט: שאלה אמיתית, ותשובה שהמשפט הראשון שלה עונה.
- גוגל כותבת שלתשובות הבינה בחיפוש שלה לא צריך סימון מיוחד, קובץ מיוחד או נתונים מובנים מיוחדים. מה שהיא מבקשת: תוכן מועיל בטקסט, שמגיעים אליו בקישורים בתוך האתר, ונתונים מובנים שתואמים למה שכתוב בדף. (נבדק במסמכים הרשמיים, 24.11.2026: https://developers.google.com/search/docs/appearance/ai-features ו־https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)

**6. קישורים מדף האודות.** בדף האודות נוסף חלק אחד, "השירותים", עם קישור לכל דף שירות ולשאלות הנפוצות, לפני יצירת הקשר. זה השינוי היחיד בדף האודות: שאר הטקסט, התגיות ב־`app/index.html` ובלוק ה־`Organization` לא משתנים. היא אישרה אותו בצעד 1. (קישורים רגילים בתוך האתר, שמגיעים בהם לכל דף: המסמך של גוגל על AI שלמעלה, ו־pillar-content-architecture, שבו אין דף שאף דף לא מפנה אליו.)

### צעד 4: מוסיפים את הדפים לכלל, למפת האתר ול־llms.txt

הדפים החדשים הם דפים ציבוריים לכל דבר, ולכן הם נכנסים לשלושת המקומות של שלב א.

**1. `app/vercel.json`, הרשימה שבכלל.** כל כתובת חדשה נכנסת לסוגריים הראשונים, בשמה המלא, עם `$` אחריה, בדיוק כמו `about$`. שאר הכלל לא משתנה. למשל, עם שני דפי שירות ודף שאלות:

```json
"source": "/((?!about$|privacy$|terms$|accessibility$|faq$|services/consulting$|services/monthly-support$)(?!google[0-9a-f]+\\.html$)(?!.*\\.(?:txt|xml|png|jpe?g|svg|ico|webp|js|css|woff2?|map|webmanifest)$).*)"
```

- כל כתובת בלי ה־`/` שבתחילתה, ועם ה־`/` שבאמצע: `services/consulting$`. באותיות בדיוק כמו בנתב.
- **`$` אחרי כל כתובת, תמיד.** בלעדיו, גם כתובות שרק מתחילות כמוה יוצאות מהסימון, ומחזירות את המערכת בלי "לא לחיפוש".
- **בלי סוגריים חדשים.** לא מקצרים ל־`services/(consulting|monthly-support)$`: סוגריים כאלה בתוך הכלל לא עוברים.
- **לא מוציאים את כל `services/` בבת אחת.** אז כל כתובת שמתחילה כך, גם שם שאין מאחוריו דף, תחזיר את המערכת בלי הסימון.
- (נבדק ב־24.11.2026, במחשב ולא באתר חי: בספרייה path-to-regexp 6.1.0, עם ההגדרות שבהן Vercel קורא את הכלל, `strict`, `sensitive` ו־`delimiter: "/"`, כמו שהן כתובות בגרסה 54.13.0 של Vercel CLI. זו לא אותה בדיקה כמו בשלב א, צעד 8, ב־`@vercel/routing-utils` 5.3.3. עם הכלל שלמעלה יצאו מהסימון `/faq`, `/services/consulting` ו־`/services/monthly-support`, יחד עם הדפים הציבוריים והקבצים, וסומנו `/`, `/customers`, `/faq/`, `/FAQ`, `/faq-old`, `/faqs`, `/services`, `/services/`, `/services/other`, `/services/consulting/`, `/services/consulting-x` ו־`/services/consulting.html`. בלי `$` יצאו מהסימון גם `/faq-old`, `/faqs`, `/services/consulting-x` ו־`/services/consulting.html`. וסוגריים כמו `(services)` החזירו שגיאה. באתר שלה את הכלל בודקים בייצור, בצעד 6, וזה תנאי להמשך.)
- (נבדק גם באתר חי, 24.11.2026, בפרויקט בדיקה נפרד, עם דף שירות אחד ובלי דף שאלות: עם `services/consulting$` ברשימה שבכלל, `/services/consulting` חזר בלי `X-Robots-Tag`, ו־`/services`, `/services/` ו־`/services/test-xyz` חזרו עם `X-Robots-Tag: noindex, nofollow`. שאר הכתובות שלמעלה, ו־`/faq`, נבדקו רק במחשב.)

**2. `app/public/sitemap.xml`.** שורה לכל דף חדש, באותה צורה כמו בשלב א, צעד 5, וה־`lastmod` מה־`updated` של הדף (בדף השאלות, `FAQ_UPDATED`). גם `/about` מקבל את התאריך של היום, כי נוספו בו קישורים. (גוגל: `lastmod` הוא התאריך של השינוי המשמעותי האחרון, כמו שינוי בתוכן, בנתונים המובנים או בקישורים. נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap)

**3. `app/public/llms.txt`.** הדפים בנויים מראש (שלב א, צעד 2), ולכן גם סורק שלא מריץ קוד קורא את הטקסט שלהם. `llms.txt` מרכז את עיקר הטקסט במקום אחד, בשביל מנועים שקוראים אותו: אחרי "אודות" ולפני "יצירת קשר" נוספים שני חלקים:

```
## שירותים

- [<שם השירות>](https://<הדומיין>/services/<slug>): <הפסקה הראשונה של הדף, מילה במילה>

## שאלות נפוצות

- [<השאלה>](https://<הדומיין>/faq): <התשובה, מילה במילה כמו בדף>
```

- **מילה במילה מקובץ התוכן.** אותו טקסט כמו בדף, בלי ניסוח חדש ובלי פרט נוסף.
- **כל שאלה בשורה, ולא ככותרת.** לפי llmstxt.org, אחרי הכותרת הראשית יש בקובץ רק כותרות `##`, ומתחת לכל אחת רשימה של קישורים, כל קישור עם הערה אחרי `:`. לכן כל שאלה היא קישור לדף השאלות, והתשובה היא ההערה שלו. (הפורמט נבדק ב־https://llmstxt.org, 24.11.2026.)
- **הכלל של שלב א, צעד 6,** "רק מה שכתוב בדף האודות", מתרחב לכל הדפים הציבוריים: רק מה שכתוב בהם. מחיר נכנס רק אם הוא כתוב בדף השירות. מסכים פנימיים ומידע מתוך המערכת: אף פעם.
- **מה זה נותן, בכנות:** גוגל כותבת שקובץ כזה לא יזיק ולא יעזור להופעה בחיפוש שלה, כי החיפוש שלה מתעלם ממנו ("as Google Search ignores them"). (נבדק במסמך הרשמי, 24.11.2026: https://developers.google.com/search/docs/fundamentals/ai-optimization-guide.) לגוגל עוזרים הדפים עצמם. הקובץ בשביל מנועי בינה אחרים, ורק אם הם קוראים אותו (שלב א, "הדפים הציבוריים בנויים מראש").

### צעד 5: בדיקה במחשב, ושמירה

1. **הכתובות זהות בחמישה מקומות.** **Claude** משווה את הדפים שבקובץ התוכן ל־`PUBLIC_PAGES` (`app/src/public-pages.tsx`, וממנו הנתב והבנייה מראש), לרשימה שבכלל, למפת האתר ול־`llms.txt`. כל כתובת מופיעה בכולם, באותן אותיות. והטקסט ב־`llms.txt` זהה לטקסט שבקובץ התוכן, מילה במילה.
2. **כמו בשלב א, צעד 9:** אין שגיאות טיפוסים, והבנייה עוברת. בשורה `prerendered` בסוף הבנייה מופיעה כל כתובת חדשה, ולכל אחת יש קובץ: `app/dist/services/<slug>/index.html`, ו־`app/dist/faq/index.html`. בכל קובץ, הבדיקות של שלב א, צעד 2, סעיף 6.2: הטקסט של הדף, השם, התיאור, `canonical`, ובלוק ה־`Service` או ה־`FAQPage`, עם אותו טקסט כמו בדף. דף חדש מפיל את הבנייה? שלב א, צעד 2, סעיף 5.
3. **מריצים את המערכת במחשב, ובודקים ב־Playwright** כל דף חדש:
   - ב־`vite preview` הקובץ המוכן נפתח בכתובת עם `/` בסוף, כמו `/services/<slug>/` (שלב א, צעד 2, סעיף 6.4). ב־console אין שגיאות ואין אזהרות.
   - הטקסט שלו, ולא מסך פנימי. גם בכתובת עם שתי רמות, העיצוב, הלוגו והתמונות נטענים.
   - ב־head בדיוק `<title>` אחד ובדיוק `meta[name="description"]` אחד, עם הטקסט של הדף הזה. ואחרי שעוברים ממנו למסך פנימי, חוזרים אלה של `app/index.html`.
   - בלוק הנתונים המובנים: JSON תקין, עם אותו טקסט כמו בדף.
   - כל קישור נפתח, וכל דף חדש מקושר מדף האודות.
   - בשלושה רוחבים, צר, בינוני ורחב: בלי גלילה הצידה, והטקסט קריא.
   - אין בדף "בקרוב", טקסט לדוגמה או חלק ריק.
4. **מראים לה לאישור, לפני שמשהו נשמר.** הדפים עוד לא עלו, ושום דבר עוד לא נשלח לגוגל. **Claude** מריץ את המערכת במחשב, פותח לה ב־Playwright את הדף הראשון, וכותב: «הדפים מוכנים במחשב, ועוד לא עלו לייצור. קראי כל דף: <רשימת הכתובות במחשב>. משהו לא מדויק? כתבי לי מה, ואתקן. הכול נכון? כתבי: "מאשרת".» ומחכים.
   - **היא מתקנת?** מתקנים בקובץ התוכן, וב־`llms.txt` באותן מילים, בודקים שוב את סעיפים 1 עד 3, ומראים לה שוב את הדף שהשתנה. ושוב מחכים ל"מאשרת".
   - **היא בונה את המערכת לעסק של מישהי אחרת?** אומרים לה במשפט שכדאי לשלוח קודם את הטקסט לבעלת העסק, ולכתוב "מאשרת" אחרי שהיא אישרה.
   - רק אחרי "מאשרת" ממשיכים לסעיף 5.
5. **שומרים גרסה, לפי "ענפים" למעלה,** בענף `feature/search-pages`: מוסיפים לגרסה את כל הקבצים של השלב, ורק אותם, לפי השם: קובץ התוכן, התבנית, דף השאלות, `app/src/public-pages.tsx`, דף האודות, `app/vercel.json`, `app/public/sitemap.xml` ו־`app/public/llms.txt`. `App.tsx` לא משתנה בשלב הזה, ו־`app/dist` לא נכנס לגרסה. יש `CHANGELOG.md`? באותה גרסה מוסיפים תחת `[Unreleased]` ← `### נוסף` את השורה "נוספו דפים לשירותים של העסק ודף שאלות נפוצות, שעוזרים למצוא את העסק בגוגל ובמנועי הבינה" (השורה כבר שם? לא מוסיפים שוב. אין קובץ? לא יוצרים). בודקים ב־`git status` שלא נשאר בחוץ קובץ של השלב. `.env`, התיקייה "בדיקות" ו־`.playwright-mcp` לא נכנסים. דוחפים, ונותנים לה קישור ל־Pull Request, עם כותרת ותיאור בעברית. היא ממזגת בעצמה, ב־GitHub. **הבדיקה בייצור, מפת האתר ו־IndexNow מחכים עד שהיא כותבת "מיזגתי".**

### צעד 6: בודקים בייצור, ורק אז ממשיכים

כמו בשלב א, צעד 10, בכתובת הקצרה, אחרי שהגרסה החדשה עלתה.

1. **כל דף חדש, ב־Playwright, בחלון שלא מחובר למערכת:** נפתח עם הטקסט שלו ועם הכותרת שלו בלשונית, בלי מסך כניסה, וב־head שלו כותרת אחת ותיאור אחד.
2. **הכותרות (headers) של התשובה:**
   - כל דף חדש: 200, **בלי `X-Robots-Tag`**, ובלי תגית `robots` או `googlebot` עם noindex בקוד שחוזר.
   - ממשיכים לקבל `X-Robots-Tag: noindex, nofollow`: `/`, `/index.html`, מסך פנימי, וגם `/faq/`, `/services`, ושם של שירות שאין לו דף, כמו `/services/test-xyz`.
   - **הקוד שחוזר, לפני שהוא רץ:** **Claude** מוריד כל דף חדש בלי דפדפן (`curl -s`), ובודק שיש בו הטקסט של הדף, השם, התיאור, `canonical` לכתובת שלו, ובלוק ה־`Service` או ה־`FAQPage` (שלב א, צעד 2, סעיף 7). ב־`/services/test-xyz`, לעומת זאת, `<div id="root"></div>` ריק.
   - (נבדק ב־24.11.2026 באתר חי, בפרויקט בדיקה, עם דף שירות אחד: `/services/consulting` חזר 200 בלי `X-Robots-Tag`, עם הטקסט ובלוק ה־`Service` בקוד שחזר. `/services`, `/services/` ו־`/services/test-xyz` חזרו 200 עם `X-Robots-Tag` ו־`#root` ריק.)
   - הדפים הציבוריים הקודמים והקבצים: כמו בשלב א, צעד 10.
3. **`/sitemap.xml` ו־`/llms.txt`:** חזר התוכן החדש, בסוג הנכון, וב־`llms.txt` עם `charset=utf-8`.
4. **אין סוד בקוד של האתר:** אותה בדיקה כמו בשלב א, צעד 10, סעיף 5. הדפים החדשים הוסיפו קוד, ולכן בודקים שוב.
5. **משהו לא עבר:** עוצרים, כמו בשלב א, צעד 10, סעיף 6.
   - **דף חדש עם `X-Robots-Tag`** הוא הדחוף: בדרך כלל הכתובת חסרה ברשימה שבכלל, כתובה שם אחרת מבנתב, או בלי `$`. מתקנים, מעלים, ובודקים שוב.
   - **`/services/test-xyz` בלי `X-Robots-Tag`:** בכלל יצאו כל הכתובות שמתחילות ב־`services/`, או שחסר `$`. מתקנים לפי צעד 4.
   - **מסך פנימי שאיבד את הסימון:** "הסימון של המסכים הפנימיים לא עבד אצלך. זה לא משהו שעשית לא נכון. נעצור כאן, ורות תבדוק."

ואז אומרים לה: "הדפים החדשים בייצור. אפשר לקרוא אותם: פתחי את <הדומיין>/<דף>. משהו לא מדויק? כתבי לי מה, ואתקן." (`<דף>`: אחד הדפים החדשים, למשל `faq`, אם היא בחרה בו.)
- **היא מתקנת?** **Claude** משנה את קובץ התוכן, ואת `llms.txt` באותן מילים, מעדכן את `updated` ואת התאריך במפת האתר, מראה לה במחשב את הדף שהשתנה ומחכה ל"מאשרת" (צעד 5, סעיף 4), ושומר בענף `fix/search-pages`, עם Pull Request. אחרי "מיזגתי" בודק שוב (צעדים 5 ו־6). ל־IndexNow שולחים רק את הכתובות שהשתנו.

### צעד 7: גוגל, Bing ומנועים נוספים

1. **Search Console** (רק אם הנכס כבר מאומת, משלב ב): **Claude** נכנס בחשבון שלה, כמו בשלב ב, צעד 1, ופותח את **Sitemaps** של הנכס, כמו בשלב ב, צעד 5. שם הוא שולח שוב את `sitemap.xml`: כותב אותו בתיבה **הוספת sitemap חדש**, ולוחץ **שלח**. אומרים לה מה כתוב במסך, כמו שהוא כתוב, ובמשפט: "גוגל קיבלה שוב את מפת האתר, עם הדפים החדשים. זה עוד לא אומר שהם כבר בחיפוש."
   - (גוגל: אחרי שינוי גדול במפת האתר, אפשר לשלוח אותה שוב. בשינויים קלים, גוגל חוזרת אליה לבד, בקצב משלה. נבדק במסמך הרשמי, 24.11.2026: https://support.google.com/webmasters/answer/7451001. שליחה חוזרת של מפת אתר שכבר נשלחה, ומה כתוב במסך אחריה: לא נבדק עדיין בהרצה.)
   - לא מבקשים להוסיף את הדפים החדשים אחד אחד. הם מגיעים לגוגל ממפת האתר, כמו בשלב ב, צעד 6, סעיף 5.
2. **IndexNow** (רק אם יש קובץ מפתח, משלב א, צעד 7): **Claude** שולח בקשה אחת, כמו בשלב ג, צעד 2, וב־`urlList` רק הכתובות החדשות ו־`/about`, שהשתנה. לא שולחים שוב כתובות שלא השתנו. ל־Bing כבר יש את מפת האתר, מהייבוא בשלב ג.
3. **שלב ב או שלב ג עוד לא נעשו?** לא עושים אותם כאן. כשיגיע תורם, הם יכסו גם את הדפים החדשים.

### בסוף השלב

1. **אומרים לה בשלוש שורות:**
   1. "נבנו <המספר> דפים חדשים: <שמות הדפים>. בדף האודות יש עכשיו קישור לכל אחד."
   2. "הם במפת האתר ובקובץ של מנועי הבינה, וגוגל, Bing ומנועים נוספים קיבלו עליהם הודעה." שלב ב או ג עוד לא נעשה? במקום החלק שלו: "גוגל תקבל אותם כשנרשום את האתר בה", או "Bing יקבל אותם כשנגיע אליו".
   3. "גוגל מוסיפה דפים לאט, ומקום בחיפוש לא מובטח. כדי לשנות טקסט, כתבי לי."
   - דף שמחכה לפרטים (צעד 2)? שורה רביעית: «הדף על <השירות> מחכה ל<מה שחסר>. כשיש תשובה, כתבי לי: "יש תשובות מבעלת העסק".»
2. **סקיל המערכת:** לא כותבים ב־`build-my-system` ולא מציעים לכתוב בו. בקורס הזה כל תלמידה מוסיפה לו את הכללים בעצמה, בבקשה מדף הפרומפטים של המפגש.

### כשנוסף שירות, או כששירות כבר לא ניתן

כשהיא כותבת "נוסף שירות", או מבקשת דף לשירות אחד:
1. בודקים רק את השירות הזה, מול המבחנים של צעד 1: הוא שירות אמיתי, יש לו פרטים משלו, והוא לא עונה על אותו חיפוש כמו דף שכבר קיים. דומה מדי לדף קיים? מציעים להוסיף אותו לדף הקיים, ומחכים לתשובה.
2. שואלים את הפרטים החסרים (צעד 2), ובונים: רשומה חדשה בקובץ התוכן, וקישור אליה בדף האודות ובדפי השירות האחרים (צעד 3). הרשומה נכנסת לבד לרשימה של הדפים הציבוריים, לנתב ולבנייה מראש, דרך `SERVICE_PAGES`.
3. מוסיפים את הכתובת לרשימה שבכלל, למפת האתר ול־`llms.txt` (צעד 4), בודקים ושומרים (צעד 5), ובודקים בייצור (צעד 6).
4. שולחים ל־IndexNow את הכתובת החדשה, ואת הדפים שנוסף בהם קישור. את מפת האתר לא שולחים שוב: דף אחד הוא שינוי קל, וגוגל תחזור אליה לבד (צעד 7, סעיף 1).
5. שאלה חדשה לשאלות הנפוצות: אותה דרך, בלי כתובת חדשה ובלי שינוי בכלל.

**שירות שכבר לא ניתן:** מורידים את הדף, באותה גרסה, מקובץ התוכן (ומשם הוא יוצא לבד מהנתב ומהבנייה מראש: הקובץ המוכן שלו לא נבנה יותר), מהרשימה שבכלל, ממפת האתר, מ־`llms.txt` ומהקישורים. מאותו רגע הכתובת שלו מחזירה את המערכת, עם "לא לחיפוש", וגוגל תוריד אותה מהחיפוש אחרי שתסרוק אותה שוב. (noindex מוציא דף מהחיפוש אחרי הסריקה הבאה: https://developers.google.com/search/docs/crawling-indexing/block-indexing. בקשה להסרה מהירה ב־Search Console לא בסקיל הזה.)

## כשמשהו נכשל

| מה רואים | מה זה, ומה עושים |
|---|---|
| דף ציבורי מחזיר 404 באינטרנט | "לפני שמתחילים", סעיף 3: `vercel.json` עם `rewrites`, הגרסה עלתה, הבנייה ב־Vercel. לא מפעילים שוב את הסקיל שבנה את הדף |
| `/robots.txt`, `/sitemap.xml` או `/llms.txt` מחזירים את המערכת (`text/html`) | הקובץ לא בתיקייה `public` של התיקייה ש־Vercel בונה ממנה, או שהגרסה עוד לא עלתה. Vercel מגיש קובץ קיים לפני כלל ה־`rewrites` |
| `llms.txt` נראה בדפדפן כמו קוד: משמאל לימין, עם `#` וקישורים | זה תקין. הדפדפן מציג כך כל קובץ טקסט. אומרים לה: "הקובץ נכתב בשביל מנועי הבינה, ולכן בדפדפן הוא נראה כמו קוד. זה תקין." |
| באינטרנט, האותיות ב־`llms.txt` שבורות: סימנים במקום עברית | בודקים ש־`app/public/llms.txt` שמור כ־UTF-8, ואיזה `charset` חוזר בתשובה (שלב א, צעד 10). במחשב, לפני שהקובץ עלה, זה צפוי, ולא מתקנים (שלב א, צעד 9) |
| ב־head של דף ציבורי שתי כותרות או שני תיאורים | הדף כותב `<title>` או `<meta>` ב־JSX, או שספרייה הוסיפה תגית ליד אלה של `app/index.html`. שלב א, צעד 2 |
| `npm run build` נעצר ב־`prerender failed:` | דף ציבורי, או קובץ שהוא מייבא, נוגע בדפדפן, בנתונים של המערכת או בהגדרה שחסרה, או שהרשימה לא תואמת ל־`app/index.html`. ההודעה מראה את הקובץ ואת השורה. שלב א, צעד 2, סעיף 5 |
| בייצור, בקוד שחוזר מדף ציבורי `#root` ריק | Vercel לא מריץ את `npm run build`, הגרסה עוד לא עלתה, או ש־`cleanUrls` נכנס ל־`vercel.json`. שלב א, צעד 2, סעיף 7.5 |
| מסך פנימי מחזיר 404 בכניסה ישירה, ובמחשב הוא נפתח | `cleanUrls` ב־`vercel.json` שובר את הכלל של `rewrites`. מורידים אותו (שלב א, צעד 2, סעיף 4.5), בענף `fix/seo`, מעלים לפי "ענפים", ואחרי "מיזגתי" בודקים שוב |
| דף ציבורי עם `X-Robots-Tag`, או עם תגית noindex בקוד | הדף חסר ברשימה שבכלל, כתוב בה אחרת, כלל ישן חל עליו, או שב־`app/index.html` נשארה תגית noindex. מתקנים לפני כל דבר אחר |
| מסך פנימי, או `/index.html`, בלי `X-Robots-Tag` | בודקים ש־`vercel.json` בתיקייה ש־Vercel בונה ממנה, שהכלל בו כמו בשלב א, צעד 8, ושהגרסה עלתה. עדיין בלי? עוצרים, ורות תבדוק (שלב א, צעד 10) |
| קובץ אמיתי, כמו תמונה או קובץ קוד, עם `X-Robots-Tag` | הסיומת שלו חסרה ברשימת הסיומות שבכלל. מוסיפים אותה, חוץ מ־`html` (שלב א, צעד 8), בענף `fix/seo`, מעלים לפי "ענפים", ואחרי "מיזגתי" בודקים שוב |
| דף ציבורי חדש חסר ב־`PUBLIC_PAGES`, ברשימה שבכלל או במפת האתר | "לפני שמתחילים", סעיף 5: הרשימה מול הנתב |
| Search Console מראה דף הסבר עם כפתור התחלה (**קדימה, מתחילים**), ולא מסך כניסה | זה קורה גם כשהיא מחוברת, למשל כשבחלון כמה חשבונות. קודם בודקים את החשבונות לפי `/u/<n>/`, ולוחצים על הכפתור רק כשהחשבון שלה לא מחובר (שלב ב, צעד 1) |
| **אמת** (Verify) נכשל | הקובץ לא בייצור (חזר דף המערכת), הכתובת של הנכס לא מדויקת (`https`, הכתובת הקצרה, `/` בסוף), או שהנכס נפתח על כתובת ארוכה של Vercel. מתקנים (קובץ באתר: בענף `fix/seo`, מעלים לפי "ענפים", ומחכים ל"מיזגתי"), ולוחצים שוב |
| **Couldn't fetch** במפת האתר | בודקים את הקובץ בייצור. תקין? בודקים שוב מאוחר יותר |
| "חרגת מהמכסה" בבקשה להוספה, גם בבקשה הראשונה | המכסה היומית. היום לא מנסים שוב. הנוסח של בקשה שלא התקבלה, ו«מחר כתבי לי: "נבקש שוב מגוגל להוסיף את דף האודות".» (שלב ב, צעד 6) |
| Search Console נפתח בחשבון אחר | `https://search.google.com/u/<n>/search-console`, ובודקים לפי הכפתור בפינה |
| מסך כניסה של גוגל עם מייל של מישהו אחר ("זה החשבון שלך?") | לא מקלידים בו סיסמה. מחפשים במסך דרך לחשבון אחר, ולא נמצאה? רות תבדוק (שלב ב, צעד 1) |
| גוגל לא נותנת להתחבר בחלון של Playwright | תוכנית ב (סוף שלב ב) |
| ב־Bing מסך פתיחה ריק לפני הייבוא, למרות שהיא כבר פתחה בעבר חשבון | אולי נכנסה אז בדרך אחרת. שואלים פעם אחת. בחשבון חדש מסך ריק הוא ההתחלה הרגילה, ומייבאים ממנו |
| ב־Bing מסך פתיחה ריק אחרי Import | זה תקין. לא מייבאים שוב ולא שואלים אותה: טוענים מחדש, ופותחים את Sitemaps של האתר (שלב ג, צעד 1, סעיף 7) |
| ב־Bing האתר לא ברשימה לייבוא | הוא עוד לא מאומת ב־Search Console, או שנבחר חשבון גוגל אחר |
| IndexNow: 403 | קובץ המפתח לא בייצור, או שהתוכן שלו שונה מהמפתח |
| IndexNow: 422 | בבקשה כתובת שלא של האתר, או מפתח שלא תואם |
| IndexNow: 429 | יותר מדי בקשות. מחכים, ולא שולחים שוב כתובות שלא השתנו |
| IndexNow: אין תשובה | שולחים את אותה בקשה ל־`https://www.bing.com/indexnow` |
| מפתח שלא אמור להיות בקוד של האתר | עוצרים, ורות תבדוק, עוד היום (שלב א, צעד 10) |
| דף של שלב ה עם `X-Robots-Tag` | הכתובת חסרה ברשימה שבכלל, כתובה שם באותיות אחרות מבנתב, או בלי `$` אחריה (שלב ה, צעד 4). מתקנים לפני כל דבר אחר |
| כתובת כמו `/services/test-xyz` חוזרת בלי `X-Robots-Tag` | בכלל יצאו כל הכתובות שמתחילות ב־`services/`, או שחסר `$`. כל כתובת בשמה המלא (שלב ה, צעד 4) |
| דף של שלב ה בלי עיצוב או בלי לוגו | בכתובת עם שתי רמות, קישור או תמונה שלא כתובים מ־`/`. כותבים אותם מ־`/`, כמו `/logo.png` (שלב ה, צעד 3) |
| דף של שלב ה בייצור, ובקוד שחוזר ממנו `#root` ריק | הדף לא ב־`PUBLIC_PAGES`, או שנכנס לנתב ישירות ולא דרך הרשימה. מעבירים אותו לרשימה (שלב ה, צעד 3, סעיף 3), ובודקים את השורה `prerendered` בבנייה |
| אחרי שינוי בכלל, הגרסה לא עולה ב־Vercel | בכלל נוספו סוגריים, או שה־JSON לא תקין. בתוך הכלל רק `(?!...)` ו־`(?:...)`, כמו בדוגמה. (מה Vercel כותב במקרה כזה: לא נבדק עדיין. במחשב, הספרייה שקוראת את הכלל עצרה בשגיאה על סוגריים כאלה: 24.11.2026) |
| הטקסט ב־`llms.txt` שונה מהטקסט בדף | הקובץ לא עודכן אחרי שינוי בקובץ התוכן. מעתיקים מקובץ התוכן, מילה במילה (שלב ה, צעד 5, סעיף 1) |

## בסוף

1. **אומרים לה בארבע שורות מה נעשה.** בשורות 1 עד 3: מוכן, או מה חסר ובאיזה סקיל.
   1. הדפים הציבוריים מוכנים, והמסכים הפנימיים מסומנים "לא לחיפוש".
   2. האתר רשום ומאומת ב־Search Console, בחשבון <החשבון>. מפת האתר נשלחה, וביקשנו להוסיף את דף האודות.
      - גוגל לא קיבלה היום את הבקשה (שלב ב, צעד 6, סעיף 4)? במקום "וביקשנו להוסיף את דף האודות": "את הבקשה להוסיף את דף האודות גוגל לא קיבלה היום, בגלל המכסה היומית." ומיד אחרי השורה הזו: «מחר כתבי לי: "נבקש שוב מגוגל להוסיף את דף האודות".»
   3. Bing ייבא את האתר, ומנועים נוספים קיבלו הודעה על הדפים.
   4. גוגל מוסיפה דפים לאט: בדרך כלל כמה ימים עד כמה שבועות. יש מכסה יומית לבקשות, ובקשה לא מבטיחה הוספה. ומיד אחרי השורה הזו: «בעוד שבוע כתבי לי: "תבדוק אם האתר בגוגל".»
2. **סקיל המערכת:** לא כותבים ב־`build-my-system` ולא מציעים לכתוב בו. בקורס הזה כל תלמידה מוסיפה לו את הכללים בעצמה, בבקשה מדף הפרומפטים של המפגש. אם היא שואלת, אומרים לה את זה במשפט.
3. **CHANGELOG.** יש בתיקייה `CHANGELOG.md`? מוסיפים תחת `[Unreleased]` ← `### נוסף` את השורה "האתר רשום בגוגל וב־Bing, עם מפת אתר וקובץ למנועי הבינה". השורה כבר שם? לא מוסיפים שוב. אין קובץ? לא יוצרים.
4. **שומרים גרסה ומעלים, רק אם השתנה קובץ** (ה־CHANGELOG). אין `CHANGELOG.md`, או שהשורה כבר שם? לא פותחים ענף ולא Pull Request. השתנה? בענף `feature/seo-changelog`, כמו בשלב א, צעד 9: Pull Request, והיא ממזגת.
5. **יציאה מהחשבונות בחלון של Playwright.** לא ממשיכים עכשיו לסקיל backup-and-keep-alive, והחשבון שלה הוא חשבון הגוגל היחיד שמחובר בחלון (שלב ב, צעד 1)? מציעים לה לצאת מגוגל ומ־Bing Webmaster Tools, ובאישור שלה Claude יוצא משניהם, לפי השמות במסך. יש בחלון עוד חשבונות גוגל? לא מציעים לצאת: היציאה מגוגל מוציאה את כל החשבונות שבחלון. (היציאה עצמה, מגוגל ומ־Bing: לא נבדק עדיין בהרצה.)
6. **מה הלאה**, במשפט אחד, רק ממה שעוד לא נעשה:
   - אין מדיניות פרטיות או תנאי שימוש: הסקיל legal-pages. אין הצהרת נגישות: הסקיל accessibility. ובאותו משפט: «כשהדף מוכן, כתבי לי: "נעדכן את גוגל".»
   - אין עדיין גיבוי (אין `.github/workflows/backup.yml`): הסקיל backup-and-keep-alive, באותו חשבון גוגל, ושם גם האפליקציה בגוגל, אם עוד לא פתוחה.
   - עוד לא נבנו דפים שעוזרים לחיפוש (אין `app/src/content/search-pages.ts`): שלב ה. ובאותו משפט: «כשתרצי, בשיעור או בבית, כתבי לי: "נבנה דפים שעוזרים לחיפוש".»

דוגמה לקבצים ולטקסטים מוכנים, של עסק בדוי: `example.md`. בסופה דוגמה לשלב ה, של עסק הדמו של הקורס. היא מראה את הרמה ואת האורך. לא מעתיקים ממנה תוכן: לא משפטים, לא כתובות ולא מפתחות.

---

## מאיפה כל דבר

| מה | המקור |
|---|---|
| "האתר של רות" בטבלה הזו | הריפו של aiclearlyapp.com (clearly-world, גרסה 8e42c3a): `src/app/site-files.ts` (robots.txt, מפת האתר, llms.txt), `vercel.json`, `public/google….html`, קובץ המפתח ו־`scripts/indexnow.mjs`, `src/app/render.ts` (הכותרות), `src/app/structured-data.ts`, `scripts/prerender.mjs` |
| רק דף ציבורי אחד הוא הזהות לגוגל, עם תגיות ונתונים מובנים; מערכת סגורה נראית לגוגל ריקה | project-about-page של רות, ו־about-page של הקורס |
| הכותרת, התיאור, תגיות ה־`og:` ובלוק ה־`Organization` של דף האודות | project-about-page (Part 3, Part 4), דרך about-page. כאן רק בודקים |
| כותרת ותיאור לכל דף, שונים זה מזה | audit-website (meta-title, meta-description, כותרות כפולות), האתר של רות (כותרת לכל דף, עם " \| Clearלי"), והמסמכים של גוגל |
| כותרת אחת ותיאור אחד ב־head: מרשימה אחת, בקובץ המוכן, ובמעבר בין מסכים דרך `document.title` והתגית הקיימת | המסמך של React על `<title>`, בדיקה בהרצה של React 19 על דף לדוגמה (19.11.2026), המסמך של גוגל על JavaScript, והבדיקה בפרויקט בדיקה, באתר חי (24.11.2026) |
| בלי תגית noindex ב־`app/index.html` | המסמך של גוגל על JavaScript |
| robots.txt: כולם מוזמנים, וכל סורק בשמו; הפניה ל־llms.txt ולמפת האתר | ai-seo (בדיקת הבוטים, והקובץ ב־platform-ranking-factors), והאתר של רות (רשימת הסורקים, השורה הראשונה והשורה האחרונה) |
| לא חוסמים בוטים של בינה | ai-seo ("What NOT to Do", סעיף 5) |
| מפת אתר עם `lastmod`, רק עם דפים ציבוריים | site-seo-geo (lastmod), האתר של רות, והמסמך של גוגל |
| llms.txt | ai-seo ("Machine-Readable Files", llmstxt.org), site-seo-geo, והאתר של רות. שהוא הצעה, ושאף מנוע לא כתוב כמי שקורא אותו לבד: llmstxt.org. שהחיפוש של גוגל מתעלם ממנו: המסמך של גוגל על AI בחיפוש (ai-optimization-guide, 24.11.2026) |
| `Content-Type` של UTF-8 ל־llms.txt | `vercel.json` של האתר של רות. ושגם בלי כלל Vercel מחזיר אצלה קבצי `.txt` כ־UTF-8: בדיקה באתר שלה (19.11.2026) |
| `X-Robots-Tag: noindex, nofollow` מ־`vercel.json` | `vercel.json` של האתר של רות (האזור הפנימי), והמסמך של גוגל על noindex. החריגה של קובץ האימות ושל סוגי הקבצים, במקום כל כתובת עם נקודה, ו־`/index.html` בבדיקה: הבדיקה של ההרצה על אתר הדמו, והבדיקה החוזרת באתר החי (19.11.2026) |
| 404 על דף שקיים בקוד, ו־`vercel.json` עם `rewrites` | about-page, legal-pages ו־backup-and-keep-alive ("הכנה בגוגל", צעד 1) |
| הרשימה שבכלל מול הנתב, ו"נעדכן את גוגל" | אין מקור. ראו "מה שונה מהמקורות", סעיף 25 |
| נכס URL-prefix ב־Search Console | site-seo-geo |
| כתובת `/u/<n>/` ב־Search Console | site-seo-geo (17.10). ושבודקים קודם אילו חשבונות מחוברים, ולא מקלידים סיסמה במסך עם מייל של מישהו אחר: ההרצה על אתר הדמו (19.11.2026) |
| Search Console מפנה לדף ההסבר כשלא מחוברים, והכפתור Start now; Bing מפנה לדף הפתיחה שלו | בדיקה בכתובות עצמן (19.11.2026). שדף ההסבר מופיע גם כשמחוברים כמה חשבונות, ושהכפתור בעברית הוא "קדימה, מתחילים": ההרצה על אתר הדמו (19.11.2026) |
| אימות בקובץ HTML בתיקייה `public` | האתר של רות (`public/google….html`), והמסמך של גוגל |
| Playwright משנה שמות של הורדות | backup-and-keep-alive (שלב 2, צעד 6) |
| שליחת מפת האתר, בקשה להוספה, והמכסה היומית | site-seo-geo (בכל יום התקבלה בקשה אחת, והשאר קיבלו "נסה שוב מאוחר יותר"; ברישום: "~10 ליום"), והמסמכים של גוגל (מכסה יומית, בלי מספר). ש"חרגת מהמכסה" יכולה להופיע כבר בבקשה הראשונה, והנוסח המלא שלה: ההרצה על אתר הדמו (19.11.2026). ההמשך של בקשה שלא התקבלה: ראו "מה שונה מהמקורות", סעיף 26 |
| כמה זמן: כמה ימים עד כמה שבועות, ובקשה לא מבטיחה הוספה | המסמכים של גוגל |
| המצב "נסרק אך לא נכלל באינדקס", בעברית, ושהוא יכול להופיע כבר ביום הראשון | site-seo-geo (14.10), וההרצה על אתר הדמו (19.11.2026) |
| מסכים של גוגל בעברית, והשמות שבסקיל בעברית | backup-and-keep-alive (שלב 2, צעד 3: מסך ההסכמה בעברית, בבדיקה של 19.11.2026), וההרצה על אתר הדמו (19.11.2026: Search Console ומסכי הכניסה של גוגל בעברית, Bing Webmaster Tools באנגלית) |
| אותו חשבון גוגל ל־Search Console ולאפליקציה בגוגל | backup-and-keep-alive ("הכנה בגוגל", צעד 2) |
| Search Console בתנאים לאישור האפליקציה בגוגל, באימות המותג | about-page ("הקשר להגדרות של גוגל", תנאי 4) |
| ייבוא ל־Bing מ־Search Console, הרשאה, ומסך פתיחה ריק | site-seo-geo, והבלוג של Bing. המסכים שבדרך, "באותה לשונית", הכפתור "המשך", האתרים שמגיעים מסומנים, ומסך הפתיחה הריק אחרי Import: ההרצה על אתר הדמו (19.11.2026) |
| IndexNow: קובץ מפתח, בקשה אחת, ונפילה ל־`www.bing.com/indexnow` | site-seo-geo, `scripts/indexnow.mjs` באתר של רות, ai-seo (חלק Copilot), ו־indexnow.org |
| מה Google-Extended עושה | המסמך של גוגל (במקום מה שכתוב ב־ai-seo) |
| דפים שנבנים בדפדפן, סורק שלא מריץ קוד, ולמה בונים מראש | ai-seo ("Agentic Experiences", "What NOT to Do" סעיף 6), okf.md (llms.txt הוא שלט שמפנה לדפים), והמסמך של גוגל על JavaScript ("server-side or pre-rendering is still a great idea"). הסיכומים והשאלות של שלב ה נשארים גם ב־llms.txt: ראו "מה שונה מהמקורות", סעיף 31 |
| בנייה מראש של הדפים הציבוריים: `entry-server.tsx`, `scripts/prerender.mjs`, וקובץ `dist/<הכתובת>/index.html` לכל דף | הבקשה של רות (24.11.2026), `scripts/prerender.mjs` באתר של רות (גרסה 8e42c3a), המדריך של Vite ל־SSR ("Pre-Rendering / SSG"), `prerenderToNodeStream` של React, ו־`StaticRouter` של React Router (כולם נבדקו ב־24.11.2026) |
| בלי `cleanUrls`, וקבצים בתיקייה לכל כתובת | המסמך של Vercel על `vercel.json` (`cleanUrls`, ו־"precedence is given to the filesystem prior to rewrites being applied"), המסמך של גוגל על קובץ האימות ("does not follow redirects"), והבדיקה באתר חי, בפרויקט בדיקה (24.11.2026) |
| `createRoot` ולא `hydrateRoot` | המסמך של React על `createRoot` (24.11.2026), והבדיקה בפרויקט הבדיקה. ראו "מה שונה מהמקורות", סעיף 7 |
| מה מפיל את הבנייה מראש, ו־`typeof window` ולא `typeof localStorage` | המסמך של Node על `localStorage` (24.11.2026), בדיקה בבנייה ב־Vercel (Node v26.13.1) ובמחשב (Node 22), ובדיקה של supabase-js 2.107.0 ב־Node (24.11.2026) |
| כתובות בלי `#`, וקישורים רגילים בין הדפים | המסמך של גוגל על JavaScript (History API, קישורי `<a href>`) |
| הבדיקות בשלב ד ובשער של שלב א, כולל סוד בקוד | הקטגוריות של audit-website (Core SEO, Social, Schema, Crawlability, Content, Images, Links, Security) |
| הטוקן של Supabase (`sbp_`) כסוד | backup-and-keep-alive ("סודות"), והמסמכים של Supabase (הצורה) |
| מנועי הבינה: ChatGPT, Claude ו־Gemini | ai-seo (הטבלה "The AI Search Landscape") |
| Test live URL | המסמך של גוגל על URL Inspection, וההרצה על אתר הדמו (19.11.2026: המסך והשמות בעברית) |
| הבדיקה הידנית בגוגל וב־ChatGPT | ai-seo ("DIY Monitoring") |
| הסריקה הרדודה ואחריה העמוקה, ובדיקת ה־checksum | audit-website |
| איך מדברים איתה, מי לוחץ, תוכנית ב, שמירה והעלאה | about-page, legal-pages ו־backup-and-keep-alive של הקורס |
| העברית ב־`llms.txt` נראית שבורה במחשב, ותקינה באינטרנט | ההרצה על אתר הדמו (19.11.2026) |
| בלי `backup.yml` האפליקציה בגוגל עדיין יכולה להיות פתוחה | ההרצה על אתר הדמו (19.11.2026), לפי מי שהריץ אותה. לא נבדק שוב |
| היציאה מגוגל מוציאה את כל החשבונות שבחלון, ולכן יוצאים רק כשהחשבון שלה הוא היחיד, וגם מ־Bing | ההרצה על אתר הדמו (19.11.2026: שלושה חשבונות גוגל באותו חלון), והבדיקה של התוצאות שלה. היציאה עצמה לא נבדקה |
| כל קובץ שהשלב יצר או שינה נכנס לגרסה, בבדיקה ב־`git status`; בדיקת הסוד גם בקבצי קוד שנטענים אחר כך | הבדיקה של ההרצה (19.11.2026). שני אלה צפי, ולא משהו שקרה בהרצה: שם כל הקבצים נכנסו, והיה קובץ קוד אחד |
| שלב ה: דף לכל שירות אמיתי, דף לסוג אירוע, ודף שאלות נפוצות | הבקשה של רות (24.11.2026), ואתר האירועים שרות בנתה (הריפו nechami-site, גרסה 4e07c44: שלושה דפי אירועים מתבנית אחת עם Service, דף שאלות עם FAQPage ומסך ניהול; גרסה 6753684: llms.txt ונתונים מובנים) |
| ארבעת הסוגים של מה שמחפשת רוצה | seo-keyword (Stage 2, ו־intent-classification-guide). בלי כלי: "If no tool is available" באותו סקיל |
| דף רק כשיש לו ערך משלו; מאחדים דפים שאפשר להבדיל רק לפי השם; דף בלי הפרטים שהוא צריך לא נבנה | programmatic-seo (template-design-patterns: "Distinctive value per page" ומבחן הדפים זה ליד זה; common-pseo-failures: "Pages look identical"; "Crawl budget management": דף בלי מספיק נתונים לא מקבל כתובת ציבורית) |
| בלי דף לכל עיר, ובלי הרבה דפים דומים | המסמך של גוגל על ספאם (Doorways, Scaled content abuse), והמסמך של גוגל על תוכן מועיל (24.11.2026) |
| בלי שני דפים לאותו חיפוש | seo-onpage (Failure patterns), pillar-content-architecture ("No facet duplication") |
| תשובה בפסקה הראשונה, כותרות בניסוח של שאלה, רשימות, וחלק שעומד בפני עצמו | seo-aeo-geo (extraction-friendly-patterns, דפוסים 1, 2, 5, 7 ו־8), ai-seo (FAQ Block ב־content-patterns), programmatic-seo ("Above-the-fold answer") |
| חלק בלי תוכן לא מופיע | programmatic-seo ("Variable density") |
| `<שם השירות> \| <שם העסק>`, ותיאור לכל דף | seo-onpage (title-and-meta-patterns), דפי האירועים באתר האירועים שרות בנתה, והמנגנון של שלב א, צעד 2 |
| כתובת קצרה באנגלית, עם מקפים | seo-onpage (URL slug) |
| קישורים בין הדפים ומדף האודות | pillar-content-architecture (Internal linking architecture), seo-onpage (Internal links), והמסמך של גוגל על AI בחיפוש ("findable through internal links") |
| תבנית אחת, ותוכן בקובץ אחד | אתר האירועים שרות בנתה (EventPageTemplate; אחר כך דפי האירועים מהמסד, עם מסך ניהול, בגרסה 878bc59), ו־programmatic-seo ("Design pages as renders from data") |
| `Service` ו־`FAQPage`, מאותו תוכן כמו הדף | אתר האירועים שרות בנתה (EventPageTemplate, FAQSchema), schema.org (Service, FAQPage, Question; גרסה 30.1), והכללים של גוגל לנתונים מובנים ("Don't mark up content that is not visible") |
| גוגל כבר לא מציגה FAQ, `Service` לא ברשימה של גוגל, וגוגל קוראת JSON-LD שהקוד כותב | https://developers.google.com/search/updates, הבלוג של גוגל מ־8.8.2023, ה־Search gallery, והמסמך של גוגל על נתונים מובנים מ־JavaScript (כולם 24.11.2026) |
| השאלות והסיכומים ב־llms.txt, כקישורים עם הערה | ההנחיה לשלב (24.11.2026), והפורמט של llmstxt.org |
| הכלל עם הדפים החדשים: כל כתובת בשמה, `$` אחרי כל אחת, ובלי סוגריים חדשים | שלב א, צעד 8, ובדיקה במחשב ב־path-to-regexp 6.1.0, עם ההגדרות של Vercel CLI 54.13.0 (24.11.2026). לא נבדק באתר חי |
| שליחה חוזרת של מפת האתר אחרי שינוי גדול, ובלי אחרי שינוי קל | עזרת Search Console על דוח Sitemaps (24.11.2026) |
| לא כותבים הערכה, ובודקים מול בעלת העסק | הכלל "לא ממציאים פרטים", ואתר האירועים שרות בנתה: הערות "placeholder" ו"הערכה ראשונית" בגרסה 4e07c44, ותיקוני המיתוג והכשרות בגרסאות 5b1ed5e ו־878bc59 |
| מסך ניהול לתוכן מחכה לכניסה ולהרשאות | אתר האירועים שרות בנתה (`/admin/faq`, והטבלה `faq_items` במיגרציה 005) |
| שמירה לפי כללי הגרסאות בסקיל המערכת, ובדיקה בייצור רק אחרי "מיזגתי" | סקיל המערכת של קורס הסמינר (`ai-dev-course/skills/build-my-system`, חלק "גרסאות, ענפים ו־GitHub") |

## מה שונה מהמקורות

הסעיף הזה בשביל רות. מה שמסומן **לשאול את רות** עוד לא הוחלט: עד שרות עונה, הסקיל עובד כמו שכתוב בו, ובשיחה עם תלמידה לא שואלים על זה.

**ההרצה המלאה לפני שהסקיל יוצא לתלמידות** נעשתה ב־19.11.2026, על אתר הדמו של הקורס, בחשבון הגוגל של הדמו. מה שנבדק בה כתוב בסקיל כמו שנראה במסך, כולל השפה של המסך ושמות הכפתורים, והתיקונים שלה כבר בסקיל. מה שעוד מסומן "לא נבדק עדיין" לא הגיע להרצה, או שלא ניתן לבדוק אותו בה: השיטה של תג HTML, אם נכס URL-prefix מספיק לאימות המותג, אם מנועי הבינה מכבדים את `X-Robots-Tag`, איך מוצאים את המספר של החשבון ב־`/u/<n>/`, הדרך מרשימת הנכסים ו־My Sites ב־Bing, האישור של בקשה שהתקבלה, הבקשה החוזרת ביום שאחרי, היציאה מהחשבונות, ומייל מגוגל על noindex. גם תוכנית ב, ההודעה לרות, המצבים של אחרי שבוע, והעלאה ל־GitHub עם בנייה של Vercel ממנו לא הגיעו להרצה. **בעוד שבוע בערך:** בודקים בתיבת הדואר של הדמו ובפעמון של Search Console אם גוגל שלחה מייל על המסכים שמסומנים noindex.

**שלב ה** נכתב ב־24.11.2026, ועוד לא נבדק בהרצה מלאה: לא הבנייה על אתר הדמו, לא הכלל עם הכתובות החדשות באתר חי, ולא השליחה החוזרת של מפת האתר. הכלל נבדק רק במחשב (שלב ה, צעד 4).
**הבנייה מראש** (שלב א, צעד 2) נכתבה ב־24.11.2026, ונבדקה באותו יום באתר חי, בפרויקט בדיקה נפרד ב־Vercel (`ofek-prerender-test`, בחשבון של הדמו), עם עותק של מערכת אופק ועם דף שירות אחד בכתובת עם שתי רמות. באותה בדיקה נבדק באתר חי גם הכלל של "לא לחיפוש" עם `services/consulting$`. היא לא נבדקה באתר הדמו של הקורס, במערכת בלי נתב באתר חי (רק בנייה במחשב), ולא מול גוגל, ב"בדיקה של כתובת אתר פעילה".

1. **רק הדפים הציבוריים.** ai-seo, audit-website והאתר של רות כתובים לאתר שכל הדפים בו ציבוריים. כאן רוב המערכת היא מסכים פנימיים, ולכן הם מסומנים "לא לחיפוש", ורק הדפים הציבוריים נכנסים למפת האתר ול־llms.txt.
2. **הכלל של "לא לחיפוש".** באתר של רות הכותרת `X-Robots-Tag: noindex, nofollow` חלה על `/admin/` ועל `/api/`. כאן היא חלה על כל כתובת, חוץ מהדפים הציבוריים, מקובץ האימות של גוגל ומקבצים לפי הסוג שלהם, כי המסכים הפנימיים יושבים בשורש האתר ולא תחת קידומת אחת. הערך זהה. בנוסח הראשון של הסקיל יצאה מהכלל כל כתובת עם נקודה, ובאתר הדמו `/index.html`, `/about.html` וכתובות דומות החזירו את המערכת בלי הכותרת. הנוסח החדש נבדק באתר החי (19.11.2026). הפער שנשאר: כתובת שנגמרת באחת הסיומות שברשימה, או שנראית כמו קובץ האימות של גוגל, ואין מאחוריה קובץ. ההשוואה של רשימת הסיומות לקבצים שלה, ו"לא את `html`", הן בלי מקור: הן באות מהמעבר לרשימת סיומות.
3. **בלי `Disallow` ב־robots.txt.** האתר של רות גם חוסם את `/admin/` ואת `/api/` ב־robots.txt. כאן לא, כי לפי גוגל robots.txt לא מוציא דף מהחיפוש, ודף חסום לא מראה לגוגל את ה־noindex שלו. ככה ה־noindex הוא שעובד. הנימוק הזה הוא של גוגל. אם הסורקים של מנועי הבינה מכבדים את `X-Robots-Tag`: לא נבדק עדיין (גוגל עצמה כותבת שמנועים אחרים עלולים להבין noindex אחרת). אצל רות שורות ה־`Disallow` חלות גם על כל הסורקים של הבינה, ובמפגש 4 המסכים הפנימיים בדרך כלל עוד לא מאחורי כניסה (legal-pages). **לשאול את רות.**
4. **robots.txt בקבוצה אחת.** באתר של רות יש קבוצה לכל סורק, כי כל אחת חוזרת על שורות ה־`Disallow`. בלי השורות האלה, קבוצה אחת עם כל השמות שווה לה, לפי גוגל, וכך גם הפורמט ב־ai-seo. רשימת הסורקים היא של האתר של רות, והיא רחבה מזו של ai-seo. CCBot מוזמן, כמו אצל רות (ב־ai-seo חסימה שלו היא החלטה עסקית).
5. **Google-Extended.** ב־ai-seo כתוב שהוא של Gemini ושל AI Overviews. לפי גוגל, הוא קובע שימוש באימון Gemini ובתשובות שלו, ולא משפיע על ההופעה בחיפוש. הסקיל אומר מה שגוגל אומרת, והסורק נשאר מוזמן, כמו אצל רות.
6. **כותרת ותיאור מרשימה אחת.** באתר של רות כל דף נבנה מראש כקובץ HTML מלא, עם הכותרת שלו. כאן גם, מאז הבנייה מראש (סעיף 7): השם והתיאור של כל דף ציבורי כתובים ברשימה אחת, `app/src/public-pages.tsx`, ומשם הם נכתבים בקובץ המוכן. במעבר בין מסכים בלי טעינה מחדש, הרכיב `PublicPageMeta` משנה את הכותרת ואת התיאור שכבר ב־`index.html`, בלי ספרייה חדשה (הכלל של about-page) ובלי תגית שנייה. גוגל קוראת אותם (המסמך של גוגל על JavaScript). הנוסח הקודם, קובץ עזר בכל דף שמחזיר כשיוצאים ממנו את הערכים שהיו קודם, יצא: עם קובץ מוכן, הערכים שהיו קודם הם של הדף שנטען, ולא של `index.html`, ומסך פנימי היה מקבל את השם של דף ציבורי.
7. **בנייה מראש של הדפים הציבוריים (prerender).** רות ביקשה אותה ב־24.11.2026, והיא בשלב א, צעד 2. גם ai-seo ("What NOT to Do", סעיף 6) וגם המסמך של גוגל על JavaScript ממליצים עליה, כי לא כל הסורקים מריצים קוד. כמו באתר של רות: מהתבנית `dist/index.html`, קובץ `dist/<הכתובת>/index.html` לכל דף, מסקריפט `scripts/prerender.mjs` שרץ אחרי הבנייה לשרת של Vite, וכל בעיה עוצרת את הבנייה. מה שונה:
   - **רק הדפים הציבוריים** נבנים מראש. אצל רות, כל האתר.
   - **בלי `trailingSlash: true`,** שאצל רות כל הכתובות נגמרות בו. כאן הכתובות בלי `/` בסוף, ו־`/about/` מסומן "לא לחיפוש".
   - **בלי `cleanUrls`.** בבדיקה באתר חי הוא שבר את הכלל של `rewrites` (המסכים הפנימיים החזירו 404) ונתן הפניה לקובץ האימות של גוגל.
   - **`createRoot` ולא `hydrateRoot`.** React כותבת שעל HTML שנבנה מראש משתמשים ב־`hydrateRoot`. כאן `createRoot` מצייר את הדף מחדש, כי `hydrateRoot` דורש ציור ראשון זהה לגמרי לקובץ, וכל הבדל נותן שגיאות. בבדיקה: בלי שום הודעה ב־console. **לשאול את רות:** לעבור ל־`hydrateRoot` אחרי שזה רץ אצל כמה תלמידות, או להשאיר `createRoot`.
   - **רשימה אחת של הדפים הציבוריים,** שממנה גם הנתב. הסקילים about-page ו־legal-pages מוסיפים `<Route>` ישר לנתב, ולכן כשהם רצים אחרי שלב א, הדף שלהם עובר לרשימה ב"לפני שמתחילים", סעיף 5. **לשאול את רות** אם להוסיף לסקילים האלה משפט על הרשימה (כמו בסעיף 25).
8. **נתונים מובנים.** באתר של רות יש מערך שלם (WebSite, Organization, Person, WebPage, BreadcrumbList, Course, Event, Service, FAQPage, Article). כאן ה־`Organization` של about-page בדף האודות, ובשלב ה, אם נבנה, `Service` בכל דף שירות ו־`FAQPage` בדף השאלות (סעיפים 32 ו־33). HowTo ו־Article, שמוזכרים ב־ai-seo, לא נכנסו: אין בדפים האלה תוכן כזה. גם `WebSite` ו־`WebPage`, שאצל רות נמצאים בכל דף, כולל מדיניות הפרטיות ותנאי השימוש, לא נכנסו לכאן. **לשאול את רות:** להוסיף אותם לדפים הציבוריים, או להשאיר רק את ה־`Organization` של about-page.
9. **תגיות `og:` ו־`canonical`.** תגיות ה־`og:` נשארות כמו שהסקיל about-page כתב אותן ב־`index.html`, לכל הכתובות, וגם בקובץ המוכן של כל דף ציבורי, כולל `og:url` של `/about`. אין `og:` לכל דף. **לשאול את רות** אם לכתוב גם אותן לכל דף, בבנייה מראש. audit-website בודק `canonical`: הוא נכתב רק בקובץ המוכן של כל דף ציבורי, לכתובת שלו, ולא ב־`index.html`, כי שם הוא היה חל על כל הכתובות. מאותה סיבה אין שם תגית `robots` עם noindex. במעבר בין מסכים בלי טעינה מחדש `canonical` לא משתנה (גוגל: לא לשנות אותו מהקוד).
10. **התאריך במפת האתר.** באתר של רות זה יום הפרסום של התוכן. כאן תאריך העדכון שכתוב בדף, או התאריך של הגרסה האחרונה ששינתה אותו. בלי `priority` ו־`changefreq`, שגוגל מתעלמת מהם.
11. **llms.txt קצר יותר.** באתר של רות יש בו פסקה באנגלית, פסקת עובדות, ופרקים של קורסים, כתבות ועבודות. כאן רק שם המערכת, התיאור, שורת העסק, "אודות" ו"יצירת קשר", מתוך דף האודות, ואחרי שלב ה גם "שירותים" ו"שאלות נפוצות", מילה במילה מהדפים (סעיף 31). הפסקה באנגלית לא נכנסה, כי התלמידה צריכה לאשר כל מילה שיוצאת בשם העסק. **לשאול את רות.**
12. **בלי llms-full.txt.** אצל רות הוא מחזיק את הטקסט המלא של דפי הקורסים, של "עליי" ושל השאלות הנפוצות. במערכת של תלמידה, כל הטקסט הציבורי של דף האודות כבר נכנס ל־llms.txt, וקובץ מלא היה חוזר עליו. גם אחרי שלב ה: יש רק שלושה עד שישה דפים, ולכן הפסקה הראשונה של כל שירות וכל השאלות והתשובות נכנסות ל־llms.txt עצמו. באתר האירועים שרות בנתה הטקסט של השאלות לא נכנס לאף קובץ: גם ב־llms.txt וגם ב־llms-full.txt יש רק קישור לדף השאלות, כי שם הדפים מגיעים מהשרת. כאן, מאז הבנייה מראש, גם הדפים בנויים מראש, והשאלה עברה לסעיף 31. **לשאול את רות.**
13. **הדפים המשפטיים לא ב־llms.txt.** גם באתר של רות הם לא שם. הם במפת האתר.
14. **שיטת האימות.** קובץ HTML, כמו באתר של רות. תגית HTML ב־`index.html` רק אם ההורדה לא הגיעה פעמיים. אם התגית עובדת כש־`/` מסומן "לא לחיפוש": לא נבדק עדיין.
15. **בקשה להוספה רק ל־`/about`.** אצל רות נשלחו בקשות לכמה דפים. כאן שאר הדפים מגיעים ממפת האתר.
16. **IndexNow בלי סקריפט.** באתר של רות יש `scripts/indexnow.mjs`, ששולח ל־`api.indexnow.org`. כאן Claude שולח את אותה בקשה ישירות, בלי קובץ בריפו, ובלי תשובה עובר ל־`www.bing.com/indexnow`, כמו שקרה אצל רות. **לשאול את רות:** להוסיף סקריפט כזה לריפו של התלמידה, או לא.
17. **Bing.** אצל רות היא פתחה את החשבון בעצמה, ואחר כך Claude המשיך. כאן היא מתחברת ונותנת הרשאה, ו־Claude עושה את השאר ב־Playwright. את הכפתור של ההרשאה Claude מעתיק מהמסך, והיא לוחצת עליו. בהרצה (19.11.2026) הוא היה "המשך", ולא Allow כמו בפוסט של Bing.
18. **audit-website לא בשימוש אצל התלמידה.** הסיבות בשלב ד. הבדיקות שלה שנוגעות לדפים הציבוריים נעשות ידנית. רוחב צר, בינוני ורחב, נגישות ודפים משפטיים נשארים לסקילים של הקורס. מהירות האתר לא נבדקת בסקיל הזה. **לשאול את רות.**
19. **בדיקת סוד בקוד של האתר.** מהקטגוריה Security של audit-website. Claude בודק בלי להדפיס ערך, בכל קבצי הקוד, גם באלה שנטענים רק כשעוברים למסך, רק לפי הצורות של המפתחות ושל הטוקן של Supabase, ולא לפי 96 הצורות של squirrel, ועוצר אם נמצא מפתח שלא אמור להיות שם. הבדיקה בשער של שלב א, לפני כל רישום.
20. **שער לפני הרישום.** בשום מקור אין תנאי כזה: שלב ב מתחיל רק אחרי שהבדיקה באינטרנט עברה, כולל הסימון "לא לחיפוש" והבדיקה שאין סוד בקוד. **לשאול את רות.**
21. **מה מ־ai-seo לא נכנס:** בדיקת נראות עם טבלת שאלות, כלי מעקב (Otterly ודומיו), נוכחות בוויקיפדיה ובאתרי ביקורות, תבניות תוכן (חוץ מתשובה בראש כל חלק ומבלוק של שאלות, שנכנסו לשלב ה), נתונים וציטוטים (בשלב ה רק מספר שבעלת העסק נתנה), `pricing.md` (בדף האודות אין מחירים, לפי about-page, ובשלב ה מחיר נכתב רק בדף השירות, אם היא נתנה אותו), חבילת OKF (ai-seo עצמו אומר לוותר עליה באתר של פחות מעשרה דפים), ופרופיל עסק בגוגל (הוא של העסק, לא של המערכת; ובמחקר של רות, לא לעסק שעובד רק באינטרנט).
22. **ההנחיה לקורס:** איך מדברים איתה, שאלה אחת בכל פעם, מי לוחץ, תוכנית ב, CHANGELOG, ושמירה בענף, עם Pull Request שהיא ממזגת ובדיקה באינטרנט אחרי "מיזגתי". בלי שורה בסקיל המערכת: בקורס הזה התלמידה מוסיפה את הכללים בעצמה. כמו בסקילים של הקורס.
23. **"האתר של רות" הוא הריפו של האתר.** ב־site-seo-geo אין את הפרטים: רשימת הסורקים, הכללים ב־`vercel.json`, קובץ האימות, IndexNow, הכותרות והנתונים המובנים לקוחים מהריפו של aiclearlyapp.com, בגרסה 8e42c3a (השורה הראשונה ב"מאיפה כל דבר"). **לשאול את רות** אם הריפו נחשב "העבודה שלה באתר".
24. **"ורות תבדוק" מהבית.** בשום מקור לא כתוב איך תלמידה פונה לרות מהבית. כאן Claude כותב לה הודעה קצרה לשלוח לרות במייל, בלי ערך של מפתח, וכשנמצא מפתח בקוד של האתר, עוד באותו יום. **לשאול את רות** איזו כתובת או דרך לכתוב בסקיל.
25. **הרשימה מול הנתב, בכל הרצה.** בשום מקור אין בדיקה כזו. דף ציבורי שנוסף אחרי הריצה הקודמת, למשל מ־legal-pages מתוך backup-and-keep-alive, נכנס לרשימה שבכלל ולמפת האתר, מקבל כותרת ותיאור, ונשלח ל־IndexNow. הסקילים legal-pages, accessibility ו־backup-and-keep-alive עוד לא מפנים למשפט "נעדכן את גוגל". **לשאול את רות** אם להוסיף להם את המשפט.
26. **בקשה שגוגל לא קיבלה.** בשום מקור אין המשך לבקשה שנדחתה בגלל המכסה היומית. בהרצה (19.11.2026) גם הבקשה הראשונה נדחתה, ולכן נוספו: הנוסח של בקשה שלא התקבלה בסוף שלב ב ובסוף, «מחר כתבי לי: "נבקש שוב מגוגל להוסיף את דף האודות"», ובדיקה של `/about` בכל הרצה חוזרת, עם בקשה אחת אם גוגל עדיין לא מכירה את הדף. הבדיקה לא מבדילה בין בקשה שנדחתה לבין בקשה שהתקבלה ועוד לא נסרקה, ולכן בהרצה חוזרת באותו יום, אחרי בקשה שהתקבלה, הבקשה הנוספת עלולה לקבל "חרגת מהמכסה". **לשאול את רות:** לבקש שוב בכל הרצה חוזרת, או רק כשהיא כותבת "נבקש שוב מגוגל להוסיף את דף האודות".
27. **כמה חשבונות גוגל בחלון.** במקורות יש רק את `/u/<n>/` (site-seo-geo). בהרצה (19.11.2026) Search Console עבר לדף ההסבר גם כשהחשבון הנכון היה מחובר, והכפתור "קדימה, מתחילים" הוביל לכניסה מחדש בחשבון אחר שבחלון. לכן בודקים קודם את החשבונות, ולא מקלידים סיסמה במסך עם מייל של מישהו אחר. מאותה סיבה יוצאים מגוגל רק כשהחשבון שלה הוא היחיד בחלון.
28. **דפים לחיפוש במערכת ניהול (שלב ה).** programmatic-seo בנוי למאות ואלפי דפים מנתונים, ו־pillar-content-architecture לדף מרכזי ארוך עם 8 עד 15 דפים סביבו. כאן שלושה עד שישה דפים. מ־programmatic-seo נלקחו רק המבחנים: לכל דף ערך משלו, שני דפים שאפשר להבדיל רק לפי השם מתאחדים, ודף בלי הפרטים שהוא צריך לא נבנה. מ־pillar-content-architecture נלקחו הקישורים בין הדפים, ושאין שני דפים לאותו נושא. בלי מספר מילים: גוגל שואלת אם כותבים למספר מילים מסוים כי שמעו שהיא מעדיפה אותו. דף האודות משמש כמרכז, ואין דף `/services` שמרכז את השירותים. **לשאול את רות** אם היא רוצה דף כזה.
29. **בלי מחקר של מילות חיפוש.** seo-keyword מתחיל ב־200 עד 500 חיפושים מכלי או מ־Search Console, ומחליט על הסוג לפי מה שרואים בתוצאות של גוגל. כאן אין כלי, ולמערכת חדשה עוד אין נתונים: את הסוג מסיקים ממה שהעסק עושה, ולא כותבים כמה מחפשים. Ahrefs ושאר הכלים בתשלום לא בשימוש. **לשאול את רות** אם לחזור לזה אחרי כמה שבועות, עם החיפושים שב־Search Console.
30. **שם העסק בכותרת.** בשלב א הכותרת היא `<שם הדף> | <שם המערכת>`. בדפי שלב ה היא `<שם השירות> | <שם העסק>`, כמו באתר האירועים שרות בנתה, כי מי שמחפשת שירות מחפשת את העסק, ולא את מערכת הניהול שלו. כך באותו אתר יש שני סיומים שונים לכותרות. **לשאול את רות.**
31. **הדפים בנויים מראש, ובאתר האירועים שרות בנתה מגיעים מהשרת.** אתר האירועים שרות בנתה בנוי ב־Next.js, וכל דף מגיע מהשרת עם הטקסט והנתונים המובנים. כאן, מאז הבנייה מראש (סעיף 7), גם דף שירות ודף השאלות מגיעים עם הטקסט והנתונים המובנים שלהם, בקובץ מוכן. הסיכום של כל שירות וכל השאלות והתשובות נשארו גם ב־llms.txt, מילה במילה, בשביל מנועים שקוראים אותו. גוגל כותבת שהחיפוש שלה מתעלם מהקובץ. **לשאול את רות:** עכשיו, כשהדפים בנויים מראש, להשאיר ב־llms.txt את כל התשובות, או רק קישור לכל דף, כמו באתר האירועים.
32. **FAQPage, למרות שגוגל כבר לא מציגה אותו.** באתר האירועים שרות בנתה (30.6.2026) הבלוק נוסף כשגוגל כבר הפסיקה להציג שאלות ותשובות (מ־7.5.2026), וההערה בקוד שם עוד מתארת תוצאה כזו. כאן הבלוק נשאר כי הוא מתאר את מה שבדף לפי schema.org, ולפי גוגל (2023) נתונים מובנים שלא בשימוש לא מזיקים. ש"מנועים אחרים קוראים אותו" כתוב ב־ai-seo וב־seo-aeo-geo, ולא נבדק במסמך רשמי. אתרים לא רשמיים כתבו שגוגל עדיין משתמשת בו כדי להבין את הדף: זה לא נמצא במסמכים של גוגל, ולכן לא כתוב בסקיל. **לשאול את רות:** להשאיר את הבלוק, או לוותר עליו.
33. **`Service` בלי פרטים שלא בדף.** באתר האירועים שרות בנתה ה־`provider` הוא `FoodEstablishment`, עם פרטי קשר ועיר. כאן `Organization`, באותו שם ובאותה כתובת כמו בדף האודות, ואזור וקהל רק אם היא אמרה אותם. `Service` לא ברשימה של גוגל, ולכן הוא לא נותן בגוגל תוצאה מיוחדת.
34. **התוכן בקובץ בקוד, ולא במסד עם מסך ניהול.** באתר האירועים שרות בנתה השאלות נשמרו מההתחלה בטבלה במסד, עם מסך ניהול (`/admin/faq`), ודפי האירועים עברו למסד אחר כך. כאן עוד אין כניסה והרשאות, ולכן התוכן בקובץ אחד, ומשנים אותו דרך Claude.
35. **בלי הערכות ובלי טקסט זמני.** באתר האירועים שרות בנתה נכתבו בהתחלה יתרונות "כהערכה ראשונית", סיפור זמני בדף האודות, מספרים  ושעות פתיחה זמניות, עם הערות לבדוק מול הלקוחה, ואחר כך תוקנו. כאן פרט שלא ידוע לא נכתב, ודף שחסר לו מה שהוא צריך מחכה.
36. **דף האודות נשאר, ונוספים לו רק קישורים.** באתר האירועים שרות בנתה דף האודות נכתב מחדש באותה עבודה: סיפור, יתרונות, מספרים, ונתונים מובנים מסוג AboutPage ו־Person. כאן הוא נשאר של הסקיל about-page, ונוסף לו רק חלק של קישורים. **לשאול את רות** אם לשדרג גם אותו.
37. **"איך מתחילים" במייל.** באתר האירועים שרות בנתה בכל דף יש כפתורים ליצירת קשר בדרכים אחרות. כאן "איך מתחילים" הוא המייל מדף האודות, או טופס, לפי הכלל של הקורס.
38. **בלי דף לכל עיר, ובלי דף לכל מילה נרדפת.** ב־programmatic-seo דפים לפי מיקום הם דוגמה מוכרת לשיטה. כאן הם לא נבנים, כי עם אותו תוכן הם דפי מעבר, לפי הכללים של גוגל.
39. **שמירה בענפים.** בקורס הסמינר כל השלבים, גם שלב ה, עובדים בענף ובבקשת מיזוג, והתלמידה ממזגת בעצמה. כל בדיקה בייצור מחכה ל"מיזגתי".
40. **אישור לפני ייצור.** לפי רות (24.11.2026): את הטקסט של דפי שלב ה היא מאשרת במחשב, אחרי שהדפים נבנו ולפני שהם נשמרים, עולים לייצור ונשלחים לגוגל ול־IndexNow. כך גם כל תיקון. כך נשמר גם סעיף 11: היא מאשרת כל מילה שיוצאת בשם העסק.
41. **מפת האתר נשלחת שוב, ובלי בקשה לכל דף.** אחרי כמה דפים חדשים, שליחה חוזרת ב־Search Console, לפי העזרה של גוגל על שינוי גדול. בקשה להוספה רק ל־`/about`, כמו בסעיף 15. שירות אחד חדש: בלי שליחה חוזרת.
42. **עסק שיש לו אתר משלו.** כל המקורות כתובים לאתר של העסק. כאן הדפים יושבים בכתובת של מערכת הניהול. אם לעסק כבר יש אתר, ייתכן שהדפים האלה שייכים לשם. מה גוגל עושה כששני אתרים של אותו עסק עונים על אותו חיפוש: לא נבדק. **לשאול את רות.**
