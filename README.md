# suricata-rule

bob suricata rule 과제

tls같은경우, handshake단계에서 나타나는 sni와 ip를 엮어서 후에는 ip를 이용해 탐지해보려고 했으나 어떻게 해야할지 모르겠어서 일단 handshake단계에 나타나는 평문 sni만 탐지하게 했다.

### 원래 의도
1. handshake에서 ip와 sni짝지어서 저장
2. 후에 사이트에 방문할 때의 ip와 저장된 ip, sni쌍 확인
3. ip, sni쌍이 존재하면 sni 출력

### 문제점
ip, sni쌍을 만드는 방법부터 모르겠다.
