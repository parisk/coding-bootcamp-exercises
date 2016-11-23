---
layout: exercise_js
title: "Syntax: Functions"
category: javascript
---

Declare a function named `cube` that receives a single argument named `n` and returns `n³`.

The value of `n` can be controled using the input below.

<div class="form-group">
    <label for="i">Value of <code>n</code></label>
    <input class="form-control" type="number" id="i" value="5">
</div>

<script>
    var i = document.getElementById('i');
    var preparator = 'var n = parseInt(i.value);'

    function evaluator() {
      if (typeof cube == 'undefined') {
        return 'You did not declare a function named <code>cube</code>.';
      } else if (typeof cube != 'function') {
        return 'You declared <code>cube</code>, but it is not a function.'
      } else {
        var r = cube(n);
        var n3 = n*n*n;

        if (r != n3) {
          return (
            '<code>cube(' + n + ') was expected to return <code>' + n3 + '</code>, ' +
            'but it returned <code>' + r + '</code>!'
          )
        }
      }
    };
</script>
