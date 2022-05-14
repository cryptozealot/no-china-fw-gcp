# no-china-fw-gcp

gcloud config set project {projectid}

gcloud compute firewall-rules create no-china-1 --description="Blocking these Chinese bots that want to rack up my network charges" --direction=INGRESS --priority=100 --network=default --action=DENY --rules=all --source-ranges=1.24.0.0/13,1.48.0.0/15,1.50.0.0/16,1.56.0.0/13,1.68.0.0/14,1.80.0.0/13,1.92.0.0/14,1.180.0.0/14,1.188.0.0/14,1.192.0.0/13,1.202.0.0/15,1.204.0.0/14,14.16.0.0/12,14.104.0.0/13,14.112.0.0/12,14.134.0.0/15,14.144.0.0/12,14.204.0.0/15,14.208.0.0/12,23.80.54.0/24,23.104.141.0/24,23.105.14.0/24,23.226.208.0/24,27.8.0.0/13,27.16.0.0/12,27.36.0.0/14,27.40.0.0/13,27.50.128.0/17,27.54.192.0/18,27.106.128.0/18,27.115.0.0/17,27.148.0.0/14,27.152.0.0/13,27.184.0.0/13,27.192.0.0/11,27.224.0.0/14,36.1.0.0/16,36.4.0.0/14,36.26.0.0/16,36.32.0.0/14,36.36.0.0/16,36.40.0.0/13,36.48.0.0/15,36.56.0.0/13,36.96.0.0/11,36.128.0.0/11,36.248.0.0/14,39.64.0.0/11,39.96.0.0/13,39.128.0.0/10,42.4.0.0/14,42.48.0.0/15,42.52.0.0/14,42.56.0.0/14,42.84.0.0/14,42.88.0.0/13,42.96.128.0/17,42.100.0.0/14,42.120.0.0/14,42.156.0.0/16,42.176.0.0/13,42.185.0.0/16,42.202.0.0/15,42.224.0.0/12,42.242.0.0/15,42.248.0.0/15,43.255.0.0/20,43.255.16.0/22,43.255.48.0/22,43.255.60.0/22,43.255.64.0/20,43.255.96.0/20,43.255.144.0/22,43.255.168.0/22,43.255.176.0/22,43.255.184.0/22,43.255.192.0/22,43.255.200.0/21,43.255.208.0/21,43.255.224.0/21,43.255.232.0/22,43.255.244.0/22,47.74.0.0/15,47.76.0.0/14,47.80.0.0/13,47.88.0.0/14,47.92.0.0/14,49.5.0.0/16,49.64.0.0/11,49.112.0.0/13,54.222.0.0/15,58.16.0.0/14,58.20.0.0/16,58.21.0.0/16,58.22.0.0/15,58.34.0.0/16,58.37.0.0/16,58.38.0.0/16,58.40.0.0/16,58.42.0.0/16,58.44.0.0/14,58.48.0.0/13,58.56.0.0/14,58.60.0.0/14,58.68.128.0/17,58.82.0.0/15,58.100.0.0/15,58.116.0.0/14,58.128.0.0/13,58.208.0.0/12,58.240.0.0/13,58.248.0.0/13,59.32.0.0/12,59.48.0.0/14,59.52.0.0/14,59.56.0.0/13,59.72.0.0/16,59.108.0.0/15,59.172.0.0/14,60.0.0.0/12,60.11.0.0/16,60.12.0.0/14,60.16.0.0/13,60.24.0.0/13,60.160.0.0/11,60.194.0.0/15,60.205.0.0/16,60.208.0.0/12,60.253.128.0/17,61.4.64.0/20,61.4.80.0/22,61.4.176.0/20,61.48.0.0/13,61.128.0.0/10,61.135.0.0/16,61.136.0.0/18,61.139.0.0/16,61.145.73.208/28,61.147.0.0/16,61.150.0.0/16,61.152.0.0/16,61.154.0.0/16,61.158.0.0/16,61.160.0.0/16,61.162.0.0/15,61.164.0.0/16,61.172.0.0/15,61.175.0.0/16,61.177.0.0/16,61.179.0.0/16,61.183.0.0/16,61.184.0.0/16,61.185.219.232/29,61.187.0.0/16,61.188.0.0/16,61.232.0.0/14,61.236.0.0/15,61.240.0.0/14,94.191.0.0/17

