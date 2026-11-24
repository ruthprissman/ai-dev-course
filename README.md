# קורס פיתוח בעזרת AI

ה-Skills והדוגמאות של הקורס, מאת רות פריסמן ([Clearלי](https://aiclearlyapp.com)).
המאגר מתעדכן לאורך הקורס.

## Skills

| Skill | מה הוא עושה | מתי | ZIP |
|---|---|---|---|
| [`idea-analysis`](skills/idea-analysis/SKILL.md) | מראיין אתכן על הרעיון לפרויקט, שאלה אחת בכל פעם, וכותב אפיון של עמוד אחד ב-`docs/idea.md` | ההכנה לקורס | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/idea-analysis.zip) |
| [`plan-my-system`](skills/plan-my-system/SKILL.md) | קורא את הטקסט שכתבתן על העסק, בתיקייה שבה אתן עובדות, ומראיין אתכן בתשעה שלבים לתכנון המערכת. שומר הכול ב-`תכנון המערכת.md` | אחרי מפגש 1 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/plan-my-system.zip) |
| [`build-my-system`](skills/build-my-system/SKILL.md) | סקיל המערכת שלנו: מלווה את הפרויקט וגדל בכל מפגש. בהתחלה: עובד לפי התכנון, משרטט אפיון ויזואלי של כל המסכים בקובץ HTML אחד (בודק איתך, מציע תוכנית, ורק אז כותב), ועובד בענפים: כל עבודה בענף משלה, Pull Request, ומיזוג ל-main. את החלקים הבאים כל אחת כותבת בעצמה, בבקשות מדף הפרומפטים של כל מפגש | מפגש 2, לתיקיית הסקילים של הפרויקט | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/build-my-system.zip) |
| [`keep-my-data`](skills/keep-my-data/SKILL.md) | **הוחלף** ב-`backup-and-keep-alive`. לא מתקינים אותו | המשימה אחרי מפגש 2 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/keep-my-data.zip) |
| [`accessibility`](skills/accessibility/SKILL.md) | נגישות לפי החוק בישראל (תקן 5568): שואל מי משתמשת במערכת, ממליץ על רמת הנגשה, בודק ומתקן את המסכים, ובונה ב-React רכיב נגישות מותאם ודף הצהרת נגישות. לא ייעוץ משפטי | מפגש 3 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/accessibility.zip) |
| [`about-page`](skills/about-page/SKILL.md) | דף אודות למערכת: של מי היא, מה היא עושה ואיך יוצרים קשר. שואל כמה שאלות קצרות, מראה טיוטה, ובונה דף שנפתח בכתובת `/about` בלי כניסה. זה דף הבית שגוגל מבקשת | מפגש 4 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/about-page.zip) |
| [`legal-pages`](skills/legal-pages/SKILL.md) | מדיניות פרטיות ותנאי שימוש למערכת, בכתובות `/privacy` ו-`/terms`, שנפתחות בלי כניסה, והודעת עוגיות לפי מה שהמערכת שומרת בדפדפן. שואל רק מה שחסר, מראה טיוטה, ובונה. גוגל דורשת את שני הדפים לפני שמפרסמים אפליקציה | מפגש 4 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/legal-pages.zip) |
| [`backup-and-keep-alive`](skills/backup-and-keep-alive/SKILL.md) | גיבוי מוצפן לדרייב בכל יום, ופרויקט Supabase החינמי שלא נרדם. שני שלבים, ושתי פעולות ב-GitHub: Keep Supabase Alive ו-Daily DB Backup. ביניהם הכנה בגוגל: אפליקציה מפורסמת ב-Google Cloud. מחליף את keep-my-data | מפגש 4 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/backup-and-keep-alive.zip) |
| [`seo`](skills/seo/SKILL.md) | רושם את המערכת בגוגל, ומכין לגוגל ולמנועי הבינה רק את הדפים הציבוריים: כותרת ותיאור לכל דף, robots.txt, מפת אתר ו-llms.txt, וכל המסכים הפנימיים מסומנים "לא לחיפוש". אחר כך רישום ב-Search Console, בקשה להוסיף את דף האודות, וייבוא ל-Bing | מפגש 4 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/seo.zip) |

## איך מתקינים Skill

קודם קוראות אותו: לוחצות על השם בטבלה וקוראות את הקובץ. Skill הוא הוראות שהבינה מבצעת, ולכן לא מתקינים Skill בלי לקרוא אותו.

**ב-Claude Code**, בתיקיית הפרויקט שלכן, כותבות (ומחליפות את השם בשם ה-Skill):

> תתקין לי את הסקיל plan-my-system מהמאגר https://github.com/ruthprissman/ai-dev-course לתיקיית הסקילים האישית שלי. קודם תקרא את הקבצים שלו, ותגיד לי בקצרה מה הוא עושה. לפני שאתה מעתיק, תחכה לאישור שלי.

את `build-my-system` מתקינות לתיקיית הסקילים של הפרויקט (`.claude/skills`), ולא לתיקייה האישית, כדי שיישמר עם הפרויקט בגרסאות. הבקשה המלאה נמצאת בדף הפרומפטים של מפגש 2 (P-02).

אחרי ההתקנה פותחות שיחה חדשה, וכותבות את שם ה-Skill אחרי לוכסן, למשל `/plan-my-system`, או פשוט מבקשות: "אני רוצה לתכנן את המערכת שאני בונה לעסק [שם העסק]".

**באתר של Claude**: מורידות את קובץ ה-ZIP מהטבלה, ומעלות אותו כמו שהוא ב-Customize › Skills.

## דוגמאות

- [`examples/tik-chodshi/idea.md`](examples/tik-chodshi/idea.md): האפיון של "תיק חודשי", מערכת למנהלת חשבונות שאוספת מסמכים מהלקוחות שלה. כל הנתונים בה מומצאים.
- [`skills/plan-my-system/example.md`](skills/plan-my-system/example.md): תכנון מלא של "אופק", CRM לעסק בדוי של ייעוץ וליווי לעסקים. זו הדוגמה שמלווה את הקורס.
