# Buffalo YOLOL Defaults
### 10 basic chips, 1 advanced, 1 memory chip
In top-down order, counting down left rack first...

Basic Chip #1 (alarm for propellant):
```basic
alarm=0 IF :AlarmOveride==1 THEN goto1 ELSE goto2 END
IF :Propellant<500 THEN alarm=1 ELSE alarm=0 goto1 END
IF alarm==1 THEN :RedLight=1 :SndT=6 :SoundOn=1 ELSE :RedLight=0 END

//-- blank lines until line 8 --

IF alarm==1 THEN :RedLight=0 ELSE :RedLight=0 END

//-- blank lines until line 13 --

IF alarm==1 THEN :RedLight=1 ELSE :RedLight=0 END

//-- blank lines until line 18 --

IF alarm==1 THEN :RedLight=0 ELSE :RedLight=0 END goto1
```

Basic Chip #2 (alarm for fuel rods):
```basic
alarm=0 IF :AlarmOveride==1 THEN goto1 ELSE goto2 END
IF :FuelCheck<500 THEN alarm=1 ELSE alarm=0 goto1 END
IF alarm==1 THEN :RedLight=1 :SndT=6 :SoundOn=1 ELSE :RedLight=0 END

//-- blank lines until line 8 --

IF alarm==1 THEN :RedLight=0 ELSE :RedLight=0 END

//-- blank lines until line 13 --

IF alarm==1 THEN :RedLight=1 ELSE :RedLight=0 END

//-- blank lines until line 18 --

IF alarm==1 THEN :RedLight=0 ELSE :RedLight=0 END goto1
```

Basic Chip #3 (mining laser):
```basic
:CTP01=-7 :CTP02=-7 :LTP01=-7  :LTP02=-7 :LTP03=-7 :LTR01=-5.2
:LTR02=5.2
IF :M_Laser==1 THEN goto4 ELSE goto5 END
:MiningLaser=1 goto3
:MiningLaser=0 goto3
```
Basic Chip #4 (transponder/safe zone check):
```basic
:TRANSPONDER_B=1 :SAFEZONE_B=1 :LFI_Check=1 :LFO_Check=1
:RFI_Check=1 :RFO_Check=1 goto1
```

Basic Chip #5 (open doors if battery low):
```basic
IF :Battery < 3000 THEN goto20 ELSE goto2 END
IF :R_Door==1 OR :L_Door==1 THEN goto3 ELSE goto1 END

//-- blank lines until line 19 --

:R_Door=0 :L_Door=0 goto1
:R_Door=1 :L_Door=1 :ENGDoor=1 goto1
```

Basic Chip #6 (flow control indicator lights):
```basic
IF :Left_Flow_IN==1 THEN :LFI_Colour=2 ELSE :LFI_Colour=1 END
IF :Left_Flow_OUT==1 THEN :LFO_Colour=2 ELSE :LFO_Colour=1 END
IF :Right_Flow_IN==1 THEN :RFI_Colour=2 ELSE :RFI_Colour=1 END
IF :Right_Flow_OUT==1 THEN :RFO_Colour=2 ELSE :RFO_Colour=1 END goto1
```
Basic Chip #7 (material scanner):
```basic
:i=0 n="\n"
:scn=n+:m :scn+=n+:v :i=1 :scn+=n+:m :scn+=n+:v
:i=0 IF :Scanner==1 THEN :Scan=1 END GOTO2
```

Basic Chip #8 (transponder/safe zone indicator lights):
```basic
if :insideSafeZone==1 then :Safe_C=2 else :Safe_C=1 end
if :transponder==1 then :Tran_C=1 else :Tran_C=2 end goto1
```

Basic Chip #9 (automated generator):
```basic
:FuelChamberUnitRateLimit = 1000- :Battery/10 goto1
```

Basic Chip #10 (exterior lighting):
```basic
IF :Nav_Lights ==1 then goto2 else goto1 end
:NavRed =1 :NavGreen =1

//-- blank lines until line 12 --

:NavRed =0 :NavGreen =0
```

<p>Advanced Chip + Memory Chip (ISAN navigation): <br/>
-- no longer works -- <br/>
Update Video: https://www.youtube.com/watch?v=xuLfWdVrRfk <br/>
PDF Doc: https://isan.to/isan.pdf</p>
