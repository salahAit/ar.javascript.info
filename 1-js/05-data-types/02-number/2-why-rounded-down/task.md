الأهمية: 4

---

#  لماذا ‎6.35.toFixed(1) == 6.3؟


تُدَوِّر كلًا من `Math.round` و `toFixed` العدد إلى أقرب عدد له وفقًا للتوثيق: الأجزاء من `0..4` تُدَوَّر للأسفل، بينما الأجزاء `5..9` تثدَوَّر للأعلى.

مثلًا:


```js run
alert( 1.35.toFixed(1) ); // 1.4
```

في المثال المشابه  أدناه، لِمَ تُدَوَّر `6.35` إلى `6.3`، وليس `6.4`؟

```js run
alert( 6.35.toFixed(1) ); // 6.3
```

كيف نُدَوِّر `6.35` بالطريقة الصحيحة؟

