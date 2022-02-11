<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap');

html, body, form{
  height: 100%;
  display: flex;
  align-items: center;
  justify-content:center;
  flex-direction: column;
  font-family: 'Roboto', sans-serif;
  background-color: #111111;
  color:white;
    text-align: center;
  vetical-align: center;
  font-size: 20px;
}

input[type="text"]{
  outline: none;
  width: 512px;background-color: #222222;
  border-radius:15px;
  border: none;
  color: white;
  padding: 10px 15px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}

input[type="submit"]{
background-color: #222222;
  margin-top: 1rem;
  border-radius:15px;
  border: none;
  color: white;
  padding: 10px 15px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}

.footer {
   position: fixed;
   left: 0;
   bottom: 0;
   width: 100%;
   background-color: #222222;
   color: white;
   text-align: center;
   padding: 3px;
}
</style>
  
<form onsubmit="unblock()">
  <h1>Website Unblocker</h1>
  <input id="input" type="text">
  <input type="submit" value="Unblock"></input>
  </input>
</form>
<div class="footer">
  <span>© 2021 Shane Paton</span>
</div>

<script defer>
  function unblock(){
  let url = document.getElementById("input").value
    console.log(url)
  var win = window.open("https://translate.google.com/translate?sl=auto&tl=en&u=" + url, '_blank');
  win.focus();
  console.log(window.location)
  }
</script>

