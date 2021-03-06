---
id: bad87fee1348bd9aeda08826
title: Target Elements by id Using jQuery
required:
  - link: 'https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.2.0/animate.css'
challengeType: 6
videoUrl: ''
localeTitle: id的目标元素使用jQuery
---

## Description
<section id="description">您还可以通过其id属性来定位元素。首先使用<code>$(&quot;#target3&quot;)</code>选择器将您的<code>button</code>元素与id <code>target3</code> <code>$(&quot;#target3&quot;)</code> 。请注意，就像CSS声明一样，您在id的名称前键入<code>#</code> 。然后使用jQuery的<code>.addClass()</code>函数添加<code>animated</code>类和<code>fadeOut</code> 。以下是如何使用id <code>target6</code>淡出的<code>button</code>元素： <code>$(&quot;#target6&quot;).addClass(&quot;animated fadeOut&quot;)</code> 。 </section>

## Instructions
<section id="instructions">
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: 选择<code>id</code>为<code>target3</code>的<code>button</code>元素，并使用jQuery <code>addClass()</code>函数为它提供<code>animated</code>类。
    testString: 'assert($("#target3").hasClass("animated"), "Select the <code>button</code> element with the <code>id</code> of <code>target3</code> and use the jQuery <code>addClass&#40&#41</code> function to give it the class of <code>animated</code>.");'
  - text: 使用id <code>target3</code>定位元素，并使用jQuery <code>addClass()</code>函数为其提供类<code>fadeOut</code> 。
    testString: 'assert(($("#target3").hasClass("fadeOut") || $("#target3").hasClass("fadeout"))  && code.match(/\$\(\s*.#target3.\s*\)/g), "Target the element with the id <code>target3</code> and use the jQuery <code>addClass&#40&#41</code> function to give it the class <code>fadeOut</code>.");'
  - text: 只使用jQuery将这些类添加到元素中。
    testString: 'assert(!code.match(/class.*animated/g), "Only use jQuery to add these classes to the element.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
