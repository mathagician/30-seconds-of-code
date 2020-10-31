---
title: getNumberOfWeeks
tags: dateTime,beginner
---

Calculates number of weeks between two dates from the given dates.

- Use `Date.getTime()` to get time part from given date.
- Use `Substraction get time remaining`.
- Use `Divison by 24*3600*1000 milliseconds to get days`.


```js
const getNumberOfWeeks = (fromDate, toDate) => {
  return parseInt(((toDate.getTime() - fromDate.getTime()) / (24*3600*1000) / 7));
};
```

```js
getNumberOfWeeks(new Date('2020-10-19'), new Date('2021-06-19')); // 34
```