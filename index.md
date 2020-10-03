<script>
function getUrlVars() {
    var vars = {};
    var parts = window.location.href.replace(/[?&]+([^=&]+)=([^&]*)/gi, function(m,key,value) {
        vars[key] = value;
    });
    return vars;
}
</script>
## Cine Simple

Player de video para um link passado por get

### Player

<video width="400" controls>
  <source src="<script>
document.write(getUrlVars()["mp4"]);
</script>" type="video/mp4">
  Your browser does not support HTML video.
</video>
