# How To Use
1.At first, change information about api_key,secret_key and url from the codes.
  api_key = "your_api_key"  
  sec_key = "your_secret_key"

  base_url = "http://your_management_ip:8080/client/api" 

2.Next, running cs3_api with *command* option.  
e.g.)

    # ./cs3_api command=createNetworkOffering \  
                displaytext=srx \
                guestiptype=Isolated \  
                name=srx \  
                supportedservices=DHCP,Firewall,StaticNAT,SourceNAT,Portforwarding \  
                traffictype=GUEST \  
                serviceproviderlist[0].service=Firewall \  
                serviceproviderlist[0].provider=JuniperSRX \  
                serviceproviderlist[1].service=StaticNAT \  
                serviceproviderlist[1].provider=JuniperSRX \  
                serviceproviderlist[2].service=SourceNAT \       
                serviceproviderlist[2].provider=JuniperSRX \  
                serviceproviderlist[3].service=Portforwarding \  
                serviceproviderlist[3].provider=JuniperSRX \                         
                response=json  
