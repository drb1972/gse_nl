# gse_nl


zowe samples:

zowe zos-jobs submit local-file "MARBDB2.jcl" --vasc
zowe db2 execute sql -q "SELECT * FROM EVENT.MARBLE" --rfj 
zowe db2 execute sql -q "SELECT * FROM EVENT.COLOR" --rfj > color.json  

HB
curl http://mstrsvw.lvn.broadcom.net:8000/hbscript/demo_orange?companies=1,2,3,4 > test.json 

More samples:
zowe zos-files compare data-set "roddi01.git.rexx3(ll01qa)" "roddi01.git.rexx3(ll01qa2)" > test.rexx --bv
