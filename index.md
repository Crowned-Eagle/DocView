<html>
<head>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body {
  font-family: Arial;
}

* {
  box-sizing: border-box;
}

.openBtn {
  background: #0080FF;
  border: none;
  padding: 10px 15px;
  position: relative;
  left: 0%;
  font-size: 16px;
  cursor: pointer;
}

.openBtn:hover {
  background: #ff0000;
}

.overlay {
  height: 20%;
  width: 100%;
  display: none;
  position: fixed;
  z-index: 1;
  top: 30%;
  left: 0;
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0, 0.9);
}

.overlay-content {
  position: relative;
  top: 46%;
  width: 80%;
  text-align: center;
  margin-top: 30px;
  margin: auto;
}

.overlay .closebtn {
  position: absolute;
  top: 20px;
  right: 45px;
  font-size: 60px;
  cursor: pointer;
  color: white;
}

.overlay .closebtn:hover {
  color: #ccc;
}

.overlay input[type=text] {
  padding: 15px;
  font-size: 16px;
  border: none;
  float: left;
  width: 80%;
  background: white;
}

.overlay input[type=text]:hover {
  background: #f1f1f1;
}

.overlay button {
  float: right;
  width: 20%;
  padding: 5px;
  background: #ff0000;
  font-size: 14px;
  border: none;
  cursor: pointer;
}

.overlay button:hover {
  background: #bbb;
}     

</style>
</head>
<body>



<div id="myOverlay" class="overlay">
  <span class="closebtn" onclick="closeSearch()" title="Close Overlay">×</span>
  <div class="overlay-content">
    <form action=https://docs.google.com/viewer? method="get">
      <div>
        <textarea name="url" cols="50" rows="1"></textarea>
        <button>Open PDF</button>
      </div>        
    </form>
  </div>
</div>

<h2 style="text-align:left">PDFview v0.1</h2>
<button class="openBtn" onclick="openSearch()">Open PDF in Firefox..</button>

<script>
function openSearch() {
  document.getElementById("myOverlay").style.display = "block";
}

function closeSearch() {
  document.getElementById("myOverlay").style.display = "none";
}
</script>
     
</body>
</html>
