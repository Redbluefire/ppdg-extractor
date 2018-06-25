# ppdg-extractor
Extract (CSV) codes from and screenshot (JPG) PayPal Digital Gifts gift cards. Adapted from https://github.com/stevenmirabito/ code in order to clean up screenshots, save screenshots as .JPG, and to process PIN and non-PIN cards using the same program.

Program specifically configured on Windows - includes ChromeDriver.exe - for gmail.

1) Install the newest version of Python: https://www.python.org/downloads/

2) Open command prompt (cmd) and navigate to this folder. Install the dependencies by running the following commands:
	
	 pip3 install -r requirements.txt

3) Rename config.sample.py to config.py and edit the following variables:
	
	a) Change IMAP_USERNAME to your gmail account
		
	b) Create a gmail label for the cards you would like to extract and change FOLDER to this label. This label will serve as the processing folder for your cards. When you would like to extract a card, label it with this label, run the extractor, and then move the card to another label. The program can only see cards that reside in this label.
	
4) Double click on MasterExtractor.bat to run the program. You will get .jpg screenshots in the "screenshots" folder and will have a .csv file with near GCW (GiftCardWiki) submission standards. In order to access the cards, open the .csv file with your notepad program of choice. I prefer Notepad++ (https://notepad-plus-plus.org/download/v7.5.3.html).

5) Enjoy!
