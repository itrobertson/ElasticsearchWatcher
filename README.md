Watcher Scripts Automation Parameters:

---

These are examples of typical Watcher Alerts, by design the automation component will fill in the variables. For example, you can choose to use BRO/HBSS/ACAS logs or allow the algorithm to chose for you. In addition, you design will allow you the user to pass in the parameter such as aggregation variable, email send to list(s), type of nested aggregation can also be passed in as reference for instance.

---

TODO: Automation can be perform on any part of the Watch. Further discussion may ultimately be required; however, for the most part its plug-and-play with a pass of the variables such as time intervals, username, and even aggregation criteria.


---

USE CASES:

---

List of Use Cases Demonstrating Broad Capabilities:



Contents; 
Daily Status Reports	1; 
New Activities Found	1; 
Systems Reporting	3; 
Critical Auth Logs	4; 
Windows Process Logs	5; 

---

The following list is a compilation of Use cases together with their output.
Daily Status Reports

The following users are currently in an inactive state for the past 30 Days or more:

---


RAW DATA RESULTS:
{jboyd=1, crosenberger=1, jkautz=1, sboyd=1, esmothers=1, dwhitten=1, jnelson=1, spersaud=1, russells=1, yamargui=1, Reedye=1, robinsona=1, tobenshain=1, lterada=1, rolayinka=1, wranglersystem=1, byrda=1, ablizzard=1, houstona=1, BLModest_SA=1, rcalvert=1, dgoldman=1, wgibson=1, jstorms=1, rparra=1, ddawson=1, dabotchie=1, skhanal=1, mschultz=1, nhoffman=1, blarson=1, gillemk=1, amartin=1, msandretto=1, mreich=1, mgutknecht=1, swilson=1, jjao=1, jnoseworthy=1, rrizvi=1, drivenbark=1, sewers=1, aosgood=1, gadams=1, ceddy=1, hmartin=1, aoniha=1, pontiac2system=1, rwilson=1}

---

EXAMPLES:
Inactive Users, Suspicious Activities/programs/applications, trends, volume activities
New Activities Found
Pipeline HBSS Logs

---


   This program captures everything that was created on the network to include new accounts, groups, software deployments, installations, tasks, etc...
Additionally, this program is designed to track all these new activities into a seperate index. This data store is user agnostic! 

 USE CASE: Daily Reporting, User Activity Monitoring, New processes and accounts monitoring, and/or Data Validation 
fshaw : 
          Create Client Task 
          Create deployment 
rorellano : 
          Create Client Task 
          Create deployment 
          Request URL 
snickles : 
          Install Rogue Sensor 
          Remove Rogue Sensor 
          Request URL 
          [DLP] Policy Created 
akronebusch : 
          Request URL 
          Create Client Task 
          Create agent deployment URL data object 
          Create deployment 
system : 
          User viewed the Agent Package Download page 
bmiller : 
          Create Client Task 
          Create deployment 
wdaley : 
          Exception created from events 
          Create Client Task 
ngruden : 
          Request URL 
slambert : 
          Create Client Task 
          Create deployment 
aparris : 
          [DLP] policy Rule Created 
          [DLP] Classification Created 
bmodest : 
          Exception created from events 
          New Group 
jcrew : 
          Request URL 
          [DLP] Policy Created 
jpetitjean : 
          Exception created from events 
nsmigiel : 
          Create Client Task 
          Create deployment 
rthompson : 
          New Tag Group 
srussell : 
          New User 
tborger : 
          Create Client Task 
          Exception created from events 
tglover : 
          Create Client Task 
tstrawser : 
          Create Client Task 
wyi : 
          Exception created from events 
          Trusted Application created from events 
aromanak : 
          Create Client Task 
          Create policy object 
dcohen : 
          Create Client Task 
dmariotti : 
          Request URL 
eyanchuk : 
          New Group 
gtom : 
          Exception created from events 
          Trusted Application created from events 
hkash : 
          Exception created from events 
kwendt : 
          Exception created from events 
thester : 
          Exception created from events 
vbedford : 
          Request URL 
abyrd : 
          New User 
ahouston : 
          New User 
arobinson : 
          New Group 
aweldon : 
          Create Client Task 
dvanhoose : 
          New User 
ereedy : 
          Create Client Task 
lstewart : 
          Exception created from events 
mdalton : 
          Create Client Task 
mjones : 
          Create agent deployment URL data object 
pfulton : 
          Create Client Task 
wvanhoose : 
          New User 
 
Systems Reporting

Pipeline Auth Logs

---

   The following systems have not reported logs in the last 24h hours using  a 3d window.
USE CASE: Verify Systems Reporting, Systems connectivity, and/or Data Validation 
Do per each index type.

---

123.456.789
etc...

Critical Auth Logs
175 Critical Errors have occured in Auth Pipeline within past 24 hours

---


MESSAGE: fatal: Cannot bind any address.
TIME: 2017-02-03T19:40:55.000Z
HOST: 123.123.123.123
SOURCE: XXX.XXX.army.mil
Windows Process Logs 
Pipeline Windows Logs

---

This Alert collects executables ran across the windows domains for a 30-day period, aggregates them according to process, and further aggregates them according to username (also, source ip possible)

---

 USE CASE: Daily Reporting, User Activity Monitoring, Process Management, Security Monitoring
 


C:\Windows\SysWOW64\cmd.exe   
          NAE\IITEL13$ Results: 2464625
          NAE\ADLCWKLS2715K$ Results: 4935
          NAE\lynn.edmiston.ao Results: 435
          NAE\lynn.edmiston Results: 373
          NT AUTHORITY\LOCAL SERVICE Results: 22
          NAE\edward.c.albert2.ao Results: 2
          NAE\thuan.nguyen2 Results: 1
C:\Windows\System32\conhost.exe   
          NAE\IITEL13$ Results: 2428339
          NAE\ADLCWKLS2715K$ Results: 24636
C:\Windows\SysWOW64\netsh.exe   
          NAE\IITEL13$ Results: 89331
          NAE\lynn.edmiston.ao Results: 25
          NAE\lynn.edmiston Results: 20
          NAE\ADLCWKLS2715K$ Results: 1
C:\Windows\SysWOW64\sc.exe   
          NAE\IITEL13$ Results: 81146
          NAE\ADLCWKLS2715K$ Results: 12
          NAE\lynn.edmiston.ao Results: 4
C:\Program Files (x86)\McAfee\Policy Auditor Agent\fimcli.exe   
          NAE\ADLCWKLS2715K$ Results: 12380
          NAE\IITEL13$ Results: 8627
C:\Windows\SysWOW64\tasklist.exe   
          NAE\IITEL13$ Results: 16566
          NAE\ADLCWKLS2715K$ Results: 2939
C:\Windows\System32\SearchFilterHost.exe   
          NAE\ADLCWKLS2715K$ Results: 14085
          NAE\IITEL13$ Results: 864
C:\Windows\System32\SearchProtocolHost.exe   
          NAE\ADLCWKLS2715K$ Results: 13742
          NAE\IITEL13$ Results: 909
C:\Program Files (x86)\McAfee\Common Framework\MfeServiceMgr.exe   
          NAE\ADLCWKLS2715K$ Results: 7074
          NAE\IITEL13$ Results: 6315
C:\Windows\SysWOW64\wbem\WmiPrvSE.exe   
          NAE\ADLCWKLS2715K$ Results: 7588
          NAE\IITEL13$ Results: 5410
