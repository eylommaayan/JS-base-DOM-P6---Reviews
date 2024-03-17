JS


קוד JavaScript זה מגדיר פונקציונליות להצגת רשימה של ביקורות, ומאפשר למשתמשים לנווט בהן באמצעות לחצנים קודמים, הבאים ואקראיים. תן לי לפרק את זה:

Reviews Data
1. **נתוני ביקורות**: מערך שנקרא `ביקורות` מכיל אובייקטים, שכל אחד מהם מייצג סקירה עם מאפיינים כמו `מזהה`, `שם`, `עבודה`, `img` ו`טקסט`. נתונים אלה מספקים מידע על אנשים שונים והביקורות שלהם.

Selecting Elements
2. **בחירת אלמנטים**: הקוד בוחר רכיבי HTML שונים באמצעות שיטות `document.getElementById()` ו-`document.querySelector()`. רכיבים אלה כוללים תמונה (`img`), שם המחבר (`מחבר`), שם תפקיד (`עבודה`) וטקסט סקירה (`מידע`). זה גם בוחר לחצנים לניווט: הקודם (`prevBtn`), הבא (`nextBtn`), ואקראי (`randomBtn`).


Starting Item
3. **פריט התחלה**: המשתנה `currentItem` מוגדר ל-0 בהתחלה, המציין את האינדקס של הסקירה הנוכחית המוצגת.


Loading Initial Item

4. **טעינת פריט ראשוני**: כאשר תוכן ה-DOM נטען (אירוע `DOMContentLoaded`), הקוד מציג את הסקירה המתאימה לאינדקס `currentItem` על ידי הגדרת הערכים המתאימים לרכיבי HTML שנבחרו.


Function to Show Person

5. **פונקציה להצגת אדם**: הפונקציה `showPerson()` לוקחת אינדקס כארגומנט ומעדכנת את הסקירה המוצגת על סמך אותו אינדקס.


Event Listeners
6. **מאזיני אירועים**: מאזיני אירועים מתווספים ללחצנים הבאים, הקודמים והאקראיים. כאשר לוחצים עליהם, כפתורים אלה מפעילים פונקציות להצגת הסקירה הבאה, הקודמת או הסקירה האקראית, בהתאמה.

Next and Previous Button Functions
7. **פונקציות הלחצן הבא והקודם**: פונקציות אלו מגדילות או מקטינות את אינדקס ה-'currentItem' ומבטיחות שהוא יישאר בגבולות אורך מערך ה-'ביקורות'.


Random Button Function
8. **פונקציית לחצן אקראית**: פונקציה זו מייצרת אינדקס אקראי בטווח של אורך מערך `ביקורות` ומציגה את הסקירה המתאימה לאינדקס זה באמצעות הפונקציה `showPerson()`.

בסך הכל, קוד זה יוצר קרוסלת ביקורות פשוטה המאפשרת למשתמשים לנווט בין ביקורות ברצף או אקראי.