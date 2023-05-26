# gse_nl


zowe samples:

zowe zos-jobs submit local-file "MARBDB2.jcl" --vasc
zowe db2 execute sql -q "SELECT * FROM EVENT.MARBLE" --rfj
zowe db2 execute sql -q "SELECT * FROM EVENT.COLOR" --rfj > color.json  

zowe  fmp populate ds roddi01.lib.data -m test1 --lds roddi01.lib.copy --lm marbles --data ./data/marbles.json

HB
TRAD
curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/gse_ned_trad > trad1.txt 
curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/gse_ned_tradjson?companies=1,2,3,4 > trad2.json 

zowe files list ds "roddi01.git.*" 
zowe files list ds "roddi01.git.*" -a --rfj 


More samples:
zowe zos-files compare data-set "roddi01.git.rexx3(ll01qa)" "roddi01.git.rexx3(ll01qa2)" > test.rexx --bv
zowe files rename ds RODDI01.GIT.REXX1 RODDI01.GIT.REXX0 

