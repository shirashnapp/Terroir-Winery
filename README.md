# Terroir

אתר תדמית וליד עבור Terroir - כרם בוטיק וחוויית שולחן אחד. אתר סטטי ב-HTML, CSS ו-JavaScript בלבד, ללא שלב build.

Brand site for Terroir, a boutique vineyard and single-table dining experience. A static site: plain HTML, CSS and JavaScript, no build step.

## מבנה

```
index.html   - כל האתר: עמודים, סגנונות וסקריפטים
assets/      - תמונות, סרטון, גופנים (Alef, LimonArak) ומסכות
```

## הרצה מקומית

```bash
python3 -m http.server 8080
# http://localhost:8080
```

פתיחה ישירה של `index.html` בדפדפן עובדת גם כן.

## פריסה ב-Vercel

1. ב-Vercel: Add New, Project, ובחירת המאגר הזה.
2. Framework Preset: **Other**. Build Command ו-Output Directory נשארים ריקים.
3. Root Directory: השורש של המאגר. Deploy.

## הערות

- דף הבית מנגן סרטון (`assets/vineyard-stages.mp4`, כ-3.7MB). בפריסה מומלץ להגיש קבצים סטטיים עם דחיסה וקאש, ש-Vercel עושה כברירת מחדל.
- שמירת בקשות הזמנה בפועל דורשת חיבור לשירות מייל או לשרת. בקוד יש הגדרה אחת לכך, `RESV_ENDPOINT` ב-`index.html`. כשהיא ריקה, הטופס פותח טיוטת מייל.
- לפני עלייה לאוויר: להוסיף `canonical`, תמונת שיתוף (`og:image`), ופרטי עסק בנתונים המובנים. הטקסטים המשפטיים הם תבנית וצריכים בדיקה משפטית.
