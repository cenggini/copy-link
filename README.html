<button id="copy-link-btn">Copy link</button>
<div id="copy-link-wrapper" class="copy-link-wrapper">
  <h2>Copy link</h2>
  <p>Press Ctrl / CMD + C to copy this to your clipboard.</p>
  <input readonly="readonly" type="text" value='' />
</div>
<div id="overlay" class="overlay"></div>

html, body {
  height: 100%;
}

html {
  font-size: 1em;
  line-height: 1.4;
}

body {
  background-color: #FFBC81;
  font-family: helvetica, arial, sans-serif;
}

*, *:before, *:after {
  -moz-box-sizing: border-box; -webkit-box-sizing: border-box; box-sizing: border-box;
 }

button {
  position: relative;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
  font-size: 1em;
  padding: 1em 2em;
  border: none;
  background-color: #3d83d6;
  color: #fff;
  font-weight: 700;
  border-bottom: 2px solid transparent;
  border-top: 2px solid transparent;
  outline: 0;
  cursor: pointer;
  &:hover {
    border-bottom-color: darken(#3d83d6, 20);
  }
  &:active {
    border-top-color: darken(#3d83d6, 20);
    border-bottom-color: transparent;
  }
}

.overlay {
  position: fixed;
  z-index: 100;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0,0,0,0.10);
  visibility: hidden;
  opacity: 0;
  transition: opacity 0.2s ease;
  .active & {
    visibility: visible;
    opacity: 1;
  }
}

.copy-link-wrapper {
  z-index: 200;
  padding: 2em;
  position: fixed;
  top: 50%;
  left: 50%;
  width: 50%;
  max-width: 500px;
  min-width: 300px;
  background-color: #fff;
  border-radius: 2px;
  transform: translateX(-50%) translateY(-50%);
  opacity: 0;
  transition: opacity 0.2s ease;
	clip:rect(1px 1px 1px 1px);
	opacity: 0;
	top: -9999999px;
	left: -9999999px;
  .active & {
    clip: auto;
	  opacity: 1;
	  top: 50%;
	  left: 50%;
  }
  h2 {
    margin: 0;
    margin-bottom: 1em;
  }
  p {
    margin-bottom: 1em;
  }
  input {
    background-color: #f3f3f3;
    color: #454545;
    border: 0;
    font-size: 1em;
    padding: 1em;
    margin: 0;
    width: 100%;
    border-radius: 2px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .error {
    text-align: center;
    color: #E7483B;
    display: block;
    padding: 0.5em;
  }
}

(function() {
  var copylinkbtn = document.getElementById("copy-link-btn"),
      copylink = document.getElementById("copy-link-wrapper"),
      overlay = document.getElementById("overlay");

  copylinkbtn.addEventListener("click", function() {
    
    var error = document.getElementsByClassName('error');
      
    while (error[0]) {
      error[0].parentNode.removeChild(error[0]);
    }

    document.body.className += ' active';
    
    copylink.children[2].value = window.location.href;
    copylink.children[2].focus();
    copylink.children[2].select();
  }, false);

  overlay.addEventListener("click", function() {
    document.body.className = '';
  }, false);

  copylink.children[2].addEventListener("keydown", function(e) {

    var error = document.getElementsByClassName('error');

    while (error[0]) {
      error[0].parentNode.removeChild(error[0]);
    }

    setTimeout(function() {

      if((e.metaKey || e.ctrlKey) && e.keyCode === 67 && isTextSelected(copylink.children[2])) {
        document.body.className = '';
      } else if((e.metaKey || e.ctrlKey) && e.keyCode === 67 && isTextSelected(copylink.children[2]) === false) {
        var error = document.createElement('span');
        error.className = 'error';
        var errortext = document.createTextNode('The link was not copied, make sure the entire text is selected.');
        
        error.appendChild(errortext);
        copylink.appendChild(error);
      }
    }, 100);

    function isTextSelected(input) {
      if (typeof input.selectionStart == "number") {
        return input.selectionStart == 0 && input.selectionEnd == input.value.length;
      } else if (typeof document.selection != "undefined") {
        input.focus();
        return document.selection.createRange().text == input.value;
      }
    }
  }, false);
})();
