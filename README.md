# subject-220704
```javascript
<script>
setTimeout(function() {
parent.document.location.hash = "%F0%9F%8F%A9%F0%9F%8C%99%F0%9F%9B%8F%F0%9F%92%91%F0%9F%92%A4%F0%9F%92%A4%F0%9F%92%A4";
}, 500);

setTimeout(function() {
parent.document.location.hash = "%F0%9F%8F%A9%F0%9F%8C%99%F0%9F%9B%8F%F0%9F%92%91"
}, 1000);
</script>
```

```javascript
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/EaselJS/1.0.2/easeljs.min.js"></script>

<script>

	$(function(){
		$("#end").on("click", function(){
			createjs.Ticker.reset();
			createjs.Ticker._timerId = null;
			createjs.Ticker._inited = false;

		});
	});

	// ***************************************
	// 繰り返しの登録
	// ***************************************
	createjs.Ticker.framerate = 1;
	createjs.Ticker.on("tick", loop_action );

	// ***************************************
	// ここがずっと呼ばれる
	// ***************************************
	function loop_action() {

		console.log("OK");

	}

</script>

<input type="button" id="end" value="終了">
```
