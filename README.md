# Security Using 802.1X Port-Based Authentication
The IEEE 802.1X standard defines a port-based access control and authentication protocol that restricts 
unauthorized workstations from connecting to a LAN through publicly accessible switch ports. The 
authentication server authenticates each workstation that is connected to a switch port before making available 
any services offered by the switch or the LAN.


### The 802.1x roles include:

    • Supplicant (Client) 

    • Authenticator (Switch)

    • Authentication server

### 802.1X Configuration
802.1X Configuration requires a few basic steps:
    
       Step 1. Enable AAA using the aaa new-model command.
      
       Step 2. Designate the RADIUS server and configure its address and ports.
      
       Step 3. Create an 802.1X port-based authentication method list using the aaa authentication dot1x
               command.
    
       Step 4. Globally enable 802.1X port-based authentication using the dot1x system-auth-control command.
      
       Step 5. Enable port-based authentication on the interface using the authentication port-control auto
               command.
               
       Step 6. Enable 802.1X authentication on the interface using the dot1x pae command. The authenticator
                options sets the Port Access Entity (PAE) type so the interface acts only as an authenticator and will not 
                respond to any messages meant for a supplicant.
