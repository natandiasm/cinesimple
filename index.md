## Cine Simple

Player de video para um link passado por get

### Player

<video id="video" width="320" height="240" controls>
</video>


<script>
function getUrlVars() {
    var vars = {};
    var parts = window.location.href.replace(/[?&]+([^=&]+)=([^&]*)/gi, function(m,key,value) {
        vars[key] = value;
    });
    return vars;
}
    
let video = document.getElementById('video');
let source = document.createElement('source');

source.setAttribute('src', getUrlVars()["mp4"]);

video.appendChild(source);
video.play();
</script>
