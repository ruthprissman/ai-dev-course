# קורס פיתוח בעזרת AI

ה-Skills והדוגמאות של הקורס, מאת רות פריסמן ([Clearלי](https://aiclearlyapp.com)).
המאגר מתעדכן לאורך הקורס.

## Skills

| Skill | מה הוא עושה | מתי | ZIP |
|---|---|---|---|
| [`idea-analysis`](skills/idea-analysis/SKILL.md) | מראיין אתכן על הרעיון לפרויקט, שאלה אחת בכל פעם, וכותב אפיון של עמוד אחד ב-`docs/idea.md` | ההכנה לקורס | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/idea-analysis.zip) |
| [`plan-my-system`](skills/plan-my-system/SKILL.md) | קורא את הטקסט שכתבתן על העסק, בתיקייה שבה אתן עובדות, ומראיין אתכן בתשעה שלבים לתכנון המערכת. שומר הכול ב-`תכנון המערכת.md` | אחרי מפגש 1 | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/plan-my-system.zip) |
| [`build-my-system`](skills/build-my-system/SKILL.md) | סקיל המערכת שלנו: מלווה את הפרויקט וגדל בכל מפגש. היום: עובד לפי התכנון, משרטט אפיון ויזואלי של כל המסכים בקובץ HTML אחד (בודק איתך, מציע תוכנית, ורק אז כותב), ושומר גרסאות ב-GitHub | מפגש 2, לתיקיית הסקילים של הפרויקט | [הורדה](https://github.com/ruthprissman/ai-dev-course/raw/main/zip/build-my-system.zip) |

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
