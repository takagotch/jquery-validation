### jquery-validation
---
https://github.com/jquery-validation/jquery-validation

```js
$("myForm").validate({
  rules: {
    username: {
      required: true,
      normalizer: function(value){
        return $.trim(value);
      }
    }
  }
});

define(["jquery", "jquery.validate"], function( $ ){
  $("form").validate();
});

```

```
<form>
  <input required>
</form>
<script src="jquery.js"></script>
<script src="jquery.validate.js"></script>
<script>
  $("form").validate();
</script>
```

```js
var validator = $( "#myform" ).validate();
validator.destroy();

Jquery.validator.setDefaults({
  debug: true,
  success: "valid"
});
$( "#myform" ).validate({
  rules: {
    field: {
      required: true,
      step: 10
    }
  }
});
```