gcloud compute firewall-rules create no-china-2 --description=https://www.wizcrafts.net/chinese-blocklist.html --direction=INGRESS --priority=100 --network=default --action=DENY --rules=all --source-ranges=101.16.0.0/12,101.37.0.0/16,101.64.0.0/13,101.72.0.0/14,101.76.0.0/15,101.80.0.0/12,101.132.0.0/15,101.200.0.0/15,101.224.0.0/13,101.248.0.0/15,101.254.0.0/16,103.211.164.0/22,103.253.4.0/22,106.4.0.0/14,106.8.0.0/15,106.12.0.0/14,106.16.0.0/12,106.32.0.0/12,106.43.0.0/16,106.56.0.0/13,106.74.0.0/15,106.80.0.0/12,106.108.0.0/14,106.112.0.0/13,106.120.0.0/13,110.6.0.0/15,110.16.0.0/14,110.51.0.0/16,110.52.0.0/15,110.80.0.0/13,110.88.0.0/14,110.96.0.0/11,110.152.0.0/14,110.156.0.0/15,110.166.0.0/15,110.173.0.0/19,110.173.32.0/20,110.173.64.0/18,110.176.0.0/14,110.184.0.0/13,110.192.0.0/11,110.228.0.0/14,110.240.0.0/12,111.0.0.0/10,111.72.0.0/13,111.85.0.0/16,111.112.0.0/15,111.120.0.0/14,111.124.0.0/16,111.126.0.0/15,111.128.0.0/11,111.160.0.0/13,111.172.0.0/14,111.176.0.0/13,111.192.0.0/12,111.224.0.0/14,111.228.0.0/14,112.0.0.0/10,112.64.0.0/14,112.73.0.0/16,112.74.0.0/16,112.80.0.0/12,112.98.0.0/15,112.100.0.0/14,112.109.128.0/17,112.111.0.0/16,112.112.0.0/14,112.116.0.0/15,112.122.0.0/15,112.192.0.0/14,112.224.0.0/11,113.0.0.0/13,113.8.0.0/15,113.12.0.0/14,113.16.0.0/15,113.18.0.0/16,113.54.0.0/15,113.56.0.0/15,113.58.0.0/16,113.59.0.0/17,113.62.0.0/15,113.64.0.0/10,113.120.0.0/13,113.128.0.0/15,113.132.0.0/14,113.136.0.0/13,113.194.0.0/15,113.200.0.0/15,113.204.0.0/14,113.218.0.0/15,113.220.0.0/14,113.224.0.0/12,113.240.0.0/13,113.248.0.0/14,114.28.0.0/16,114.54.0.0/15,114.64.0.0/14,114.80.0.0/12,114.96.0.0/13,114.104.0.0/14,114.112.0.0/14,114.135.0.0/16,114.138.0.0/15,114.215.0.0/16,114.216.0.0/13,114.224.0.0/11,115.24.0.0/15,115.28.0.0/15,115.32.0.0/14,115.48.0.0/12,115.84.0.0/18,115.100.0.0/14,115.148.0.0/14,115.152.0.0/15,115.159.0.0/16,115.166.64.0/19,115.168.0.0/14,115.192.0.0/11,115.224.0.0/12,116.1.0.0/16,116.2.0.0/15,116.4.0.0/14,116.8.0.0/14,116.16.0.0/12,116.52.0.0/14,116.56.0.0/15,116.60.0.0/14,116.76.0.0/15,116.85.0.0/16,116.90.80.0/20,116.95.0.0/16,116.112.0.0/14,116.116.0.0/15,116.128.0.0/10,116.204.0.0/15,116.207.0.0/16,116.208.0.0/14,116.213.64.0/18,116.213.128.0/17,116.224.0.0/12,116.248.0.0/15,116.252.0.0/15,116.254.128.0/18,117.8.0.0/13,117.21.0.0/16,117.22.0.0/15,117.24.0.0/13,117.32.0.0/13,117.40.0.0/14,117.44.0.0/15,117.50.0.0/16,117.51.0.0/16,117.57.0.0/16,117.60.0.0/14,117.64.0.0/13,117.79.224.0/20,117.80.0.0/12,117.106.0.0/15,117.112.0.0/13,117.128.0.0/10,118.24.0.0/15,118.26.0.0/16,118.72.0.0/13,118.80.0.0/15,118.89.0.0/16,118.112.0.0/13,118.120.0.0/14,118.124.0.0/15,118.132.0.0/14,118.144.0.0/14,118.180.0.0/14,118.186.0.0/15,118.192.0.0/15,118.194.0.0/16,118.213.0.0/16,118.244.0.0/16,118.248.0.0/13,119.0.0.0/13,119.8.0.0/16,119.10.0.0/17,119.18.192.0/20,119.23.0.0/16,119.28.0.0/15,119.32.0.0/14,119.36.0.0/16,119.39.0.0/16,119.44.0.0/16,119.48.0.0/13,119.57.0.0/16,119.60.0.0/15,119.62.0.0/16,119.84.0.0/14,119.88.0.0/14,119.96.0.0/13,119.108.0.0/15,119.112.0.0/13,119.120.0.0/13,119.128.0.0/12,119.144.0.0/14,119.162.0.0/15,119.164.0.0/14,119.176.0.0/12,119.233.0.0/16,119.248.0.0/14,120.0.0.0/12,120.24.0.0/14,120.30.0.0/15

