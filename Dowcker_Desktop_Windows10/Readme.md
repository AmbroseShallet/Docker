Since we are having virtualbox installed for minikube, If we install docker desktop with Hyper-v it will conflict. Because both Hyper-V and Virtualbox uses the virtualization platform.
So in this case we can install Docket desktop with WSL 2. 

WSL 2 (Windows Subsystem for Linux) enabled if you're using the WSL 2 backend.

Open Powershell and install WSL

wsl --install

Set Default Version to WSL 2

wsl --set-default-version 2

Download Docker Desktop for windows 

Install it. Restart pop=up will come after installing Docker Desktop


![image](https://github.com/user-attachments/assets/1cb01d42-1ad2-481c-a626-dc3e5f6c5140)

Ubundu Unix Username : shallet
pass: universal password


How to check whether Docker desktop is using WSL 2 instead of Hyper-V

Open Docker Desktop. Singn in with creds.

![image](https://github.com/user-attachments/assets/03756135-80d1-463f-9501-55ac6c409b8f)

while executing docker info command, got below error.


![image](https://github.com/user-attachments/assets/fb4ea042-1c72-446b-ae46-d4d761459d88)

Solution:

enable ubuntu in resources for WSL

![image](https://github.com/user-attachments/assets/30e532a8-4338-4447-9e5b-b281497481ae)

while runninng docker info from powershell got below error:

![image](https://github.com/user-attachments/assets/b586c6e1-95cf-42b8-ae24-7051c4fdd9fc)

Solution:

![image](https://github.com/user-attachments/assets/6eab56ae-7efa-4144-ae9b-438d795cefc4)

Reboot windows system if required.













