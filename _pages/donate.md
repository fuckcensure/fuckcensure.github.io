---
title: "Donate"
permalink: "/donate"
image: assets/images/banner.png
---
- <font class="notranslate">Bitcoin (BTC): <a href="javascript:void(0);" onclick="dc_donate('Bitcoin (BTC)','bc1qlh3y5eclqt3gwgf64mpvf29klmc5n4ka3vrqkp');">bc1qlh3y5eclqt3gwgf64mpvf29klmc5n4ka3vrqkp</a></font>
- <font class="notranslate">Ethereum (ETH): <a href="javascript:void(0);" onclick="dc_donate('Ethereum (ETH)','0x4255eE58c6360b39C404601C2d74482A16F9cC29');">0x4255eE58c6360b39C404601C2d74482A16F9cC29</a></font>
- <font class="notranslate">Bitcoin Cash (BCH): <a href="javascript:void(0);" onclick="dc_donate('Bitcoin Cash (BCH)','qpg6qhlsqukymjydurvmdhmqyx6rm5u5ycglsdeauq');">qpg6qhlsqukymjydurvmdhmqyx6rm5u5ycglsdeauq</a></font>
- <font class="notranslate">Ripple (XRP): <a href="javascript:void(0);" onclick="dc_donate('Ripple (XRP)','rwpBCZEvRuZjWB2r1DidwZgPC9r512khRG');">rwpBCZEvRuZjWB2r1DidwZgPC9r512khRG</a></font>
- <font class="notranslate">Litecoin (LTC): <a href="javascript:void(0);" onclick="dc_donate('Litecoin (LTC)','ltc1q5rhawhg9vecgmvjr2ztc2at36ee8avwvmyptfa');">ltc1q5rhawhg9vecgmvjr2ztc2at36ee8avwvmyptfa</a></font>
- <font class="notranslate">Dash (DASH): <a href="javascript:void(0);" onclick="dc_donate('Dash (DASH)','XvSgnhy9MLhw7Av8JirTgvfYragqVKA6QA');">XvSgnhy9MLhw7Av8JirTgvfYragqVKA6QA</a></font>
- <font class="notranslate">Ethereum Classic (ETC): <a href="javascript:void(0);" onclick="dc_donate('Ethereum Classic (ETC)','0x4572e6E7DE8Fafa71e6F9C1486BAC243554d0510');">0x4572e6E7DE8Fafa71e6F9C1486BAC243554d0510</a></font>
- <font class="notranslate">Zcash (ZEC): <a href="javascript:void(0);" onclick="dc_donate('Zcash (ZEC)','t1L2gXFZAjjrTVBkcj7u1yy85tk7E9gZrbt');">t1L2gXFZAjjrTVBkcj7u1yy85tk7E9gZrbt</a></font>
- <font class="notranslate">Tezos (Pre-Launch) (XTZ): <a href="javascript:void(0);" onclick="dc_donate('Tezos (Pre-Launch) (XTZ)','tz1VeTQu7BjZv869rz3Zn22U8X7Hr8k9ahCM');">tz1VeTQu7BjZv869rz3Zn22U8X7Hr8k9ahCM</a></font>
- <font class="notranslate">OmiseGO (OMG): <a href="javascript:void(0);" onclick="dc_donate('OmiseGO (OMG)','0x4255eE58c6360b39C404601C2d74482A16F9cC29');">0x4255eE58c6360b39C404601C2d74482A16F9cC29</a></font>
- <font class="notranslate">Tether (USDT): <a href="javascript:void(0);" onclick="dc_donate('Tether (USDT)','0x4255eE58c6360b39C404601C2d74482A16F9cC29');">0x4255eE58c6360b39C404601C2d74482A16F9cC29</a></font>
- <font class="notranslate">Cardano (ADA): <a href="javascript:void(0);" onclick="dc_donate('Cardano (ADA)','0x4255eE58c6360b39C404601C2d74482A16F9cC29');">0x4255eE58c6360b39C404601C2d74482A16F9cC29</a></font>

<div id="dc_content" style="display: none">
	<div id="dc_overlay" style="position: fixed;top: 0;left: 0;width: 100%;height: 100%;background-color: #000;filter:alpha(opacity=50);-moz-opacity:0.5;-khtml-opacity: 0.5;opacity: 0.8;z-index: 10000;"></div>
	<div id="dc_overlaydiv" style="z-index:20000;padding:20px;height:70%;width:70%;border:1px solid #808080;background-color:#ffffff;position:absolute;left:0;right:0;top:0;bottom:0;margin:auto;max-width:100%;max-height:100%;overflow:auto;text-align:center;"><div id="dc_title" style="font-size:30px; border-bottom: 1px solid #e5e5e5;"></div><div id="dc_address" style="margin-top: 20px; font-size:16px; font-weight:bold;"></div><div><img id="dc_qr" style="height:60%; width:35%;" src="" ></div><div style="font-size:16px;"><a href="javascript:void(0);" onclick="dc_close();">close</a></div></div>
</div>
<script>
function dc_donate(currency,address){
	document.getElementById("dc_title").innerHTML = '<font class="notranslate">Donate&nbsp;'+ currency +'</font>';
	document.getElementById("dc_address").innerHTML = address;
	document.getElementById("dc_qr").src = 'https://chart.googleapis.com/chart?chs=512x512&cht=qr&chl=' + address;
   	document.getElementById('dc_content').style.display = 'block';
   	return false;
}
function dc_close(){
	document.getElementById('dc_content').style.display = 'none';
   	return false;
}
window.onkeyup = function (dc_event) {
  if (dc_event.keyCode == 27) {
	dc_close();
  }
}
</script>
