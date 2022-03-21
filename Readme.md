#  How to create service account with mobile phone using termux

- [x] First install termux on your phone and You can download Termux here by click below icon.
[![](hhttps://telegra.ph/file/bba5b4f396e1d9d4a6420.png)version 0.117](https://drive.google.com/uc?id=1vi4EoX7m_6rS1WNW17Lur1J0f1Zt1j8o&export=download)

After complete installation process, run below cmd on termux.
```
termux-setup-storage
```
```
pkg update
```
```
pkg upgrade 
```
```
pkg install git
```
```
pkg install python
```
```
pip install --upgrade pip
```
```
mkdir /sdcard/MyTermux/ -p
```
```
cd /sdcard/MyTermux
```
```
git clone https://github.com/phoethar1/service-accounts
```
```
cd /sdcard/MyTermux/service-accounts
```
```
pip3 install -r requirements.txt
```
credentials.json file ကို [Google Console](https://console.cloud.google.com/?pli=1)မှာပြုလုပ်ပါ

```
python3 gen_sa_accounts.py --quick-setup -1
```
```
python3 gen_sa_accounts.py  --download-keys Your Project ID
```
python generate_drive_token.py
```
```
cd accounts
```
```
python3 emails.py
```