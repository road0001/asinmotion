
```
import com.asinmotion.effects.*;
import com.asinmotion.easing.*;

//ease defaults to Linear.easeNone
//time defaults to 1000 (in milliseconds)
//either set a start and end position
var efkt:Effect = new Effect({target:box, start_x:100, end_x:150, ease:Sine.easeOut, time: 1000});
ekft.run();

//or just the end postion
var efkt2:Effect = new Effect({target:box, scaleX:1.5, ease:Sine.easeOut, time: 1000});
ekft2.run();


//both queue and parallel work the same
var list:Queue = new Queue();
list.addEffect({target:box, scaleX:1.5})
list.addEffect({target:box, x:300})
list.addEffect({target:box, y:200})
list.start();
```