gcloud compute firewall-rules create no-china-3 --description="2 and 3 are both made up of line 2 in the source rules" --direction=INGRESS --priority=100 --network=default --action=DENY --rules=all --source-ranges=120.32.0.0/13,120.40.0.0/14,120.68.0.0/14,120.76.0.0/14,120.80.0.0/13,120.92.0.0/16,120.192.0.0/10,121.0.16.0/20,121.4.0.0/15,121.8.0.0/13,121.16.0.0/12,121.32.0.0/14,121.40.0.0/14,121.52.208.0/20,121.52.224.0/19,121.56.0.0/15,121.60.0.0/14,121.68.0.0/14,121.76.0.0/15,121.100.128.0/17,121.196.0.0/14,121.201.0.0/16,121.204.0.0/14,121.224.0.0/12,122.4.0.0/14,122.8.0.0/16,122.10.128.0/17,122.51.128.0/17,122.64.0.0/11,122.96.0.0/15,122.119.0.0/16,122.136.0.0/13,122.156.0.0/14,122.188.0.0/14,122.192.0.0/14,122.198.0.0/16,122.200.64.0/18,122.224.0.0/12,122.240.0.0/13,123.4.0.0/14,123.8.0.0/13,123.52.0.0/14,123.56.0.0/14,123.64.0.0/11,123.97.128.0/17,123.100.0.0/19,123.112.0.0/12,123.128.0.0/13,123.138.0.0/15,123.144.0.0/14,123.148.0.0/15,123.150.0.0/15,123.152.0.0/13,123.160.0.0/14,123.164.0.0/14,123.172.0.0/15,123.178.0.0/15,123.180.0.0/14,123.184.0.0/13,123.196.0.0/15,123.206.0.0/15,123.232.0.0/14,123.244.0.0/14,123.249.0.0/16,124.42.0.0/16,124.64.0.0/15,124.66.0.0/17,124.67.0.0/16,124.72.0.0/13,124.88.0.0/15,124.92.0.0/14,124.112.0.0/15,124.114.0.0/15,124.117.0.0/16,124.118.0.0/15,124.126.0.0/15,124.128.0.0/13,124.152.0.0/16,124.160.0.0/13,124.192.0.0/15,124.200.0.0/13,124.224.0.0/16,124.226.0.0/15,124.228.0.0/14,124.234.0.0/15,124.236.0.0/14,124.240.0.0/17,124.240.128.0/18,124.248.0.0/17,125.32.0.0/14,125.36.0.0/14,125.40.0.0/13,125.64.0.0/12,125.79.0.0/16,125.80.0.0/13,125.88.0.0/13,125.104.0.0/13,125.112.0.0/12,125.210.0.0/15,125.216.0.0/13,132.232.0.0/16,134.175.0.0/16,139.129.0.0/16,139.170.0.0/16,139.189.0.0/16,139.199.0.0/16,139.206.0.0/16,139.208.0.0/13,139.217.0.0/16,139.224.0.0/16,139.226.0.0/15,140.143.0.0/16,140.206.0.0/15,140.224.0.0/16,140.237.0.0/16,140.240.0.0/16,140.246.0.0/16,140.249.0.0/16,140.255.0.0/16,142.4.117.0/30,144.0.0.0/16,144.12.0.0/16,144.52.0.0/16,144.123.0.0/16,144.255.0.0/16,150.109.0.0/16,150.138.0.0/15,150.242.152.0/21,150.242.160.0/21,150.242.168.0/22,153.0.0.0/16,153.99.0.0/16,159.226.0.0/16,162.209.168.0/24,171.8.0.0/13,171.34.0.0/15,171.36.0.0/14,171.40.0.0/13,171.80.0.0/14,171.88.0.0/13,171.104.0.0/13,171.112.0.0/14,171.116.0.0/14,171.120.0.0/13,171.208.0.0/12,175.0.0.0/12,175.16.0.0/13,175.24.0.0/14,175.30.0.0/15,175.42.0.0/15,175.44.0.0/16,175.46.0.0/15,175.48.0.0/12,175.64.0.0/11,175.102.0.0/16,175.106.128.0/17,175.146.0.0/15,175.148.0.0/14,175.152.0.0/14,175.160.0.0/12,175.178.0.0/16,175.184.128.0/18,175.185.0.0/16,175.186.0.0/15,175.188.0.0/14,180.76.0.0/16,180.95.128.0/17,180.96.0.0/11,180.136.0.0/13,180.152.0.0/13,180.160.0.0/12,180.208.0.0/15,180.212.0.0/15,182.18.0.0/17,182.32.0.0/12,182.50.112.0/20,182.61.0.0/16,182.84.0.0/14,182.88.0.0/14,182.96.0.0/12,182.112.0.0/12,182.128.0.0/12,182.144.0.0/13,182.200.0.0/13,182.240.0.0/13,183.0.0.0/10,183.64.0.0/13,183.92.0.0/14,183.128.0.0/11,183.160.0.0/12,183.184.0.0/13,183.192.0.0/10,192.34.109.224/28,198.2.203.64/28,198.2.212.160/28,198.15.171.64/26

