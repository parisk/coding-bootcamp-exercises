---
layout: exercise_js
title: "DOM: Modifying HTML elements"
category: javascript
---

Modify the `src` attribute of the `img` element with id `avatar` to `https://github.com/parisk.png`.

<div id="parent" style="padding: 8px; background-color: #f5f5f5;">
  <img id="avatar" style="width: 100px; height: 100px;" src="https://github.com/akalipetis.png" alt="avatar" />
  ← This is the avatar.
</div>

<script>
    function evaluator() {
      var avatar = document.getElementById('avatar');
      if (avatar.src != 'https://github.com/parisk.png') {
        return (
          'The `src` attribute of the avatar was expected to be' +
          '<code>https://github.com/parisk.png</code>, but it is ' +
          '<code>' + avatar.src + '</code>.'
        ) ;
      }
    };
</script>
