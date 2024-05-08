# Suricata

apt-get install software-properties-common iproute-2 nano curl

sudo apt install suricata

sudo nano /etc/suricata/suricata.yaml

community-id: false a true

ip a

cambiar en /etc/suricata/suricata.yaml --> af-packet --> interface por la interfaz de red usada

<pre><code>default-rule-path: /var/lib/suricata/rules
rule-files:
  - suricata.rules

<strong>
</strong><strong>detect-engine:
</strong>  -  rule-reload: true
</code></pre>

suricata-update

suricata-update list-sources

suricata-update enable-source et/open

suricata -T -c /etc/suricata/suricata.yaml -v

nano /etc/default/suricata --> cambiar a yes

curl http://testmynids.org/uid/index.html

grep 2100498 /var/log/suricata/fast.log

cat /var/log/suricata/eve.log
