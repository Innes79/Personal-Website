How to install and run your Hugo website

1. Install git
 
install git with this command (install winget if not already installed, should be default)  or use the installer provided on their website:
winget install --id Git.Git -e --source winget

2. Install Hugo

install hugo with this command (install winget if not already installed, should be default):
winget install Hugo.Hugo.Extended

3. Clone the repository

reset your terminal to allow the terminal to reset and update then paste this into your terminal:
git clone --recurse-submodules https://github.com/Innes79/Personal-Website.git

4. Enter the folder created

type this into your terminal to enter the file created with all the code and assets:
cd Personal-Website

5. launch the website

while still in the folder we entered with cd type this into your terminal to host the website:
hugo server

6. Make it available for all devices on your network

to make it available for all devices on your network first find your ip address type this comand into a new terminal window and look for IPv4 Address:
ipconfig

7. enter the folder we cloned from github earlier:

type this into your terminal to enter the file created with all the code and assets earlier:
cd Personal-Website

8. bind the website to your IPv4 Address

type this to bind it to your ip address but replace 192.168.1.XX with your IPv4 Address (this is temporary and will need to be typed in again if the terminal is shut, you will need to bind it again)
hugo server --bind 0.0.0.0 --baseURL http://192.168.1.XX
