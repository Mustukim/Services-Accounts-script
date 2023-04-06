# Services-Accounts-script
A script to generate 100 Services Accounts 
A script to generate 100 Services Accounts HomeCreate 100 Services Accounts ( 100 json files ) , Token.pickle , Token_sa.pickle & emails.txt

Create 100 Services Accounts ( 100 json files ) , Token.pickle , Token_sa.pickle & emails.txt

Run these commands in Termux👇

pkg install python3

pkg update python3

pkg install git

git clone https://github.com/Mustukim/Services-Accounts-script

pip3 install -r requirements.txt

pip install --upgrade pip ( optional )

pwd

cd /sdcard or cd /storage or cd sdcard or cd storage

cd download

cp -r credentials.json "YOUR COPIED PATH"

cd

cd Services-Accounts-script

ls

python3 gen_sa_accounts.py

Note - AUTHORIZE URL

python3 gen_sa_accounts.py --enable-services $PROJECT ID

python3 gen_sa_accounts.py --create-sas PROJECT ID

python3 gen_sa_accounts.py --download-keys $PROJECT ID

ls

cd

cd accounts

grep -oPh '"client_email": "\K[^"]+' *.json > emails.txt

ls

cp -r emails.txt /sdcard/download

rm -r emails.txt

cd ..

cp -rf accounts /sdcard/download

python3 generate_drive_token.py

Note - 27th command is optional. ( It is for generating Token.pickle File )

exit
