# Bot_Flipkart


Automated program to buy Flipkart products in flash sale online. 
Specifically to buy products which go out of sale in a fraction of seconds and are too difficult to buy manually.

HOW TO:

To run the program follow below steps:

1. Get the latest version of Python at http://www.python.org/getit/.

2.Ensure that python and pip3 path is added in the environment variables

3. install selenium, configparser by running below command in Command Promt.
(this command won't work if environment variable for pip3 is not set)

pip3 install selenium configparser 

4. Download chromedriver from below website and move the .exe file to the folder of the main project folder.

http://chromedriver.chromium.org/

5. Modify the config.ini file to

[MAIN]
DRIVER_LOCATION = chromedriver.exe

>> This is the path of the chromedriver.exe file. Do not change it if the .exe file is in the main project folder.

[CREDENTIALS]
USERNAME = usename@email.com
PASSWORD = password123

>> Add your flipkart credentials

[ORDER]
CVV = 123
ADDRESS = CNTCTC4582E2C20EB4B74BFAD64124
PAYMENT = EMI_OPTIONS

>> Use below Payment keywords to select different options for payment
>> FULL / NET_OPTIONS / PHONEPE / COD / EMI_OPTIONS
>> To select address of delivery, right click and select inspect on delivery address on flipkart page, prior to running the script, and find the address ID as shown in below image. Keep only one address saved on flipkart and delete the rest, as multiple addresses may cause confusion to the script
https://imgur.com/TahLmU8

[EMIOPTIONS]
BANK = HDFC Bank Credit Card
TENURE = 6

>> To select EMI option for payment. Only need to be changed if PAYMENT is selected as EMI_OPTIONS
