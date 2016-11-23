---
layout: exercise_js
title: "Syntax: Variables"
category: javascript
---

Create a variable with name `greeting` and value `Hello world!`.

<script>
    function evaluator() {
      if (typeof greeting == 'undefined') {
        return 'You did not create a variable called <code>greeting</code>.';
      } else if (greeting != 'Hello world!') {
        return (
          'The value of <code>greeting</code> is <code>' + greeting + '</code>' +
          'instead of <code>Hello world!</code>.');
      }
      return false;
    };
</script>
