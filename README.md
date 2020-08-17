# netfilter-test
실행 전, iptable 설정

sudo iptables -F

sudo iptables -A OUTPUT -j NFQUEUE --queue-num 0

sudo iptables -A INPUT -j NFQUEUE --queue-num 0

그 후,

make 후 sudo ./netfilter-test <host> (ex. sudo ./netfilter-test test.gilgil.net)
