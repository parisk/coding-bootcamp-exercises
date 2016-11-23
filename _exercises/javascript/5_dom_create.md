---
layout: exercise_js
title: "DOM: Creating HTML elements"
category: javascript
---

Create a `<p></p>` element and append it to the element with id `parent`.

<div id="parent" style="padding: 8px; background-color: #f5f5f5;">I am the parent.</div>

<script>
    function preparator() {
      document.getElementById('parent').textContent = 'I am the parent.';
    }

    function evaluator() {
      if (!document.getElementById('parent').querySelectorAll('p').length) {
        return 'You did not append a <code>p</code> element into parent!';
      }
    };
</script>
