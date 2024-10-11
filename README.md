# How to run the code

In order to run this code you need to have a Linux envitonment. This can be achieved by:
- Having a Linux as your or OS
- Installing WSL on Windows
- Running a Linux VM

In your linux envorinment, do:

1. Make sure you have all the necessary tools installed. You can run ```sudo apt-get install git build-essential gcc pkg-config cmake python``` in the terminal to install them
2. Get [vscode](https://code.visualstudio.com/download), if you don't have it already. If you are running on WSL, DO NOT install vscode directly in your WSL. Instead, open vscode in windows and add the [WSL extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl) to it
3. Install the [CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools) extension in vscode
4. Git clone [open62541](https://github.com/open62541/open62541) into the folder of your choice
5. Git clone this template INTO THE SAME FOLDER where you cloned open62541 in the previous step
6. Open the Open62541_template folder in vscode
7. Navigate to the CMake panel on the left and click Launch
   ![Skärmbild 2024-10-11 162604](https://github.com/user-attachments/assets/d460efe1-8346-4530-be3a-918a0c0b22f5)
8. The server should be running now and you will see output similar to this
   ![image](https://github.com/user-attachments/assets/e077cc0c-206a-4fd4-82bf-52595743ea8b)

9. Press Ctrl + C in the terminal window in vscode to stop the server. You should see an output similar to this
  ![image](https://github.com/user-attachments/assets/be698acc-5eff-4f99-8f34-0a73e208a029)


That's it! This template can be used as a starting point for working with open62541 tutorials, such as the [PubSub one](https://www.open62541.org/doc/v1.4.0/tutorial_pubsub_publish.html)
