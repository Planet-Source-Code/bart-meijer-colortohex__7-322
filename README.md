<div align="center">

## ColorToHex


</div>

### Description

Converts a TColor to a HTML Hex value
 
### More Info
 
Inp: Tcolor

Nothing special...

A string containing the html color


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Bart Meijer](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/bart-meijer.md)
**Level**          |Beginner
**User Rating**    |3.9 (27 globes from 7 users)
**Compatibility**  |Delphi 5, Delphi 4, Pre Delphi 4
**Category**       |[Internet/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-html__7-34.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/bart-meijer-colortohex__7-322/archive/master.zip)

### API Declarations

Who cares?


### Source Code

```
function ColorToHex(Inp: TColor): String;
var
  tmp: Longint;
begin
  tmp:= ColorToRGB(inp);
  Result:= '#' + IntToHex(GetRValue(tmp),2) + IntToHex(GetGValue(tmp),2) + IntToHex(GetBValue(tmp),2);
end;
```

