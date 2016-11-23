---
layout: exercise_js
title: "Syntax: Control flow (loops)"
category: javascript
---

You are provided with a variable named `counter` and value `0` (**you don't have to declare it**).

Create either a `for` or a `while` loop that will run **5 times** and will increment the value of `counter` by `1` during each step.

**The final value of `counter` should be `5`**.

<script>
    var i = document.getElementById('i');
    var preparator = 'var counter = 0;'

    function evaluator() {
      var usesLoop = false;
      var kw = editor.getWrapperElement().querySelectorAll('.cm-keyword');
      var loops = ['while', 'for'];

      for (var c=0; c<kw.length; c++) {
        if (loops.indexOf(kw[c].textContent) >= 0) {
          usesLoop = true;
          break;
        }
      }

      if (!usesLoop) {
        return 'You are not using a <code>for</code> or <code>while</code> loop!';
      }

      if (counter != 5) {
        return (
          'The value of <code>counter</code> was expected to be <code>5</code> ' +
          'but it is <code>' + counter + '</code>!'
        )
      }
    };
</script>
