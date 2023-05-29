# gse_nl

zowe
----

zowe.cofig.json file

zowe files list ds "roddi01.lib.*" 

Zowe DB2 (video: zowe_db2)
--------
MARBDB2.jcl

zowe jobs submit local-file "MARBDB2.jcl" --vasc
zowe db2 execute sql -q "SELECT * FROM EVENT.MARBLE" 
zowe db2 execute sql -q "SELECT * FROM EVENT.MARBLE" --rfj
zowe db2 execute sql -q "SELECT * FROM EVENT.MARBLE" --rfj > marble.json  
zowe db2 execute sql -q "SELECT * FROM EVENT.COLOR" --rfj > color.json 


Zowe FMP (video: zowe_fmp)
--------
./data/marbles.json
zowe explorer: copy, data sets

zowe  fmp populate ds roddi01.lib.data -m marbles1 --lds roddi01.lib.copy --lm marbles --data ./data/marbles.json


HB (video: hb_total)
-- 
CICS MBS Maps

Eclipse:
http://mstrsvw.lvn.broadcom.net:8000/hbscript/helloworld 

TRAD

http://mstrsvw.lvn.broadcom.net:8000/hbscript/index.html  

curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/gse_ned_trad  
curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/gse_ned_tradjson?companies=1,2,3,4
curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/gse_ned_tradjson?companies=1,2,3,4 > trad.json 


More zowe

zowe files list ds "roddi01.git.*" 
zowe files list ds "roddi01.git.*" -a
zowe files list ds "roddi01.git.*" -a --rfj 
zowe files list am "roddi01.git.jcl" 
zowe files list am "roddi01.git.jcl" -a


More samples:
zowe zos-files compare data-set "roddi01.git.rexx3(ll01qa)" "roddi01.git.rexx3(ll01qa2)" > test.rexx --bv
zowe files rename ds RODDI01.GIT.REXX1 RODDI01.GIT.REXX0 

