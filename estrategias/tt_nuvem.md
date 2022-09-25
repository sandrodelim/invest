# TT_Nuvem

```
var
 MC, ML, MI : Float;

begin
  MC:= mediaexp(17, close);
  MI:= mediaexp(34, close);
  ML:= mediaexp(72, close);

  
  if( (MC > MI[1]) and (MC > ML[1]) and (MI > ML[1]) )then
    PaintBar(clGreen)
  else if( (MC < MI[1]) and (MC < ML[1]) and (MI < ML[1]) )then
    PaintBar(clRed)
  else 
    PaintBar(clGray);

  Plot(MC);
  Plot2(MI);
  Plot3(ML);

end;
```


