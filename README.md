# lern-javascript
lerning javascript


## upload and preview

````
<input type='file' accept='image/*' onchange='openFile(event)'><br>
<img id='output'>

<script>
  var openFile = function(event) {
    var input = event.target;
    var reader = new FileReader();
    reader.onload = function(){
      var dataURL = reader.result;
      var output = document.getElementById('output');
      output.src = dataURL;
    };
    reader.readAsDataURL(input.files[0]);
  };
</script>
````

https://www.javascripture.com/FileReader
