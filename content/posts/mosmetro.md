---
title: Московское метро
description: Схема транслитерации Московского метрополитена
slug: mosmetro
---

Схема транслитерации, которую использует Московский метрополитен. Визуально самая приятная из всех, хотя уступает Википедии по фонетической точности. Сочетает удачные решения [Википедии](/wikipedia) и [Яндекс.Карт](/yandex-maps). Придумана в Студии Лебедева, официально нигде не описана.

📅 2013 2.0 / 2019 4.0 • ✔️ действует • ⚪ без диакритики

Особенности:

-   Приятная `Щ` → `SCH`
-   Без апострофов для `Ъ` и `Ь`
-   Cхлопывает окончания на `-Й`

<div class="tabs">
<input name="tabs" type="radio" id="text" checked="checked" class="input"/>
<label for="text" class="label"><span>Текст</span></label>
<div class="panel pre-group">

<pre data-ref="source" contenteditable="true" class="editable"><code>Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю</code></pre>
<pre data-ref="target" data-schema="mosmetro"><code>Yuliya, syesh esche etikh myagkikh frantsuzskikh bulok iz Yoshkar-Oly, da vypey altayskogo chayu</code></pre>
</div>

<input name="tabs" type="radio" id="js" class="input"/>
<label for="js" class="label"><span>JavaScript</span></label>
<pre class="panel"><code>var source = "Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю";
var result = iuliia.translate(source, iuliia.MOSMETRO);</code></pre>

<input name="tabs" type="radio" id="python" class="input"/>
<label for="python" class="label"><span>Python</span></label>
<pre class="panel"><code>import iuliia
source = "Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю"
result = iuliia.translate(source, schema=iuliia.MOSMETRO)</code></pre>
</div>

## Правила

```
cyr  lat
а    a
б    b
в    v
г    g
д    d
е    e
ё    e,yo
ж    zh
з    z
и    i
й    y
к    k
л    l
м    m
н    n
о    o
п    p
р    r
с    s
т    t
у    u
ф    f
х    kh
ц    ts,s
ч    ch
ш    sh
щ    sch
ъ    —,y
ы    y
ь    —,y
э    e
ю    yu
я    ya
```

Буква `Ё` →

-   `YO` после `Ь` и `Ъ`;
-   `E` в остальных случаях.

Буква `Ц` →

-   `S` после `Т`;
-   `TS` в остальных случаях.

Буква `Ь` →

-   `Y` перед `A`, `Е`, `И`, `О`, `У`, `Э`;
-   опускается в остальных случаях.

Буква `Ъ` →

-   `Y` перед `A`, `Е`, `И`, `О`, `У`, `Э`;
-   опускается в остальных случаях.

Окончания:

-   `-ЫЙ` → `-Y`;
-   `-ИЙ` → `-Y`.

ℹ️ [artlebedev.ru](https://www.artlebedev.ru/metro/map4/)
