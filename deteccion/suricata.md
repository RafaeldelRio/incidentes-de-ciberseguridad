# Suricata

sudo add-apt-repository ppa:iosf/suricata-stable

sudo apt install suricata

sudo nano /etc/suricata/suricata.yaml

community-id: false a true

ip -p -j route show default

cambiar en /etc/suricata/suricata.yaml --> af-packet --> interface por la interfaz de red usada

```
detect-engine:
  -  rule-reload: true
```

pidof suricata --> sudo kill -usr2 \<pid-suricata>

sudo suricata-update

sudo suricata-update list-sources

sudo suricata-update enable-source et/open

sudo suricata -T -c /etc/suricata/suricata.yaml -v

curl http://testmynids.org/uid/index.html

grep 2100498 /var/log/suricata/fast.log

cat /var/log/suricata/eve.log
