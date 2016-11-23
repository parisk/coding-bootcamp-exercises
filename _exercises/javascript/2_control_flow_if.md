---
layout: exercise_js
title: Control flow (if statements)
category: javascript
---

You are provided with two variables (**you don't have to declare them**):

- A number: `n` (you can control it's value using the input below)
- A boolean: `isZero`

If the value of `n` equals `0`, then assign the value `true` to `isZero`.

If the value of `n` **does not equal** `0`, then assign the value `false` to `isZero`.

<div class="form-group">
    <label for="i">Value of <code>n</code></label>
    <input class="form-control" type="number" id="i" value="5">
</div>

<script>
    var i = document.getElementById('i');
    var preparator = 'var n = parseInt(i.value); var isZero;'

    function evaluator() {
      var shouldBeZero = (n == 0);
      if (shouldBeZero != isZero) {
          return (
            '<code>isZero</code> should be <code>' + shouldBeZero + '</code>, ' +
            'but it is <code>' + isZero + '</code>.'
          )
      }
    };
</script>
