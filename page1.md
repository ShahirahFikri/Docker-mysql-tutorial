## DOCKER INSTALLATION

1) Visit https://docs.docker.com/desktop/windows/install to view the instructions (for windows).

![photo_2022-06-18_15-46-48](https://user-images.githubusercontent.com/104122185/174428310-8499a7d7-213c-49c6-8126-0d34d960bca6.jpg)


2) Click on "Docker Desktop for Windows" and it will automatically be downloaded.

![photo_2022-06-18_15-47-05](https://user-images.githubusercontent.com/104122185/174428353-d080fdd2-ff6a-4b8b-b4a0-f815d2e9a2a9.jpg)


3) Once downloaded, open the Docker Desktop Installer.exe.

![photo_2022-06-18_16-04-49](https://user-images.githubusercontent.com/104122185/174428848-707420de-885d-40c5-9380-a14321aec58c.jpg)


4) Select where you want the installer to save your files. Double click on the "Docker Desktop Installer" to run the installation.

![photo_2022-06-18_16-33-44](https://user-images.githubusercontent.com/104122185/174429828-964d09a8-db34-4cf0-bc05-0f284cf6e5e8.jpg)


5) Configure your Docker desktop and then click "OK" to begin the installation process.

![photo_2022-06-18_16-33-44 (2)](https://user-images.githubusercontent.com/104122185/174429841-a205d435-6d85-46d5-b50a-fcc0682c27b3.jpg)


6) Docker will begin the installation by unpacking the files and wait till the process is done.

![Screenshot (1959)](https://user-images.githubusercontent.com/104122185/174429877-1e54cd27-559b-46d2-be9f-0f0aad69ca47.png)


7) After the installation is completed, click Close and Restart.

![Screenshot (1960)](https://user-images.githubusercontent.com/104122185/174429882-2f4712d2-df51-4f69-9cb7-7bfab5945920.png)


## WSL2 INSTALLATION

1) For installing WSL 2, Docker will display a URL of https://aka.ms/wsl2kernel to be clicked on.

![fi6](https://user-images.githubusercontent.com/104122185/174431467-6b6529ed-c0fa-4d75-beba-30e1cf3c7ad1.jpg)


2) After clicking the link above, select the link that says "Download the latest package."

![photo_2022-06-18_17-35-31](https://user-images.githubusercontent.com/104122185/174431903-50a10557-a999-441c-bc63-c7e5baa54344.jpg)


3) Click on the wsl_update_x64 and wait until the installation finished.

![photo_2022-06-18_17-40-55](https://user-images.githubusercontent.com/104122185/174432134-9ef4a345-bc71-46fc-862e-b9e98d35d9a8.jpg)


4) Click "Finish" when the installation is completed.

![Screenshot (1965)](https://user-images.githubusercontent.com/104122185/174432416-087a519e-e8ba-4ee1-967e-4a577dde454d.png)

## CONNECT MYSQL TO DOCKER

1) Go to Command Prompt to download MYSQL image into Docker

![Screenshot (3)](https://user-images.githubusercontent.com/107701670/174435837-4db905c7-ed2b-4dae-bb3b-42ea2837cb97.png)

2) Login to Docker account and run MYSQL image script 

![Screenshot (1923)](https://user-images.githubusercontent.com/107701670/174435866-18526eda-933b-4b14-b8dc-ed01fb86912f.png)

3) MYSQL is now pulling into Docker

![Screenshot (1924)](https://user-images.githubusercontent.com/107701670/174435817-f0f05dcd-8241-4de8-9126-a8c1e22fa495.png)

4) Pull has completed and MYSQL has uploaded

![Screenshot (1925)](https://user-images.githubusercontent.com/107701670/174435894-5cb753ec-0e78-4c30-966e-d91012ee1fe3.png)

5) Open SQL WorkBench to connect your MYSQL account to Docker account

![WhatsApp Image 2022-06-18 at 7 52 59 PM](https://user-images.githubusercontent.com/107701670/174436603-78719f22-7bfb-44c1-8f5c-19289040306c.jpeg)

6) Put Username as Local Host and password you put before in your Command Prompt and you successfuly made the MYSQL connection

![Screenshot (1926)](https://user-images.githubusercontent.com/107701670/174435921-c663792f-6d13-4bd9-a8f7-4b9abc24fd9c.png)

7) MYSQL will be opened and ready to use

![Screenshot (1927)](https://user-images.githubusercontent.com/107701670/174435967-81a9b26b-48c1-412b-9e7c-a31eeb27917b.png)

8) MYSQL image is already in your Docker account

![Screenshot (1939)](https://user-images.githubusercontent.com/107701670/174435941-3cced452-a535-41c2-a987-bfcd5ae9fb0f.png)

9) Your container will show your MYSQL is running

![Screenshot (1941)](https://user-images.githubusercontent.com/107701670/174435949-69428f5c-a116-492b-9e43-c205e7e9a0cd.png)


Examples of code and commands start here






