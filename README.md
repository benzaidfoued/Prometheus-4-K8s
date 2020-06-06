See https://prometheus.io/docs/instrumenting/writing_exporters/#port-numbers for why this exists. Integrations other than exporters (e.g. adapters, webhooks) may also be listed here.

**Please look for open ports on this list (Ctrl+F "FREE") before adding a new port. Thanks!**

If you do not have a public repository with working code, please do not allocate a port. If a project is work-in-progress/WIP, please wait until you are ready to share it with others.

## Core components starting at 9090

| Port | Protocol | Component |
| ---- | -------- | --------- |
| 9090 | http | Prometheus server |
| 9091 | http | Pushgateway |
| 9092 | n/a | UNALLOCATED (to avoid collision with Kafka) |
| 9093 | http | Alertmanager |
| 9094 | ? | Alertmanager clustering |

## Exporters starting at 9100

| Port | Exporter |
| ---- | -------- |
| 9100 | [Node exporter](http://github.com/prometheus/node_exporter) |
| 9101 | [HAProxy exporter](http://github.com/prometheus/haproxy_exporter) (v2 has [native](https://github.com/prometheus/haproxy_exporter#official-prometheus-exporter) support) |
| 9102 | [StatsD exporter](http://github.com/prometheus/statsd_exporter): Metrics |
| 9103 | [Collectd exporter](http://github.com/prometheus/collectd_exporter) |
| 9104 | [MySQLd exporter](http://github.com/prometheus/mysqld_exporter) |
| 9105 | [Mesos exporter](http://github.com/mesosphere/mesos_exporter) |
| 9106 | [CloudWatch exporter](https://github.com/prometheus/cloudwatch_exporter) |
| 9107 | [Consul exporter](http://github.com/prometheus/consul_exporter) |
| 9108 | [Graphite exporter](http://github.com/prometheus/graphite_exporter): Metrics |
| 9109 | [Graphite exporter](http://github.com/prometheus/graphite_exporter): Ingestion |
| 9110 | [Blackbox exporter](https://github.com/prometheus/blackbox_exporter) |
| 9111 | [Expvar exporter](/docker-infra/expvar_exporter) |
| 9112 | [promacct: pcap-based network traffic accounting](https://github.com/kumina/promacct) |
| 9113 | [Nginx exporter](/discordianfish/nginx_exporter) [[alternative](/nginxinc/nginx-prometheus-exporter)] |
| 9114 | [Elasticsearch exporter](https://github.com/justwatchcom/elasticsearch_exporter) |
| 9115 | [Blackbox exporter](http://github.com/prometheus/blackbox_exporter) |
| 9116 | [SNMP exporter](http://github.com/prometheus/snmp_exporter) |
| 9117 | [Apache exporter](https://github.com/Lusitaniae/apache_exporter) |
| 9118 | [Jenkins exporter](https://github.com/RobustPerception/python_examples/tree/master/jenkins_exporter) |
| 9119 | [BIND exporter](https://github.com/digitalocean/bind_exporter) |
| 9120 | [PowerDNS exporter](https://github.com/janeczku/powerdns_exporter) |
| 9121 | [Redis exporter](https://github.com/oliver006/redis_exporter) |
| 9122 | [InfluxDB exporter](https://github.com/prometheus/influxdb_exporter) |
| 9123 | [RethinkDB exporter](https://github.com/oliver006/rethinkdb_exporter) |
| 9124 | [FreeBSD sysctl exporter](https://svnweb.freebsd.org/base/head/usr.sbin/prometheus_sysctl_exporter/) |
| 9125 | [StatsD exporter](http://github.com/prometheus/statsd_exporter): Ingestion |
| 9126 | [New Relic exporter](https://github.com/jfindley/newrelic_exporter) |
| 9127 | [PgBouncer exporter](http://git.cbaines.net/prometheus-pgbouncer-exporter/) |
| 9128 | [Ceph exporter](https://github.com/digitalocean/ceph_exporter/) |
| 9129 | [HAProxy Log exporter](http://git.cbaines.net/prometheus-haproxy-log-exporter/) |
| 9130 | [UniFi Poller](https://github.com/unifi-poller/unifi-poller) and [UniFi exporter (archived, use UniFi Poller or SNMP instead)](https://github.com/mdlayher/unifi_exporter) |
| 9131 | [Varnish exporter](https://github.com/jonnenauha/prometheus_varnish_exporter) |
| 9132 | [Airflow exporter](https://github.com/shalb/airflow-exporter) |
| 9133 | [Fritz!Box exporter](https://github.com/ndecker/fritzbox_exporter) |
| 9134 | [ZFS exporter](https://github.com/eliothedeman/zfs_exporter) / [ZFS exporter (pdf)](https://github.com/pdf/zfs_exporter) |
| 9135 | [rTorrent exporter](https://github.com/mdlayher/rtorrent_exporter) |
| 9136 | [Collins exporter](https://github.com/soundcloud/collins_exporter) |
| 9137 | [SiliconDust HDHomeRun exporter](https://github.com/mdlayher/hdhomerun_exporter) |
| 9138 | [Heka exporter](https://github.com/imgix/heka_exporter) |
| 9139 | [Azure SQL exporter](https://github.com/iamseth/azure_sql_exporter) |
| 9140 | [Mirth exporter](https://github.com/vynca/mirth_exporter) |
| 9141 | [Zookeeper exporter](https://github.com/carlpett/zookeeper_exporter) |
| 9142 | [BIG-IP exporter](https://github.com/ExpressenAB/bigip_exporter) |
| 9143 | [Cloudmonitor exporter](https://github.com/ExpressenAB/cloudmonitor_exporter) |
| 9144 | [grok_exporter](https://github.com/fstab/grok_exporter) |
| 9145 | [Aerospike exporter](https://github.com/alicebob/asprom) |
| 9146 | [Icecast exporter](https://github.com/markuslindenberg/icecast_exporter) |
| 9147 | [Nginx Request exporter](https://github.com/markuslindenberg/nginx_request_exporter) |
| 9148 | [NATS exporter](https://github.com/markuslindenberg/nats_exporter) |
| 9149 | [Passenger exporter](https://github.com/stuartnelson3/passenger_exporter) |
| 9150 | [Memcached exporter](https://github.com/prometheus/memcached_exporter) |
| 9151 | [Varnish Request exporter](https://github.com/stigsb/varnish_request_exporter) |
| 9152 | [Command runner exporter](https://github.com/tomwilkie/prom-run) |
| 9153 | [CoreDNS](https://coredns.io/plugins/metrics/) |
| 9154 | [Postfix Exporter](https://github.com/kumina/postfix_exporter) |
| 9155 | [vSphere Graphite](https://github.com/cblomart/vsphere-graphite)|
| 9156 | [WebDriver Exporter](https://github.com/mattbostock/webdriver_exporter) |
| 9157 | [IBM MQ exporter](https://github.com/ibm-messaging/mq-golang) |
| 9158 | [Pingdom Exporter](https://github.com/strike-team/pingdom_exporter) |
| 9159 | [Syslogstash](https://github.com/discourse/syslogstash) metrics |
| 9160 | [Apache Flink Exporter](https://github.com/matsumana/flink_exporter) |
| 9161 | [Oracle DB Exporter](https://github.com/iamseth/oracledb_exporter) |
| 9162 | [apcupsd exporter](https://github.com/mdlayher/apcupsd_exporter) |
| 9163 | [zgres exporter](https://github.com/jinty/zgres/blob/master/zgres/prometheus.py) |
| 9164 | [s6_exporter](https://github.com/imgix/s6_exporter) |
| 9165 | [AWS instance health exporter](https://github.com/bobtfish/aws-instance-health-exporter) |
| 9166 | [Dovecot exporter](https://github.com/kumina/dovecot_exporter) |
| 9167 | [Unbound exporter](https://github.com/kumina/unbound_exporter) |
| 9168 | [gitlab-monitor](https://gitlab.com/gitlab-org/gitlab-monitor/) |
| 9169 | [Lustre exporter](https://github.com/HewlettPackard/lustre_exporter) |
| 9170 | [Docker Hub Exporter](https://github.com/infinityworksltd/docker-hub-exporter) |
| 9171 | [GitHub Exporter](https://github.com/infinityworksltd/github-exporter) [[alternative](https://github.com/jkroepke/github_exporter)]  |
| 9172 | [Script Exporter](https://github.com/adhocteam/script_exporter) |
| 9173 | [Rancher Exporter](https://github.com/infinityworksltd/prometheus-rancher-exporter) |
| 9174 | [Docker-Cloud Exporter](https://github.com/infinityworksltd/docker-cloud-exporter) |
| 9175 | [Saltstack exporter](https://github.com/BonnierNews/saltstack_exporter) |
| 9176 | [OpenVPN exporter](https://github.com/kumina/openvpn_exporter) |
| 9177 | [libvirt exporter](https://github.com/kumina/libvirt_exporter) |
| 9178 | [Stream exporter](https://github.com/carlpett/stream_exporter) |
| 9179 | [Shield exporter](https://github.com/bosh-prometheus/shield_exporter) |
| 9180 | [ScyllaDB exporter](https://github.com/scylladb/scylla) |
| 9181 | [Openstack Ceilometer exporter](https://github.com/carlpett/openstack-ceilometer_exporter) |
| 9182 | [Windows exporter](https://github.com/prometheus-community/windows_exporter/) _(Formerly wmi_exporter)_ |
| 9183 | [Openstack exporter](https://github.com/CanonicalLtd/prometheus-openstack-exporter)  |
| 9184 | [Twitch exporter](https://github.com/damoun/twitch_exporter) |
| 9185 | [Kafka topic exporter](https://github.com/ogibayashi/kafka-topic-exporter) |
| 9186 | [Cloud Foundry Firehose exporter](https://github.com/bosh-prometheus/firehose_exporter) |
| 9187 | [PostgreSQL exporter](https://github.com/wrouesnel/postgres_exporter) |
| 9188 | [Crypto exporter](https://github.com/ix-ai/crypto-exporter) |
| 9189 | [Hetzner Cloud CSI Driver (Nodes)](https://github.com/hetznercloud/csi-driver) |
| 9190 | [BOSH exporter](https://github.com/bosh-prometheus/bosh_exporter) |
| 9191 | [netflow exporter](https://github.com/paihu/netflow_exporter) |
| 9192 | [ceph_exporter](https://github.com/jcollie/ceph_exporter) |
| 9193 | [Cloud Foundry exporter](https://github.com/bosh-prometheus/cf_exporter) |
| 9194 | [BOSH TSDB exporter](https://github.com/bosh-prometheus/bosh_tsdb_exporter) |
| 9195 | [MaxScale exporter](https://github.com/skord/maxscale_exporter) |
| 9196 | [UPnP Internet Gateway Device exporter](https://github.com/yrro/igd-exporter) |
| 9197 | [Google's mtail log data extractor](https://github.com/google/mtail) |
| 9198 | [Logstash exporter](https://github.com/BonnierNews/logstash_exporter) |
| 9199 | [Cloudflare exporter](https://github.com/wehkamp/docker-prometheus-cloudflare-exporter) |
| 9200 | UNALLOCATED (to avoid collision with Elasticsearch) |
| 9201 | Remote storage bridge example code |
| 9202 | [Pacemaker exporter](https://github.com/marcan/pacemaker-exporter) |
| 9203 | [Domain Exporter](https://github.com/shift/domain_exporter) |
| 9204 | [PCSensor TEMPer exporter](https://github.com/yrro/temper-exporter) |
| 9205 | [Nextcloud exporter](https://github.com/xperimental/nextcloud-exporter) |
| 9206 | [Elasticsearch exporter](https://github.com/braedon/prometheus-es-exporter) (queries and cluster metrics) |
| 9207 | [MySQL exporter](https://github.com/braedon/prometheus-mysql-exporter) (queries) |
| 9208 | [Kafka Consumer Group exporter](https://github.com/braedon/prometheus-kafka-consumer-group-exporter) |
| 9209 | [FastNetMon Advanced exporter](https://fastnetmon.com/docs-fnm-advanced/)|
| 9210 | [Netatmo exporter](https://github.com/xperimental/netatmo-exporter) |
| 9211 | [dnsbl-exporter](https://github.com/Luzilla/dnsbl_exporter/) |
| 9212 | [DigitalOcean Exporter](https://github.com/metalmatze/digitalocean_exporter) |
| 9213 | [Custom Exporter](https://github.com/orange-cloudfoundry/custom_exporter) |
| 9214 | [MQTT Blackbox Exporter](https://github.com/inovex/mqtt_blackbox_exporter) |
| 9215 | [Prometheus Graphite Bridge](https://github.com/stuart-c/prometheus-graphite-bridge) |
| 9216 | [MongoDB Exporter](https://github.com/percona/mongodb_exporter) |
| 9217 | [Consul agent exporter](https://github.com/BonnierNews/consul-agent_exporter) |
| 9218 | [promql-guard](https://github.com/kfdm/promql-guard) |
| 9219 | [SSL Certificate exporter](https://github.com/ribbybibby/ssl_exporter) |
| 9220 | [NetApp Trident exporter](https://github.com/NetApp/trident) |
| 9221 | [Proxmox VE Exporter](https://github.com/znerol/prometheus-pve-exporter) |
| 9222 | [AWS ECS exporter](https://github.com/slok/ecs-exporter) |
| 9223 | [BladePSGI exporter](https://github.com/johto/BladePSGI_exporter) |
| 9224 | [fluentd exporter](https://github.com/wyukawa/fluentd_exporter) |
| 9225 | [mailexporter](https://github.com/cherti/mailexporter) |
| 9226 | [allas](https://github.com/johto/allas) |
| 9227 | [proc_exporter](https://github.com/arnarg/proc_exporter) |
| 9228 | [Flussonic exporter](https://github.com/vsperson/flussonic-exporter)  |
| 9229 | [gitlab-workhorse](https://gitlab.com/gitlab-org/gitlab-workhorse) |
| 9230 | [Network UPS Tools exporter](https://github.com/dominikh/go-nut/tree/master/cmd/nut_exporter) |
| 9231 | [Solr exporter](https://github.com/noony/prometheus-solr-exporter) |
| 9232 | [Osquery exporter](https://github.com/zwopir/osquery_exporter) |
| 9233 | [mgmt exporter](https://github.com/purpleidea/mgmt) |
| 9234 | [mosquitto exporter](https://github.com/sapcc/mosquitto-exporter) |
| 9235 | [gitlab-pages exporter](https://gitlab.com/gitlab-org/gitlab-pages/) |
| 9236 | [gitlab gitaly exporter](https://gitlab.com/gitlab-org/gitaly) |
| 9237 | [SQL Exporter](https://github.com/justwatchcom/sql_exporter) |
| 9238 | [uWSGI Expoter](https://github.com/AndreaGreco/prometeus_uwsgi_exporter) [[alternative](https://github.com/timonwong/uwsgi_exporter)] |
| 9239 | [Surfboard Exporter](https://github.com/ipstatic/surfboard_exporter) |
| 9240 | [Tinyproxy exporter](https://github.com/igzivkov/tinyproxy_exporter) |
| 9241 | [ArangoDB Exporter](https://gitlab.com/flare/arangodb-exporter) |
| 9242 | [Ceph RADOSGW Usage Exporter](https://github.com/blemmenes/radosgw_usage_exporter) |
| 9243 | [Chef Compliance exporter](https://github.com/contino/chef_compliance_exporter) |
| 9244 | [Moby Container Exporter](https://github.com/infinityworks/moby-container-stats) |
| 9245 | [Naemon / Nagios Exporter](https://github.com/Griesbacher/Iapetos) |
| 9246 | [SmartPi](https://github.com/nDenerserve/SmartPi) |
| 9247 | [Sphinx Exporter](https://github.com/foxdalas/sphinx_exporter) |
| 9248 | [FreeBSD gstat Exporter](https://github.com/tykling/gstat_exporter) |
| 9249 | [Apache Flink Metrics Reporter](https://ci.apache.org/projects/flink/flink-docs-master/monitoring/metrics.html#prometheus-orgapacheflinkmetricsprometheusprometheusreporter) |
| 9250 | [OpenTSDB Exporter](https://github.com/cloudflare/opentsdb_exporter) |
| 9251 | [Sensu Exporter](https://github.com/reachlin/sensu_exporter) |
| 9252 | [GitLab Runner Exporter](https://gitlab.com/gitlab-org/gitlab-ci-multi-runner) |
| 9253 | [PHP-FPM exporter](https://github.com/JamesBarwell/phpfpm_exporter) [[alternative](https://github.com/kumina/phpfpm_exporter)] [[alternative](https://github.com/hipages/php-fpm_exporter)] [[alternative (for k8s envs)](https://github.com/oleh-ozimok/php-fpm-exporter)] |
| 9254 | [Kafka Burrow exporter](https://github.com/jirwin/burrow_exporter) |
| 9255 | [Google Stackdriver exporter](https://github.com/frodenas/stackdriver_exporter) |
| 9256 | [td-agent exporter](https://github.com/matsumana/td-agent_exporter) |
| 9257 | [S.M.A.R.T. exporter](https://github.com/cloudandheat/prometheus_smart_exporter) |
| 9258 | [Hello Sense Exporter](https://github.com/xperimental/hello-exporter) |
| 9259 | [Azure Resources Exporter](https://github.com/FXinnovation/azure-resources-exporter) |
| 9260 | [Buildkite Exporter](https://github.com/smithamax/buildkite_exporter) |
| 9261 | [Grafana exporter](https://github.com/frodenas/grafana_exporter) |
| 9262 | [Bloomsky exporter](https://github.com/krazylek/bloomsky-prometheus-exporter) |
| 9263 | [VMWare Guest exporter](https://github.com/ncabatoff/vmwareguest-exporter) |
| 9264 | [Nest exporter](https://github.com/jcollie/nest_exporter) |
| 9265 | [Weather exporter](https://github.com/celliott/weather_exporter) |
| 9266 | [OpenHAB exporter](https://github.com/jcollie/openhab_exporter) |
| 9267 | [Nagios Livestatus Exporter](https://github.com/m-lab/prometheus-nagios-exporter) |
| 9268 | [CrateDB remote remote read/write adapter](https://github.com/crate/crate_adapter) |
| 9269 | [fluent-agent-lite exporter](https://github.com/matsumana/fluent-agent-lite_exporter) |
| 9270 | [Jmeter exporter](https://github.com/johrstrom/jmeter-prometheus-plugin) |
| 9271 | [Pagespeed exporter](https://github.com/foomo/pagespeed_exporter) |
| 9272 | [VMWare exporter](https://github.com/pryorda/vmware_exporter) |
| 9273 | [Telegraf prometheus_client](https://github.com/influxdata/telegraf) |
| 9274 | [Kubernetes PersistentVolume Disk Usage Exporter](https://github.com/joar/k8s-pv-disk-usage-exporter) |
| 9275 | [NRPE exporter](https://github.com/robustperception/nrpe_exporter) |
| 9276 | [GitHubQL Exporter](https://github.com/metalmatze/githubql_exporter) |
| 9276 | [Azure Monitor exporter](https://github.com/RobustPerception/azure_metrics_exporter) |
| 9277 | [Mongo collection exporter](https://github.com/y8/mongo_collection_exporter) |
| 9278 | [Crypto Miner exporter](https://github.com/bugroger/miner-exporter) |
| 9279 | [InstaClustr Exporter](https://github.com/fcgravalos/instaclustr_exporter) |
| 9280 | [Citrix NetScaler Exporter](https://github.com/rokett/Citrix-NetScaler-Exporter) |
| 9281 | [Fastd Exporter](https://github.com/freifunk-darmstadt/fastd-exporter) |
| 9282 | [FreeSWITCH Exporter](https://github.com/moises-silva/mod_prometheus) |
| 9283 | [Ceph ceph-mgr "prometheus" plugin](https://github.com/ceph/ceph) |
| 9284 | [Gobetween](https://github.com/yyyar/gobetween)  |
| 9285 | [Database exporter](https://github.com/Corundex/database_exporter) (oracle/postgres/mssql/mysql sql queries)x |
| 9286 | [VDO Compression and deduplication exporter](https://github.com/pcuzner/vdo_exporter)  |
| 9287 | [Ceph iSCSI Gateway Statistics](https://github.com/ceph/ceph-iscsi) |
| 9288 | [Elgato Key Light exporter](https://github.com/mdlayher/keylight_exporter) |
| 9289 | [Lovoo's IPMI Exporter](https://github.com/lovoo/ipmi_exporter) (to be run on the IPMI host itself) |
| 9290 | [SoundCloud's IPMI Exporter](https://github.com/soundcloud/ipmi_exporter) (querying IPMI externally, blackbox-exporter style) |
| 9291 | [IBM Z HMC Exporter](https://github.com/zhmcclient/zhmc-prometheus-exporter) |
| 9292 | [Netapp ONTAP API Exporter](https://github.com/sapcc/netapp-api-exporter) |
| 9293 | [Connection Status Exporter](https://github.com/daviddetorres/connection-status-exporter) |
| 9294 | [MiFlora / Flower Care Exporter](https://github.com/xperimental/flowercare-exporter) |
| 9295 | [Freifunk Exporter](https://github.com/xperimental/freifunk-exporter) |
| 9296 | [ODBC Exporter](https://github.com/MACHBASE/prometheus-odbc-exporter) |
| 9297 | [Machbase Exporter](https://github.com/MACHBASE/prometheus-machbase-exporter) |
| 9298 | [Generic Exporter](https://github.com/klau2005/prometheus_generic_exporter) |
| 9299 | [Exporter Aggregator](https://github.com/tynany/exporter_aggregator) |
| 9300 | UNALLOCATED (to avoid collision with Elasticsearch) |
| 9301 | [Squid Exporter](https://github.com/boynux/squid-exporter) |
| 9302 | [Faucet SDN Faucet Exporter](https://github.com/REANNZ/faucet/) |
| 9303 | [Faucet SDN Gauge Exporter](https://github.com/REANNZ/faucet/) |
| 9304 | [Logstash Exporter](https://gitlab.com/alxrem/prometheus-logstash-exporter/) |
| 9305 | [go-ethereum Exporter](https://gitlab.com/tlex/geth-exporter/) |
| 9306 | [Kyototycoon Exporter](https://github.com/kanga333/kyototycoon_exporter/) |
| 9307 | [Audisto exporter](https://github.com/ZeitOnline/audisto_exporter) |
| 9308 | [Kafka Exporter](https://github.com/danielqsj/kafka_exporter/) |
| 9309 | [Fluentd Exporter](https://github.com/V3ckt0r/fluentd_exporter) |
| 9310 | [Open vSwitch Exporter](https://github.com/digitalocean/openvswitch_exporter) |
| 9311 | [IOTA Exporter](https://github.com/crholliday/iota-prom-exporter) |
| 9312 | UNALLOCATED (to avoid collision with Sphinx search API) |
| 9313 | [Cloudprober Exporter](https://github.com/google/cloudprober) |
| 9314 | [eris Exporter](https://github.com/prologic/eris) |
| 9315 | [Centrifugo Exporter](https://github.com/nordicdyno/centrifugo_exporter) |
| 9316 | [Tado Exporter](https://github.com/exporters/tado) |
| 9317 | [Tellstick Local Exporter](https://github.com/hoihrig/prometheus-tellstick-exporter) |
| 9318 | [conntrack Exporter](https://github.com/hiveco/conntrack_exporter) |
| 9319 | [FLEXlm Exporter](https://github.com/mjtrangoni/flexlm_exporter) |
| 9320 | [Consul Telemetry Exporter](https://github.com/SWCE/consul_telemetry_exporter) |
| 9321 | [Spring Boot Actuator Exporter](https://github.com/Scalify/spring_exporter) |
| 9322 | [haproxy_abuser_exporter](https://github.com/Bigpoint/haproxy_abuser_exporter) |
| 9323 | [Docker Prometheus Metrics](https://github.com/docker/docker) under `/metrics` endpoint |
| 9324 | [Bird Routing Daemon Exporter](https://github.com/czerwonk/bird_exporter) |
| 9325 | [oVirt Exporter](https://github.com/czerwonk/ovirt_exporter) |
| 9326 | [JunOS Exporter](https://github.com/czerwonk/junos_exporter) |
| 9327 | [S3 Exporter](https://github.com/jamotion/s3-exporter) |
| 9328 | [OpenLDAP syncrepl Exporter](https://github.com/ThoreKr/syncrepl_exporter) |
| 9329 | [CUPS Exporter](https://github.com/ThoreKr/cups_exporter) |
| 9330 | [OpenLDAP Metrics Exporter](https://github.com/tomcz/openldap_exporter) |
| 9331 | [influx-spout Prometheus Metrics](https://github.com/jumptrading/influx-spout/) |
| 9332 | [Network Exporter](https://github.com/Selfnet/prometheus-network-exporter) |
| 9333 | [Vault PKI Exporter](https://github.com/aarnaud/vault-pki-exporter) |
| 9334 | [Ejabberd exporter ](https://github.com/greizgh/ejabberd_exporter) |
| 9335 | [nexsan exporter](https://github.com/yrro/nexsan-exporter)  |
| 9336 | [Mediacom Internet Usage Exporter](https://github.com/jcollie/mediacom-internet-usage-exporter) |
| 9337 | [mqttgateway](https://github.com/inuits/mqttgateway) |
| 9338 | [cAdvisor (Container Advisor) alternate port](https://github.com/google/cadvisor) |
| 9339 | [AWS S3 Exporter](https://github.com/ribbybibby/s3_exporter) |
| 9340 | [(Financial) Quotes Exporter](https://github.com/marcopaganini/quotes-exporter) |
| 9341 | [slurm exporter](https://github.com/vpenso/prometheus-slurm-exporter) |
| 9342 | [FRR Exporter](https://github.com/tynany/frr_exporter) |
| 9343 | [GridServer Exporter](https://github.com/mhale/gridserver-exporter) |
| 9344 | [MQTT Exporter](https://github.com/bendikwa/mqtt_exporter) |
| 9345 | [Ruckus SmartZone Exporter](https://github.com/ddericco/smartzone_exporter) |
| 9346 | [Ping Exporter](https://github.com/knsd/ping-exporter) |
| 9347 | [Junos Exporter](https://github.com/tynany/junos_exporter) |
| 9348 | [BigQuery Exporter](https://github.com/m-lab/prometheus-bigquery-exporter) |
| 9349 | [Configurable Elasticsearch query exporter](https://github.com/croesnick/promesque) |
| 9350 | [ThousandEyes Exporter](https://github.com/sapcc/1000eyes_exporter) |
| 9351 | [Wal-e/wal-g exporter](https://github.com/camptocamp/wal-g-prometheus-exporter) |
| 9352 | [Nature Remo Exporter](https://github.com/kenfdev/remo-exporter) |
| 9353 | [Ceph Exporter](https://github.com/vinted/ceph-exporter) |
| 9354 | [Deluge Exporter](https://github.com/tobbez/deluge_exporter) |
| 9355 | [Nightwatch.js Exporter](https://github.com/nmcclain/nightwatchjs_exporter) |
| 9356 | [Pacemaker Exporter](https://github.com/mjtrangoni/pacemaker_exporter)  |
| 9357 | [P1 Exporter](https://github.com/rgruyters/prometheus-p1-exporter)  |
| 9358 | [Performance Counters Exporter](https://github.com/rgl/PerformanceCountersExporter)  |
| 9359 | [Sidekiq Prometheus](https://github.com/fastly/sidekiq-prometheus) |
| 9360 | [PowerShell Exporter](https://github.com/rgl/PowerShellExporter)  |
| 9361 | [Scaleway SD Exporter](https://github.com/scaleway/prometheus-scw-sd) |
| 9362 | [Cisco Exporter](https://github.com/lwlcom/cisco_exporter) |
| 9363 | [ClickHouse](https://github.com/ClickHouse/ClickHouse) |
| 9364 | [Continent8 Exporter](https://github.com/shift/continent8_exporter) |
| 9365 | [Cumulus Linux Exporter](https://github.com/tynany/cumulus_exporter) |
| 9366 | [HAProxy Stick Table Exporter](https://github.com/sportradar/HAProxy-stick-tables-exporter) |
| 9367 | [teamspeak3_exporter](https://gitea.lubiland.de/lub/teamspeak3_exporter)  |
| 9368 | [Ethereum Client Exporter](https://github.com/31z4/ethereum-prometheus-exporter) |
| 9369 | [Prometheus PushProx](https://github.com/RobustPerception/PushProx)  |
| 9370 | [u-bmc](https://github.com/u-root/u-bmc) |
| 9371 | [conntrack-stats-exporter](https://github.com/traum-ferienwohnungen/conntrack-stats-exporter) |
| 9372 | [AppMetrics/Prometheus](https://github.com/AppMetrics/AppMetrics) |
| 9373 | [GCP Service Discovery](https://github.com/m-lab/gcp-service-discovery) |
| 9374 | ["Smokeping" prober"](https://github.com/SuperQ/smokeping_exporter) |
| 9375 | [Particle Exporter](https://github.com/DazWilkin/particle-exporter)  |
| 9376 | [Falco](https://github.com/falcosecurity/falco) |
| 9377 | [Cisco ACI Exporter](https://github.com/RavuAlHemio/prometheus_aci_exporter) |
| 9378 | [etcd gRPC Proxy Exporter](https://github.com/coreos/etcd) |
| 9379 | [etcd Exporter](https://github.com/coreos/etcd) |
| 9380 | [MythTV Exporter](https://github.com/thknepper/mythtv_exporter) |
| 9381 | [Kafka ZooKeeper Exporter](https://github.com/cloudflare/kafka_zookeeper_exporter) |
| 9382 | [FRRouting Exporter ](https://github.com/snapserv/prometheus-frr-exporter) |
| 9383 | [AWS Health Exporter](https://github.com/Jimdo/aws-health-exporter) |
| 9384 | [AWS SQS Exporter](https://github.com/jmal98/sqs_exporter) |
| 9385 | [apcupsdexporter](https://github.com/tynsh/apcupsdexporter) |
| 9386 | [httpd-exporter](https://github.com/technicalguru/httpd-exporter) |
| 9386 | [Tankerkönig API Exporter](https://github.com/lukasmalkmus/tankerkoenig_exporter) |
| 9387 | [SABnzbd Exporter](https://github.com/msroest/sabnzbd_exporter) |
| 9388 | [Linode Exporter](https://github.com/DazWilkin/linode-exporter)  |
| 9389 | [Scylla-Cluster-Tests Exporter](https://github.com/scylladb/scylla-cluster-tests/) |
| 9390 | [Kannel Exporter](https://github.com/apostvav/kannel_exporter) |
| 9391 | [Concourse Prometheus Metrics](https://concourse.ci/metrics.html) |
| 9392 | [Generic Command Line Output Exporter](https://github.com/MarioMartReq/generic-exporter) |
| 9393 | [Alertmanager Github Webhook Receiver](https://github.com/m-lab/alertmanager-github-receiver) |
| 9394 | [Ruby Prometheus Exporter](https://github.com/discourse/prometheus_exporter) |
| 9395 | [LDAP Exporter](https://github.com/titisan/ldap_exporter) |
| 9396 | [Monerod Exporter](https://github.com/ExcitableAardvark/monerod_exporter) |
| 9397 | [COMAP](https://gitlab.com/sre-gems/comap) |
| 9398 | [Open Hardware Monitor Exporter](https://github.com/rgl/OpenHardwareMonitorExporter) |
| 9399 | [Prometheus SQL Exporter](https://github.com/free/sql_exporter) |
| 9400 | [RIPE Atlas Exporter](https://github.com/czerwonk/atlas_exporter) |
| 9401 | [1-Wire Exporter](https://github.com/bugroger/onewire-exporter) |
| 9402 | [Google Cloud Platform Exporter](https://github.com/DazWilkin/gcp-exporter)  |
| 9403 | [Zerto Exporter](https://github.com/claranet/zerto-exporter) |
| 9404 | [JMX Exporter](https://github.com/prometheus/jmx_exporter) |
| 9405 | [Discourse Exporter](https://github.com/discourse/discourse-prometheus) |
| 9406 | [HHVM Exporter](https://github.com/wikimedia/operations-software-hhvm_exporter) |
| 9407 | [OBS Studio Exporter](https://github.com/lukegb/obs_studio_exporter) |
| 9408 | [RDS Enhanced Monitoring Exporter](https://github.com/mtanda/rds_enhanced_monitoring_exporter) |
| 9409 | [ovn-kubernetes Master Exporter](https://github.com/ovn-org/ovn-kubernetes) |
| 9410 | [ovn-kubernetes Node Exporter](https://github.com/ovn-org/ovn-kubernetes) |
| 9411 | [SoftEther Exporter](https://github.com/dalance/softether_exporter) |
| 9412 | [Sentry Exporter](https://github.com/snakecharmer/sentry_exporter) |
| 9413 | [MogileFS Exporter](https://github.com/KKBOX/mogilefs-exporter) |
| 9414 | [Homey Exporter](https://github.com/rickardp/homey-prometheus-exporter) |
| 9415 | [cloudwatch_read_adapter](https://github.com/mtanda/cloudwatch_read_adapter) |
| 9416 | [HP iLO Metrics Exporter](https://github.com/infinityworks/hpilo-exporter) |
| 9417 | [Ethtool Exporter](https://github.com/adeverteuil/ethtool_exporter) |
| 9418 | [Gearman Exporter](https://github.com/bakins/gearman-exporter) |
| 9419 | [RabbitMQ Exporter](https://github.com/kbudde/rabbitmq_exporter) |
| 9420 | [Couchbase Exporter](https://github.com/brunopsoares/prometheus_couchbase_exporter) |
| 9421 | [APIcast](https://github.com/3scale/apicast) |
| 9422 | [jolokia_exporter](https://github.com/scalify/jolokia_exporter) |
| 9423 | [HP RAID Exporter](https://github.com/ProdriveTechnologies/hpraid_exporter) |
| 9424 | [InfluxDB Stats Exporter](https://github.com/carlpett/influxdb_stats_exporter) |
| 9425 | [Pachyderm Exporter](https://github.com/button/pachyderm_exporter) |
| 9426 | [Vespa engine exporter](https://github.com/vespa-engine/vespa_exporter) |
| 9427 | [Ping Exporter](https://github.com/czerwonk/ping_exporter) |
| 9428 | [SSH Exporter](https://github.com/Nordstrom/ssh_exporter) |
| 9429 | [Uptimerobot Exporter](https://github.com/wosc/prometheus-uptimerobot) |
| 9430 | [CoreRAD](https://github.com/mdlayher/corerad) |
| 9431 | [Hpfeeds broker Exporter](https://github.com/Jc2k/hpfeeds3) |
| 9432 | [Windows perflib exporter](https://github.com/leoluk/perflib_exporter) |
| 9433 | [Knot exporter](https://github.com/ghedo/knot_exporter) |
| 9434 | [OpenSIPS exporter](https://github.com/VoIPGRID/opensips_exporter) |
| 9435 | [eBPF exporter](https://github.com/cloudflare/ebpf_exporter) |
| 9436 | [mikrotik-exporter](https://github.com/nshttpd/mikrotik-exporter) |
| 9437 | [Dell EMC Isilon Exporter](https://github.com/paychex/prometheus-isilon-exporter) |
| 9438 | [Dell EMC ECS Exporter](https://github.com/paychex/prometheus-emcecs-exporter) |
| 9439 | [Bitcoind exporter](https://github.com/LePetitBloc/bitcoind-exporter)  |
| 9440 | [RavenDB Exporter](https://github.com/marcinbudny/ravendb_exporter) |
| 9441 | [Nomad Exporter](https://github.com/pcarranza/nomad-exporter) |
| 9442 | [Mcrouter Exporter](https://github.com/Dev25/mcrouter_exporter) |
| 9443 | [Napalm Logs Exporter](https://github.com/napalm-automation/napalm-logs) |
| 9444 | [FoundationDB Exporter](https://github.com/leoluk/fdb_exporter) |
| 9445 | [NVIDIA GPU Exporter](https://github.com/mindprince/nvidia_gpu_prometheus_exporter) |
| 9446 | [Orange Livebox DSL modem Exporter](https://github.com/jeanfabrice/livebox-exporter) |
| 9447 | [Resque Exporter](https://github.com/kaorimatz/resque_exporter) |
| 9448 | [EventStore Exporter](https://github.com/marcinbudny/eventstore_exporter) |
| 9449 | [OMERO.server Exporter ](https://github.com/IDR/omero-prometheus-tools) |
| 9450 | [Habitat Exporter](https://github.com/chef/habitat_exporter) |
| 9451 | [Reindexer Exporter](https://github.com/igtulm/reindexer_exporter) |
| 9452 | [FreeBSD Jail Exporter](https://github.com/phyber/jail_exporter) |
| 9453 | [midonet-kubernetes](https://github.com/midonet/midonet-kubernetes) |
| 9454 | [NVIDIA SMI Exporter](https://github.com/a0s/nvidia-smi-exporter) |
| 9455 | [iptables Exporter](https://github.com/retailnext/iptables_exporter) |
| 9456 | [AWS Lambda Exporter](https://github.com/mtanda/aws_lambda_exporter) |
| 9457 | [Files Content Exporter](https://github.com/a0s/files-content-exporter)  |
| 9458 | [Rocket.Chat Exporter](https://github.com/RocketChat/Rocket.Chat) |
| 9459 | [Yarn Exporter](https://github.com/soloradish/yarn_exporter) |
| 9460 | [HANA Exporter](https://github.com/jenningsloy318/hana_exporter) |
| 9461 | [AWS Lambda read adapter](https://github.com/mtanda/aws_lambda_read_adapter) |
| 9462 | [PHP OPcache Exporter](https://github.com/czhujer/php_opcache_exporter)  |
| 9463 | [Virgin Media/Liberty Global Hub3 Exporter](https://github.com/welbymcroberts/hub3_exporter) |
| 9464 | [Opencensus-nodejs Prometheus Exporter](https://github.com/census-instrumentation/opencensus-node/)  |
| 9465 | [Hetzner Cloud k8s Cloud Controller Manager](https://github.com/hetznercloud/hcloud-cloud-controller-manager) |
| 9466 | [MQTT push gateway](https://github.com/Svedrin/mqtt-pushgateway) |
| 9467 | [nginx-prometheus-shiny-exporter](https://github.com/serge-name/nginx-prometheus-shiny-exporter) |
| 9468 | [nasa-swpc-exporter](https://github.com/cznewt/nasa-swpc-exporter) |
| 9469 | [script_exporter](https://github.com/ricoberger/script_exporter) |
| 9470 | [cachet_exporter](https://github.com/ContaAzul/cachet_exporter) |
| 9471 | [lxc-exporter](https://github.com/czhujer/lxc-exporter) |
| 9472 | [Hetzner Cloud CSI Driver (Controller)](https://github.com/hetznercloud/csi-driver) |
| 9473 | [stellar-core-exporter](https://github.com/stellar/packages/blob/master/stellar-core-prometheus-exporter/stellar-core-prometheus-exporter.py) |
| 9474 | [libvirtd_exporter](https://github.com/vexxhost/libvirtd_exporter) |
| 9475 | [wgipamd](https://github.com/mdlayher/wgipam) |
| 9476 | [immugw exporter](https://github.com/codenotary/immudb)  |
| 9477 | [immuclient exporter](https://github.com/codenotary/immudb)  |
| 9478 | [Sentinel exporter](https://github.com/sportradar/sentinel-exporter) |
| 9479 | [Elasticbeat exporter](https://github.com/trustpilot/beat-exporter)  (filebeat, metricbeat, packetbeat, etc...)  |
| 9480 | [Brigade exporter](https://github.com/slok/brigade-exporter) |
| 9481 | [DRBD9 exporter](https://github.com/monzo/drbd9_exporter/) |
| 9482 | [Vector Packet Process (VPP) exporter](https://github.com/FDio/vpp/blob/master/src/vpp/app/vpp_prometheus_export.c) |
| 9483 | [IBM App Connect Enterprise exporter](https://github.com/ot4i/ace-docker) |
| 9484 | [kubedex-exporter](https://github.com/Kubedex/exporter) |
| 9485 | [Emarsys exporter](https://github.com/runtastic/emarsys_exporter) |
| 9486 | [Domoticz exporter](https://github.com/wywywywy/domoticz_exporter) |
| 9487 | [Docker Stats exporter](https://github.com/wywywywy/docker_stats_exporter) |
| 9488 | [BMW Connected Drive exporter](https://github.com/wywywywy/bmw_cd_exporter) |
| 9489 | [Tezos node metrics exporter](https://github.com/ecadlabs/tezos_exporter) |
| 9490 | [Exporter for Docker Libnetwork Plugin for OVN](https://github.com/ovnworks/docker-ovn-driver) |
| 9491 | [Docker Container Stats exporter (`docker ps`)](https://github.com/MOZGIII/docker-ps-exporter) |
| 9492 | [Azure Exporter (Monitor and Usage)](https://gitlab.com/gavinkflam/azure-exporter)  |
| 9493 | [ProSAFE Exporter](https://github.com/dalance/prosafe_exporter) |
| 9494 | [Kamailio Exporter](https://github.com/florentchauveau/kamailio_exporter) |
| 9495 | [Ingestor Exporter](https://github.com/bosh-prometheus/ingestor_exporter) |
| 9496 | [389ds/IPA Exporter](https://github.com/terrycain/389ds_exporter) |
| 9497 | [ImmuDB exporter](https://github.com/codenotary/immudb)  |
| 9498 | [tp-link HS110 exporter](https://github.com/misach/hs110-exporter.git)  |
| 9499 | [Smartthings exporter](https://github.com/kadaan/smartthings_exporter) |
| 9500 | [Cassandra exporter](https://github.com/zegelin/cassandra-exporter) |
| 9501 | [HetznerCloud exporter](https://github.com/promhippie/hcloud_exporter) |
| 9502 | [Hetzner exporter](https://github.com/promhippie/hetzner_exporter) |
| 9503 | [Scaleway exporter](https://github.com/promhippie/scw_exporter) |
| 9504 | [GitHub exporter](https://github.com/promhippie/github_exporter) |
| 9505 | [DockerHub exporter](https://github.com/promhippie/dockerhub_exporter) |
| 9506 | [Jenkins exporter](https://github.com/promhippie/jenkins_exporter) |
| 9507 | [ownCloud exporter](https://github.com/promhippie/owncloud_exporter) |
| 9508 | [ccache exporter](https://github.com/virtualtam/ccache_exporter) |
| 9509 | [Hetzner Storagebox exporter](https://github.com/fleaz/prometheus-storagebox-exporter) |
| 9510 | [Dummy Exporter](https://github.com/kobtea/dummy_exporter) |
| 9511 | [IIS Log Exporter](https://github.com/GrupaPracuj/iislog-prometheus-exporter/) |
| 9512 | [Cloudera exporter](https://github.com/peterloeffler/cloudera_exporter) |
| 9513 | [OpenConfig Streaming Telemetry Exporter](https://github.com/exaring/openconfig-streaming-telemetry-exporter) |
| 9514 | [App Stores exporter](https://github.com/timoa/app-stores-prometheus-exporter) (Google Play & Itunes) |
| 9515 | [swarm-exporter](https://github.com/jeinwag/swarm-exporter) |
| 9516 | [Prometheus Speedtest Exporter](https://github.com/jeanralphaviles/prometheus_speedtest) |
| 9517 | [Matroschka Prober](https://github.com/exaring/matroschka-prober) |
| 9518 | [Crypto Stock Exchange's Funds Exporter](https://github.com/a0s/crypto-funds-exporter) |
| 9519 | [Acurite Exporter](https://github.com/kadaan/acurite_exporter) |
| 9520 | [Swift Health Exporter](https://github.com/sapcc/swift-health-exporter)|
| 9521 | [Ruuvi exporter](https://github.com/joneskoo/ruuvi-prometheus) |
| 9522 | [TFTP Exporter](https://github.com/adobe/prometheus_tftp_exporter) |
| 9523 | [3CX Exporter](https://github.com/digineo/3cx_exporter/) |
| 9524 | [loki_exporter](https://github.com/ricoberger/loki_exporter) |
| 9525 | [Alibaba Cloud Exporter](https://github.com/aylei/aliyun-exporter) |
| 9526 | [kafka_lag_exporter](https://github.com/mbode/kafka_lag_exporter) |
| 9527 | [Netgear Cable Modem Exporter](https://github.com/ickymettle/netgear_cm_exporter) |
| 9528 | [Total Connect Comfort Exporter](https://github.com/ksanislo/tcc-exporter) |
| 9529 | [Octoprint exporter](https://github.com/wywywywy/octoprint_exporter) |
| 9530 | [Custom Prometheus Exporter](https://github.com/marckhouzam/custom-prometheus-exporter) |
| 9531 | [JFrog Artifactory Exporter](https://github.com/peimanja/artifactory_exporter) |
| 9532 | [Snyk exporter](https://github.com/lunarway/snyk_exporter) |
| 9533 | [Network Exporter for Cisco API](https://github.com/greenpau/network_exporter) |
| 9534 | [Humio exporter](https://github.com/lunarway/humio_exporter) |
| 9535 | [Cron Exporter](https://github.com/serhatcetinkaya/cronetheus) |
| 9536 | [IPsec exporter](https://github.com/dennisstritzke/ipsec_exporter) |
| 9537 | [CRI-O](https://github.com/kubernetes-sigs/cri-o) |
| 9538 | [Bull Queue](https://github.com/UpHabit/bull_exporter) |
| 9539 | [Dedibox Exporter](https://github.com/FinweVI/dedibox-exporter) |
| 9540 | [EMQ exporter](https://github.com/nuvo/emq_exporter) |
| 9541 | [smartmon_exporter](https://github.com/tobbez/smartmon_exporter) |
| 9542 | [SakuraCloud exporter](https://github.com/sacloud/sakuracloud_exporter) |
| 9543 | [Kube2IAM exporter](https://github.com/jtblin/kube2iam) |
| 9544 | [pgio exporter](https://gitlab.com/ongresinc/pgio) |
| 9545 | [HP iLo4 Exporter](https://github.com/MauveSoftware/ilo4_exporter) |
| 9546 | [pwrstat-exporter](https://github.com/ksanislo/pwrstat-exporter) |
| 9547 | [Patroni exporter](https://github.com/Showmax/patroni-exporter) / [Kea Exporter](https://github.com/mweinelt/kea-exporter) |
| 9548 | [trafficserver exporter](https://github.com/poblahblahblah/trafficserver_exporter) |
| 9549 | [raspberry exporter](https://github.com/DerKnerd/raspberry-exporter) |
| 9550 | [rtl_433 exporter](https://github.com/mhansen/rtl_433_prometheus) |
| 9551 | [hostapd exporter](https://bitbucket.i2cat.net/scm/~miguel_catalan/hostapd_prometheus_exporter.git)
| 9552 | [Alpine apk exporter](https://github.com/DerKnerd/apk-exporter)|
| 9552 | [AWS Elastic Beanstalk Exporter](https://github.com/jeremietharaud/elasticbeanstalk-exporter)|
| 9553 | [Apt exporter](https://github.com/DerKnerd/apt-exporter) |
| 9554 | [ACC Server Manager Exporter](https://github.com/grimsi/accservermanager-backend) |
| 9555 | [SONA exporter](https://wiki.onosproject.org/display/ONOS/SONA%3A+DC+Network+Virtualization)|
| 9556 | [routinator exporter](https://github.com/NLnetLabs/routinator)|
| 9557 | [mysql count exporter](https://github.com/errm/mysql_count_exporter) |
| 9558 | [systemd exporter](https://github.com/povilasv/systemd_exporter) |
| 9559 | [ntp exporter](https://github.com/sapcc/ntp_exporter) |
| 9560 | [SQL queries exporter](https://github.com/albertodonato/query-exporter) | 
| 9561 | [qBittorrent exporter](https://github.com/fru1tstand/qbittorrent-exporter) | 
| 9562 | [PTV xServer exporter](https://github.com/concrest/ptv-xserver-exporter) |
| 9563 | [Kibana exporter](https://github.com/vladvasiliu/kibana-prometheus-exporter-py) |
| 9564 | [PurpleAir exporter](https://github.com/vlowe/purpleair_exporter) |
| 9565 | [Bminer exporter](https://github.com/hashrabbit/prometheus-bminer-exporter) |
| 9566 | [RabbitMQ CLI Consumer](https://github.com/corvus-ch/rabbitmq-cli-consumer) |
| 9567 | [Alertsnitch](https://gitlab.com/yakshaving.art/alertsnitch) |
| 9568 | [Dell PowerEdge IPMI exporter](https://github.com/CaptainVascular/poweredge_exporter)  |
| 9569 | [HVPA Controller](https://github.com/gardener/hvpa-controller) |
| 9570 | [VPA Exporter](https://github.com/gardener/vpa-exporter) |
| 9571 | [Helm Exporter](https://github.com/sstarcher/helm-exporter) |
| 9572 | [ctld exporter](https://github.com/Gandi/ctld_exporter) |
| 9573 | [JKStatus Exporter](https://github.com/romulofagundes/jkstatus_exporter)|
| 9574 | [opentracker Exporter](https://github.com/sbruder/opentracker_exporter) |
| 9575 | [PowerAdmin Server Monitor Exporter](https://github.com/FXinnovation/poweradmin_exporter)  |
| 9576 | [ExaBGP Exporter](https://github.com/lusis/exabgp_exporter) |
| 9577 | [Syslog-NG Exporter](https://github.com/brandond/syslog_ng_exporter) |
| 9578 | [aria2 Exporter](https://github.com/sbruder/aria2_exporter) |
| 9579 | [iPerf3 Exporter](https://github.com/edgard/iperf3_exporter) |
| 9580 | [Azure Service Bus Exporter](https://github.com/marcinbudny/servicebus_exporter) |
| 9581 | [CodeNotary vcn Exporter](https://github.com/vchain-us/vcn-k8s) |
| 9582 | [Logentries/Rapid7 Exporter](https://github.com/Diogo-Costa/logentries_exporter) |
| 9583 | [Signatory a remote operation signer for Tezos](https://github.com/ecadlabs/signatory) |
| 9584 | [BunnyCDN exporter](https://github.com/permutive/bunnycdn_exporter) |
| 9585 | [Opvizor Performance Analyzer process exporter](https://github.com/opvizor/process-exporter) |
| 9586 | WireGuard exporter:  [Rust (wg(8))](https://github.com/MindFlavor/prometheus_wireguard_exporter), [Go (native)](https://github.com/mdlayher/wireguard_exporter) |
| 9587 | [nfs-ganesha exporter](https://github.com/Gandi/ganesha_exporter) |
| 9588 | [ltsv-tailer exporter](https://github.com/hirose31/ltsv-tailer) |
| 9589 | [goflow exporter](https://github.com/cloudflare/goflow) |
| 9590 | [Flow Exporter](https://github.com/neptune-networks/flow-exporter) |
| 9591 | [SRCDS Exporter](https://github.com/991jo/srcds_exporter) |
| 9592 | [GCP Quota Exporter](https://github.com/mintel/gcp-quota-exporter) |
| 9593 | [Lighthouse Exporter](https://github.com/pkesc/prometheus_lighthouse_exporter) |
| 9594 | [Plex Exporter](https://github.com/arnarg/plex_exporter)  |
| 9595 | [Netio Exporter](https://github.com/tomsajan/netio-exporter) |
| 9596 | [Azure Elastic SQL Exporter](https://github.com/benclapp/azure_elastic_sql_exporter) |
| 9597 | [GitHub Vulnerability Alerts Exporter](https://github.com/ZeitOnline/github_vulnerability_exporter) |
| 9598 | [Vector Logs & Metrics Router Exporter](https://github.com/timberio/vector) |
| 9599 | [Pirograph Exporter ](https://github.com/marco-m/pirograph) |
| 9600 | [CircleCI Exporter](https://github.com/kronostechnologies/prometheus-exporter-circleci) |
| 9601 | [MessageBird Exporter](https://github.com/roaldnefs/messagebird_exporter) |
| 9602 | [Modbus Exporter](https://github.com/mxinden/modbus_exporter) |
| 9603 | [Xen Exporter (using xenlight)](https://github.com/Gandi/xenlight_exporter) |
| 9604 | [XMPP Blackbox Exporter](https://github.com/horazont/prometheus-xmpp-blackbox-exporter) |
| 9605 | [fping-exporter](https://github.com/schweikert/fping-exporter) |
| 9606 | [ecr-exporter](https://github.com/ministryofjustice/prometheus_ecr_exporter) |
| 9607 | [Raspberry Pi Sense HAT Exporter](https://github.com/mhansen/sense_hat_exporter) |
| 9608 | [Ironic Prometheus Exporter](https://github.com/metal3-io/ironic-prometheus-exporter) |
| 9609 | [netapp exporter](https://github.com/jenningsloy318/netapp_exporter) |
| 9610 | [kubernetes_exporter](https://github.com/shalb-docker/kubernetes_exporter) |
| 9611 | [speedport_exporter](https://gitlab.com/chrko/speedport-exporter) |
| 9612 | "FREE" |
| 9613 | [Azure Health Exporter](https://github.com/FXinnovation/azure-health-exporter)  |
| 9614 | [NUT upsc Exporter](https://github.com/jzck/prometheus-upsc-exporter) |
| 9615 | [Mellanox mlx5 Exporter](https://github.com/david-macmahon/prometheus-mlx5-exporter) |
| 9616 | [Mailgun Exporter](https://github.com/missionlane/prometheus-mailgun-exporter) |
| 9617 | [PI-Hole Exporter](https://github.com/eko/pihole-exporter) |
| 9618 | [stellar-account-exporter](https://github.com/stellar/stellar-account-prometheus-exporter)  |
| 9619 | [stellar-horizon-exporter](https://github.com/stellar/stellar-horizon-prometheus-exporter)  |
| 9620 | [rundeck_exporter](https://github.com/phsmith/rundeck_exporter) |
| 9621 | [OpenNebula exporter](https://github.com/jorisdevrede/one_exporter) |
| 9622 | [BMC exporter](https://github.com/gebn/bmc_exporter)  |
| 9623 | [TC4400 exporter](https://github.com/markuslindenberg/tc4400_exporter) |
| 9624 | [Pact Broker Exporter](https://github.com/pperzyna/pactbroker_exporter)  |
| 9625 | [Bareos Exporter](https://github.com/dreyau/bareos_exporter/)  |
| 9626 | [hockeypuck](https://github.com/hockeypuck/hockeypuck) |
| 9627 | [Artifactory Exporter](https://github.com/mikejoh/artifactory-exporter)  |
| 9628 | [Solace PubSub+ Exporter](https://github.com/dabgmx/solace_exporter) |
| 9629 | [Prometheus GitLab notifier](https://github.com/FUSAKLA/prometheus-gitlab-notifier) |
| 9630 | [nftables exporter](https://github.com/Sheridan/nftables_exporter) |
| 9631 | [A OP5 Monitor exporter](https://github.com/opsdis/monitor-exporter) |
| 9632 | "FREE" |
| 9633 | [smartctl exporter](https://github.com/Sheridan/smartctl_exporter) |
| 9634 | [Aerospike ttl exporter](https://github.com/Alb0t/aerospike-ttl-exporter) |
| 9635 | [Fail2Ban Exporter](https://github.com/lfuelling/fail2ban-exporter) |
| 9636 | "FREE" |
| 9637 | [KubeVersion Exporter](https://github.com/ricoberger/kubeversion-exporter)
| 9638 | [A Icinga2 exporter](https://github.com/opsdis/icinga2-exporter) |
| 9639 | "FREE" |
| 9640 | [Logstash Output Exporter](https://github.com/SpencerMalone/logstash-output-prometheus) |
| 9641 | "FREE" |
| 9642 | [Bugsnag Exporter](https://github.com/ZeitOnline/bugsnag_exporter) |
| 9643 | "FREE" |
| 9644 | [Exporter for grouped process](https://github.com/k1LoW/grouped_process_exporter) |
| 9645 | [Burp exporter](https://github.com/svalouch/burp_exporter) |
| 9646 | [Locust Exporter](https://github.com/ContainerSolutions/locust_exporter) |
| 9647 | [Docker Exporter](https://github.com/shalb-docker/docker_exporter) |
| 9648 | [NTPmon exporter](http://github.com/paulgear/ntpmon) |
| 9649 | [Logstash Exporter](https://github.com/Wing924/logstash-exporter) <br> [Logstash Pipeline Exporter](https://github.com/piequi/prometheus-logstash-pipeline-exporter)|
| 9650 | [Keepalived Exporter](https://github.com/gen2brain/keepalived_exporter) |
| 9651 | [Storj Exporter](https://github.com/anclrii/Storj-Exporter) |
| 9652 | [Praefect Exporter](https://gitlab.com/gitlab-org/gitaly/tree/master/cmd/praefect) |
| 9653 | [Jira Issues Exporter](https://github.com/ZeitOnline/jira_exporter) |
| 9654 | "FREE" |
| 9655 | "FREE" |
| 9656 | [Matrix](https://github.com/matrix-org/synapse/blob/master/docs/metrics-howto.md) |
| 9657 | [Krill exporter](https://github.com/NLnetLabs/krill) |
| 9658 | [SAP Hana SQL Exporter](https://github.com/ulranh/hana_sql_exporter) |
| 9659 | "FREE" |
| 9660 | [Kaiterra Laser Egg Exporter](https://github.com/mhansen/kaiterra_laser_egg_exporter) |
| 9661 | [Hashpipe Exporter](https://github.com/david-macmahon/rb-hashpipe) |
| 9662 | [PMS5003 Particulate Matter Sensor Exporter](https://github.com/mhansen/breathe) |
| 9663 | [SAP NWRFC Exporter](https://github.com/ulranh/sapnwrfc_exporter) |
| 9664 | [Linux HA ClusterLabs exporter](https://github.com/ClusterLabs/ha_cluster_exporter) |
| 9665 | [Senderscore Exporter](https://github.com/MauveSoftware/senderscore_exporter) / [Juniper Junos Exporter](https://github.com/lampwins/junos_exporter) |
| 9666 | [Alertmanager Silences Exporter](https://github.com/FXinnovation/alertmanager-silences-exporter) |
| 9667 | [SMTPD Exporter](https://github.com/xsteadfastx/smtpd_exporter) |
| 9668 | [hanadb_exporter](https://github.com/SUSE/hanadb_exporter) |
| 9669 | [panopticon native metrics](https://github.com/Feeld/panopticon) |
| 9670 | [flare native metrics](https://github.com/Feeld/flare) |
| 9671 | [AWS EC2 Spot Exporter](https://github.com/patcadelina/ec2-spot-exporter) |
| 9672 | [AirControl CO2 Exporter](https://github.com/gebi/co2exporter) |
| 9673 | [CO2 Monitor Exporter](https://github.com/markuslindenberg/co2monitor_exporter) |
| 9674 | [Google Analytics Exporter](https://github.com/xplorfin/googleanalytics_exporter) |
| 9675 | [Docker Swarm Exporter](https://github.com/tomcat-engineering/docker_swarm_exporter) |
| 9676 | [Hetzner Traffic Exporter](https://github.com/UweOhse/hetzner-traffic-exporter) |
| 9677 | [AWS ECS Exporter](https://github.com/bevers222/ecs-exporter)|
| 9678 | [IRCd user exporter](https://github.com/dgl/prometheus-ircd-user-exporter)
| 9679 | [AWS Health Exporter ](https://github.com/vladvasiliu/aws-health-exporter-rs) |
| 9680 | [SAP Host Exporter](https://github.com/SUSE/sap_host_exporter) |
| 9681 | [MyFitnessPal Exporter](https://github.com/lausser/myfitnesspal_exporter) |
| 9682 | [Powder Monkey](https://github.com/sapcc/powder-monkey)  |
| 9683 | [Infiniband Exporter](https://github.com/guilbaults/infiniband-exporter) |
| 9684 | [Kibana Standalone Exporter](https://github.com/chamilad/kibana-prometheus-exporter) |
| 9685 | [Eideticom](http://www.eideticom.com) NoLoad Metric Exporter  |
| 9686 | [AWS EC2 Exporter](https://github.com/0x0I/aws_ec2_exporter) |
| 9687 | [Gitaly Blackbox Exporter](https://gitlab.com/gitlab-org/gitaly) |
| 9688 | BigBlueButton Exporter: [Go](https://github.com/baltuonis/prometheus-bigbluebutton-exporter), [Python](https://github.com/greenstatic/bigbluebutton-exporter) |
| 9689 | [LAN Server Modbus Exporter](https://github.com/MarcusCalidus/lan-server-modbus) |
| 9690 | [TCP Longterm Connection Exporter](https://github.com/culpinnis/tcp_established_exporter) |
| 9691 | [Celery/Redis Exporter](https://github.com/ZeitOnline/celery_redis_prometheus) |
| 9692 | [GCP GCE Exporter](https://github.com/0x0I/gcp-gce-exporter)  |
| 9693 | [Sigma Air Manager Exporter](https://github.com/MarcusCalidus/sigma-air-manager-exporter) |
| 9694 | [Per-User usage Exporter for Cisco XE LNSs](https://github.com/TheHolm/cisco-lns-promethius-exported) |
| 9695 | [CIFS Exporter](https://github.com/shibumi/cifs-exporter)  |
| 9696 | [Jitsi Videobridge Exporter](https://github.com/slrz/jvb-exporter)  |
| 9697 | [Tendermint Blockchain Exporter](https://github.com/dmitry-ee/tendermint-prometheus-exporter) |
| 9698 | [Integrated Dell Remote Access Controller (iDRAC) Exporter](https://github.com/greenpau/idrac_exporter)  |
| 9699 | [Pyncette Exporter](https://github.com/tibordp/pyncette/blob/master/src/pyncette/prometheus.py) 
| 9700 | [Jitsi Meet Exporter](https://github.com/xsteadfastx/jitsiexporter) | 
| 9701 | [Workbook exporter](https://github.com/tobiasbp/workbook_exporter) |
| 9702 | [HomePlug PLC exporter](https://github.com/brandond/homeplug_exporter) |
| 9703 | [Vircadia](https://github.com/kasenvr/project-athena)  |
| 9704 | [Linux TC exporter](https://github.com/fbegyn/tc_exporter)  |
| 9705 | [UPC Connect Box Exporter](https://github.com/mbugert/connectbox-prometheus) |
| 9706 | [Postfix exporter](https://github.com/vinted/postfix-exporter) |
| 9707 | [Radarr exporter](https://github.com/onedr0p/radarr-exporter) |
| 9708 | [Sonarr exporter](https://github.com/onedr0p/sonarr-exporter) |
| 9709 | "FREE" |
| 9710 | [Fortigate exporter](https://github.com/bluecmd/fortigate_exporter) |
| 9711 | [Cloudflare Flan Scan report exporter](https://github.com/MauveSoftware/flan_exporter) |
| 9712 | [Siemens S7 PLC exporter](https://github.com/MarcusCalidus/s7-plc-exporter) |
| 9713 | [GlusterFS Exporter](https://github.com/gluster/gluster-prometheus) |
| 9714 | [Fritzbox exporter](https://github.com/pkern/prometheus-fritzbox-exporter) |
| 9715 | [TwinCAT ADS Web Service exporter](https://github.com/MarcusCalidus/twincat-ads-webservice-exporter) |
| 9716 | [Signald webhook receiver](https://github.com/dgl/alertmanager-webhook-signald) | 
| 9717 | [TPLink EasySmart Switch Exporter](https://github.com/thelastguardian/tplinkexporter)  | 
| 9718 | [Warp10 Exporter](https://github.com/centreon/warp10-sensision-exporter) | 
| 9719 | [Pgpool-II Exporter](https://github.com/pengbo0328/pgpool2_exporter)  | 
| 9720 | [Moodle DB Exporter](https://github.com/debugloop/moodledb_exporter) | 
| 9721 | "FREE" |
| 9722 | [Miele Exporter](https://github.com/gebn/miele_exporter)  |
| 9723 | "FREE" |
| 9724 | [FreeSWITCH Exporter](https://github.com/znerol/prometheus-freeswitch-exporter) |
| 9725 | [sunnyboy_exporter](https://github.com/roidelapluie/sunnyboy_exporter) |
| 9726 | [Python RQ Exporter](https://github.com/mdawar/rq-exporter) |
| 9727 | [CTDB Exporter](https://github.com/jf-guillou/ctdb_exporter) |
| 9728 | [NGINX-RTMP Exporter](https://github.com/mauricioabreu/nginx_rtmp_prometheus) |
| 9729 | [libvirtd_exporter](https://git.cyberia.club/services/libvirtd_exporter) |
| 9730 | [lynis_exporter](https://github.com/MauveSoftware/lynis_exporter) |
| 9731 | [Nebula MAM Exporter](https://github.com/nebulabroadcast/nebula-prometheus-exporter) |
| 9732 | [nftables_exporter](https://github.com/Intrinsec/nftables_exporter) |
| 9733 | [honeypot_exporter](https://github.com/Intrinsec/honeypot_exporter) |
| 9734 | [A10-Networks Prometheus Exporter](https://github.com/a10networks/PrometheusExporter) |
| 9735 | [WebWeaver](https://www.webweaver.de) |
| 9736 | [MongoDB Query Exporter](https://github.com/patrick246/mongodb-query-exporter) |
| 9737 | [Folding@home Exporter](https://github.com/jtai/foldingathome_exporter) |
| 9738 | [Processor Counter Monitor Exporter](https://github.com/opcm/pcm) |
| 9739 | [Kafka Consumer Lag Monitoring](https://github.com/omarsmak/kafka-consumer-lag-monitoring) |
| 9740 | [flightdeck](https://github.com/mdlayher/flightdeck) |
| 9741 | [IBM Spectrum Exporter](https://github.com/topine/ibm-spectrum-exporter) |
| 9742 | [Nature Remo E series Exporter](https://github.com/sorah/remo-e-exporter) |
| 9743 | [GitLab CI Server Exporter](https://gitlab.com/rsrchboy/gitlab_ciserver_exporter) |
| 9744 | [NSX-T Exporter](https://github.com/jk8s/nsxt_exporter) |
| 9745 | [Cryptowat Exporter](https://github.com/nbarrientos/cryptowat_exporter) |
| ... | "FREE" (pick a port in between here please) |
| 9901 | [Envoy proxy](https://github.com/envoyproxy/envoy), since [v1.7.0](https://www.envoyproxy.io/docs/envoy/v1.7.0/intro/version_history#id1) ([doc](https://www.envoyproxy.io/docs/envoy/latest/operations/admin#get--stats?format=prometheus)) |
| 9911 | [Skipper Exporter](https://opensource.zalando.com/skipper/operation/operation/#prometheus) |
| 9913 | [Nginx VTS Exporter](https://github.com/hnlq715/nginx-vts-exporter) |
| 9980 | [Login Exporter](https://github.com/uniwue-rz/login_exporter)|
| 9943 | [FileStat Exporter](https://github.com/michael-doubez/filestat_exporter) |
| 9983 | [Sia Exporter](https://github.com/tbenz9/sia_exporter)|
| 9984 | [CouchDB exporter](https://github.com/gesellix/couchdb-exporter) |
| 9987 | [NetApp Solidfire Exporter](https://github.com/mjavier2k/solidfire-exporter) |
| 9990 | [Wildfly Exporter](https://docs.wildfly.org/18/Admin_Guide.html#MicroProfile_Metrics_SmallRye) |
| 9999 | [Exporter exporter](https://github.com/QubitProducts/exporter_exporter) |

**Please look for open ports on this list (Ctrl+F "FREE") before adding a new port. Thanks!**

If you do not have a public repository with working code, please do not allocate a port. If a project is work-in-progress/WIP, please wait until you are ready to share it with others.

Add new exporters above. If there's a gap try to fill it, otherwise add 1 to the last entry.

## Exporters outside of the standard port ranges:

| Port | Exporter |
| ---- | -------- |
| 3903 | [mtail](https://github.com/google/mtail) |
| 7300 | [MidoNet agent](https://github.com/midonet/midonet) |
| 8080 | [cAdvisor (Container Advisor)](https://github.com/google/cadvisor) / [Traefik](https://docs.traefik.io/observability/metrics/prometheus/) |
| 8082 | [trickster](https://github.com/Comcast/trickster) |
| 8088 | [Fawkes](https://www.fawkesrobotics.org) |
| 8089 | [prom2teams](https://github.com/idealista/prom2teams) |
| 8292 | [Phabricator webhook for Alertmanager](https://github.com/knyar/phalerts) |
| 8404 | [HA Proxy (v2+)](https://www.haproxy.com/blog/haproxy-exposes-a-prometheus-metrics-endpoint/) |
| 9042 | [rds_exporter](https://github.com/percona/rds_exporter) |
| 9087 | [Telegram bot for Alertmanager](https://github.com/inCaller/prometheus_bot) |
| 9095 | [Layer2_Exporter Network Inventory](https://github.com/RamboRogers/layer2_exporter/) |
| 9097 | [JIRAlert](https://github.com/alin-sinpalean/jiralert) |
| 9099 | [SNMP Trapper](https://github.com/chrusty/prometheus_webhook_snmptrapper) |
| 9100 - 9999 | **_see standard port range above!_** |
| 16995 | [Storidge exporter](https://github.com/Storidge/cio-user-docs/blob/master/integrations/prometheus.md) |
| 19091 | [Transmission Exporter](https://github.com/metalmatze/transmission-exporter) |
| 19999 | [Netdata](https://github.com/firehol/netdata) |
| 24231 | [Fluent Plugin for Prometheus](https://github.com/kazegusuri/fluent-plugin-prometheus) |
| 42004 | [ProxySQL exporter](https://github.com/percona/proxysql_exporter) |
| 44322 | [Performance Co-Pilot exporter](https://man7.org/linux/man-pages/man3/pmwebapi.3.html) |
| 61091 | [DCOS exporter](https://docs.d2iq.com/mesosphere/dcos/1.13/metrics/) |
