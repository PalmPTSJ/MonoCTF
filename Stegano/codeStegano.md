# Code Stegano

You are inspecting chat messages between two programmers which you think that they are planning to do something.
The messages are mostly useless and have no meaning at all, except this piece of code.

```Javascript
var message,obfus,n,op,len,end,temp,sz,_1,p1,afterDel,yPos,_2,sub,obf2,merged,_finish

// Read here FIRST !
message = "The flag is "
obfus = "nopqrstuvwerehy"
n = 96
op = window.setInterval(function()
{
len = obfus.length
end = ""
temp = message
sz = temp.length
_1 = String.fromCharCode(n+len)
p1 = obfus.indexOf("ereh");
len = sz
afterDel = obfus.substr(0,14).replace("pqrstuvw","t");
yPos = obfus.indexOf("y");
_2 = String.fromCharCode(n+len)+_1
sub = obfus.substring(yPos-4,yPos)
obf2 = sub.split('').reverse().join('')
merged = afterDel.replace("ereh","")+'_'+obf2
end = merged+'_'+_2+'l'
_finish = temp + end
console.log(_finish)
temp = ""
for(var i = 0;i < 3;i++) console.log(".");
},3000);
```

This code seems to not has any meaning at all ... or not ?

(The flag format is mono{xxx})
