Example config with muxing:

config interface 'wan'
	option proto 'qmi'
	option apn 'nonbonding.hybrid'
	option pincode '1234'
	option failreboot '50'
	option ipv6 '1'
	option ipv4 '1'
	option dhcp '0'
	option auto '1'
	option device 'wwan0m1'
	option zero_rx_timeout '600'
	list at_init 'AT+QCFG="NWSCANMODE",3'
	list at_init 'AT+QNWLOCK="common/4g",4,1300,212,6400,381,3749,199,500,353'

