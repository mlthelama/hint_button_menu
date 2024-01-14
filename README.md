File expects to be in \data\interface\ and expects the file buttonart.swf to be .\skyui\buttonart.swf relative to itself. This is the normal location for the file so should be fine 99% of the time.

Paths to the movieclips are:
```
main clip: _root.main
  LB Hint: _root.main.LB_Hint
    LB Hint Text: _root.main.LB_Hint.HintText
    LB Button Art: _root.main.LB_Hint.ButtonArt_MC
  RB Hint: _root.main.RB_Hint
    RB Hint Text: _root.main.RB_Hint.HintText
    RB Button Art: _root.main.RB_Hint.ButtonArt_MC
```
  The text for the hints is already setup to use a scaleform translation, which is implemented for all menu's using https://www.nexusmods.com/skyrimspecialedition/mods/22603

  Button art for the menu is stored as individual frames of buttonart.swf, so if you want to change the button art just change the frame the respective ButtonArt_MC clips are going to with gotoAndStop();
