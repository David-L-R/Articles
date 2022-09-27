# 𝐂𝐥𝐞𝐚𝐧 𝐂𝐨𝐝𝐞 - 𝐇𝐨𝐰 𝐭𝐨 𝐍𝐚𝐦𝐞 𝐕𝐚𝐫𝐢𝐚𝐛𝐥𝐞𝐬 🧹

> 𝘛𝘩𝘦𝘳𝘦 𝘢𝘳𝘦 𝘰𝘯𝘭𝘺 𝘵𝘸𝘰 𝘩𝘢𝘳𝘥 𝘵𝘩𝘪𝘯𝘨𝘴 𝘪𝘯 𝘊𝘰𝘮𝘱𝘶𝘵𝘦𝘳 𝘚𝘤𝘪𝘦𝘯𝘤𝘦: [...] 𝘢𝘯𝘥 𝘯𝘢𝘮𝘪𝘯𝘨 𝘵𝘩𝘪𝘯𝘨𝘴.
> 𝘗𝘩𝘪𝘭 𝘒𝘢𝘳𝘭𝘵𝘰𝘯

If you have been coding for a while, you probably read this quote before. But it is true that naming things in programming is HARD!

How to name variables will take up a few posts, because there are many things to take into consideration.

But, for now, let's focus on the first tip:

## ❌ Avoid

Don't give a variable one letter. When writing code, d might be an obvious abbreviation for "day" but for another developer...

Trying to find a bug in your code or adding a feature, they will have to start looking around to understand it - what a waste of time!

```js
let d = 5;
```

## ✅ Better

Calling your variable "dayOfTheWeek" - which will represent "Sunday", "Monday", and so on...

But still not so good, is to give it a "magic number". When we write it, we might think that it is obvious that 5 is Friday (Sunday is 0), but how can another developer can be sure?!

We will talk about magic numbers and how to handle them. But here is one solution:

```js
// Now we know we are talking about which day of the week it is
// But it is still unclear what is 5 (is it Thursday or Friday?)
const dayOfTheWeek = 5;
```

## ⭐ Great!

Create a clear map of the days. Then, another developer that reads your code will basically read English:

"the day of the week, out of all days of the week, is Friday".

Beautiful.

```js
let weekDays = {
  sunday: 0,
  monday: 1,
  tuesday: 2,
  wednesday: 3,
  thursday: 4,
  friday: 5,
  saturday: 6,
};

let dayOfWeek = weekDays.friday;
```
