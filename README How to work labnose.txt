LabNose connects to the internet and to arduino cloud once powered on. However, the Internet Name and password must be entered on the arduino cloud site underneath the “Things” tab. 
Arduino is currently using Roy Corella’s Arduino account so his log in info will be left below in case someone else needs to access the LabNose dashboard and code.

Link To cloud:
https://app.arduino.cc/

Username:
(private)

Password:
(private)

Arduino then continuously collects data and feeds it to the arduino dashboard page in order to make charts. These charts are VOC over time and are held in the arduino cloud for 15 days.

LabNose is connected to a 3rd party website called If This Then That (ITTT for short) in order to send a text when enough gas is detected. Once the trigger is set off (currently it is hitting 1000 ppb) then the arduino sends a webhook signal to the If This Then That website. Once IFTT receives the webhook signal, it is set up so then it will send a text to the associated phone number on the account. There are currently 2 LabNoses functioning. Each LabNose requires a separate IFTT account and each account requires a $3/month subscription. We have set up 2 IFTT accounts. One for each LabNose. The login information will be left below. The accounts are currently getting paid by Roy.

IFTT #1 (Connected to Dr. K’s phone currently)

Username: (private)
Password: (private)

IFTT #2 (Connected to Roy’s phone currently)

Username: (private)
Password: (private)




IF LABNOSE IS ALREADY SETUP: 

If LabNose has already been connected setup previously then follow these instructions to operate it.

Plug in LabNose
Log In to Arduino Cloud
Open the LabNose Dashboard in order to see charts and gauges 
You can also download the arduino cloud app on IPhone and access the dashboard that way

If you need to modify the code or look at the serial monitor you must also connect the micro usb to LabNose to a computer and open up the serial monitor in the Sketch tab on the arduino cloud website.

