### smoke.js
---
https://github.com/bijection/smoke.js?utm_source=recordnotfound.com

```js
var ctx = canvas.getContext('2d')
var party = smokemachine(ctx)
party.addsmoke(500,500)
party.start()

var party = smokemachine(context, [1,5,253])
```

```
<canvas id="canvas"></canvas>
<script src="smoke.js"></script>
<script>
  var canvas = document.getElementById('canvas')
  var ctx = canvas.getContext('2d')
  canvas.width = 1000
  canvas.height = 1000
  var party = smokemachine(ctx, [54, 16.8, 18.2])
  party.start()
  party.addsmoke(500,500,10)
  setTimeout(function(){
    party.stop()
    party.addsmoke(600,500,100)
    party.addsmoke(500,600,20)
    for(var i = 0; i< 10; i++){
      party.step(10)
    }
    setTimeout(function(){
      party.start()
    },1000)
  },1000)
</script>
```

```
```

