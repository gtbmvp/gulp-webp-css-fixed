# GULP-WEBP-CSS-FIXED

---

### FEATURES

- Comments inside CSS rules don't cause error;
- SVG extension excluded from iteration;

---

### Description

[gulp-webp-css](https://www.npmjs.com/package/gulp-webp-css) by seokirill doesn't have additional type check. It excludes comments between selectors from iteration by checking rule.type, but it doesn't check comments presence inside rules. Therefore in rules with comments, for example, string "`border: 1px solid black /* example */`" would have typeof **undefined** and iteration through searching substring in rule (`indexOf("background")/indexOf("url")/indexOf(".webp")`) leads to error.

Original repository of gulp-webp-css seems to be deleted, so i have to make my own package.

---

### Plan2do

- rule comments should not move to next line
