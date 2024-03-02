# CISCO-OSPD-Routing-protocol-

Router 1
Router(config)#router ospf 1
Router(config-router)#router-id 2.2.2.2
Router(config-router)#network 192.168.10.0 0.0.0.3 area 0
Router(config-router)#network 192.168.10.8 0.0.0.3 area 0
Router(config-router)#exit 

Router 2
Router(config)#router ospf 1
Router(config-router)#router-id 1.1.1.1
Router(config-router)#network 192.168.10.12 0.0.0.3 area 1
Router(config-router)#network 192.168.10.0 0.0.0.3 area 0
Router(config-router)#network 192.168.10.4 0.0.0.3 area 1
Router(config-router)#exit

Router 3
Router(config)#router ospf 1
Router(config-router)#router-id 3.3.3.3
Router(config-router)#network 192.168.10.16 0.0.0.3 area 1
Router(config-router)#network 192.168.10.4 0.0.0.3 area 1
Router(config-router)#exit 