gcloud compute firewall-rules create no-china-4 --description="rule 4 is line 3 in source file, as of 2019-09-18" --direction=INGRESS --priority=100 --network=default --action=DENY --rules=all --source-ranges=202.43.144.0/22,202.46.32.0/19,202.65.96.0/20,202.66.0.0/16,202.75.208.0/20,202.96.0.0/12,202.111.160.0/19,202.112.0.0/14,202.117.0.0/16,202.127.112.0/20,202.165.176.0/20,202.196.80.0/20,203.69.0.0/16,203.81.16.0/20,203.86.0.0/18,203.86.64.0/19,203.93.0.0/16,203.169.160.0/19,203.171.224.0/20,203.195.160.0/23,210.5.0.0/19,210.12.0.0/16,210.14.128.0/19,210.21.0.0/16,210.22.0.0/16,210.32.0.0/14,210.51.0.0/16,210.52.0.0/15,210.75.0.0/16,210.77.0.0/16,210.79.64.0/18,210.192.96.0/19,211.76.96.0/20,211.78.208.0/20,211.80.0.0/13,211.86.144.0/20,211.90.0.0/15,211.92.0.0/14,211.96.0.0/13,211.136.0.0/13,211.144.0.0/12,211.160.0.0/13,211.233.70.0/24,212.64.0.0/17,218.0.0.0/11,218.56.0.0/13,218.64.0.0/11,218.84.0.0/14,218.88.0.0/13,218.96.0.0/14,218.102.0.0/16,218.104.0.0/14,218.108.0.0/15,218.194.80.0/20,218.200.0.0/13,218.240.0.0/13,218.249.0.0/16,219.128.0.0/11,219.154.0.0/15,219.223.192.0/18,219.232.0.0/16,219.234.80.0/20,219.235.0.0/16,219.238.0.0/15,220.112.0.0/16,220.154.0.0/15,220.160.0.0/11,220.181.0.0/16,220.191.0.0/16,220.192.0.0/12,220.228.70.0/24,220.242.0.0/15,220.248.0.0/14,220.250.0.0/19,220.252.0.0/16,221.0.0.0/12,221.122.0.0/15,221.130.0.0/15,221.136.0.0/15,221.172.0.0/14,221.176.0.0/13,221.192.0.0/14,221.196.0.0/15,221.198.0.0/16,221.199.0.0/17,221.200.0.0/14,221.204.0.0/15,221.206.0.0/16,221.207.0.0/16,221.208.0.0/12,221.212.0.0/15,221.214.0.0/15,221.216.0.0/13,221.224.0.0/13,221.228.0.0/14,221.232.0.0/13,222.32.0.0/11,222.64.0.0/12,222.80.0.0/12,222.128.0.0/14,222.132.0.0/14,222.136.0.0/13,222.160.0.0/14,222.168.0.0/13,222.172.222.0/24,222.176.0.0/13,222.184.0.0/13,222.200.0.0/16,222.208.0.0/13,222.216.0.0/14,222.220.0.0/15,222.222.0.0/15,222.240.0.0/13,222.249.0.0/16,223.4.0.0/14,223.8.0.0/13,223.64.0.0/11,223.96.0.0/12,223.112.0.0/14,223.144.0.0/12,223.198.0.0/15,223.214.0.0/15,223.223.176.0/20,223.223.192.0/20,223.255.0.0/17,223.240.0.0/13
