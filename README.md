# test.bash
#!/bin/bash  　 ng () {       echo NG at Line $1       res=1 } 　 res=0 　  out=$(seq 5 | ./plus) [ "${out}" = 14 ] || ng ${LINENO} 　 [ "$res" = 0 ] &amp;&amp; echo OK exit $res
