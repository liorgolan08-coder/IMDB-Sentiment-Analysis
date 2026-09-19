# ניתוח סנטימנט של ביקורות סרטים ב-IMDB

## תיאור הפרויקט

העבודה עוסקת בניתוח סנטימנט של ביקורות סרטים מתוך IMDB.

מטרת העבודה היא לבנות מודל של למידת מכונה שמקבל טקסט של ביקורת ומסווג אותה לפי עמודת `label`.

תהליך העבודה כולל טעינת הנתונים, בדיקתם, עיבוד מקדים של הטקסט, המרת הטקסט לייצוג מספרי באמצעות TF-IDF, אימון מודל Logistic Regression, בדיקת שילובים שונים של פרמטרים והערכת ביצועי המודל באמצעות Macro F1.

---

## Dataset

מאגר הנתונים שנבחר לעבודה הוא:

**IMDB Movie Ratings Sentiment Analysis**

ה-Dataset נלקח מ-Kaggle.

הוא כולל שתי עמודות:
- `text` – טקסט ביקורת הסרט
- `label` – המחלקה המתאימה לביקורת

הקובץ `movie.csv` אינו מצורף ל-Repository בגלל גודלו.

ניתן להוריד את ה-Dataset דרך Kaggle בקישור הבא:

**Kaggle:**  
[[https://www.kaggle.com/datasets/yasserh/imdb-movie-ratings-sentiment-analysis]
לאחר הורדת הקובץ יש למקם את `movie.csv` באותה תיקייה שבה נמצאת מחברת ה-Jupyter Notebook.

---

## תהליך העבודה

העבודה כוללת את השלבים הבאים:

- טעינת הנתונים ובדיקת מבנה ה-Dataset
- בדיקת ערכים חסרים ורשומות כפולות
- בדיקת התפלגות המחלקות
- חלוקה ל-Train ו-Test
- ניקוי ועיבוד מקדים של הטקסט
- המרת הטקסט לייצוג מספרי באמצעות TF-IDF
- שימוש ב-n-grams
- אימון מודל Logistic Regression
- יצירת מודל Baseline
- בדיקת Hyperparameters באמצעות Grid Search
- שימוש ב-5-Fold Cross Validation
- הערכת ביצועי המודל באמצעות Macro F1
- הצגת Classification Report
- הצגת Confusion Matrix
- ניתוח המאפיינים שהשפיעו על המודל

---

## תוצאות

תוצאת מודל ה-Baseline:

**Macro F1: 0.8861**

התוצאה הטובה ביותר ב-Cross Validation:

**Macro F1: 0.8924**

התוצאה הסופית על קבוצת ה-Test:

**Macro F1: 0.8937**

---

## קבצים ב-Repository

### `IMDB_Sentiment_Assignment_final.ipynb`

מחברת Jupyter Notebook הכוללת את המימוש המלא של העבודה, ההסברים, הקוד, תוצאות ההרצה והערכת ביצועי המודל.

### `README.md`

קובץ זה, הכולל הסבר קצר על העבודה, ה-Dataset והקישורים הרלוונטיים.

---

## סרטון הצגת העבודה

סרטון הצגת העבודה זמין לצפייה בקישור הבא:

**YouTube:**  
[https://youtu.be/eeT5X4HZCns]

---

## מגישים

- ליאור ג.
- מור ע.
- דניאל א.
- גל י.
