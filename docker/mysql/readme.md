grant all privileges on _._ to riskcontrol@'%' with grant option;

flush privileges;

create database riskcontrol;

use riskcontrol;

source /root/mpc/riskcontral/manifest/migration/risk_control.sql

mysql -h 127.0.0.1 -P 3306 -u riskcontrol -p < ./packages/riskmanage_dump.sql
