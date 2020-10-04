---
title: "Contact"
image: assets/images/banner.png
permalink: "/contact-us"
---

Do you have a question or a suggestion?  
Please send your message to {{site.name}}. We will reply as soon as possible!  

Or you can contact us directly at : <mailto:chiisainakamoto@mail2tor.com>

<form action="javascript:void(0);" id="mailform">    
<div class="form-group row">
<div class="col-md-6">
<input class="form-control" type="text" id="pseudo" placeholder="Pseudo*" required>
</div>
<div class="col-md-6">
<input class="form-control" type="text" id="subject" placeholder="Subject*" required>
</div>
</div>
<textarea rows="8" class="form-control mb-3" id="message" placeholder="Message*" required></textarea>    
<button class="btn btn-success" onclick="mail();">Send</button>
</form>

<script>
var form = document.getElementById('mailform');
function mail() {
  if(form.checkValidity() != false) {
    var pseudo = document.getElementById("pseudo").value;
    var subject = document.getElementById("subject").value;
    var message = document.getElementById("message").value;
    location.href='mailto:chiisainakamoto@mail2tor.com?subject='+subject+'%20|%20By%20'+pseudo+'&body='+message+'%20|%20With%20https://fuckcensure.github.io';
  }
}
</script>
