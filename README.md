# WindowServer2025_SharedFolderMappedtoLocalHost_FileServerCreation

## Objective
[Brief Objective]

### GitHub Project Description

This project aims to develop a file server that facilitates file sharing between multiple machines connected to the same network. It will also include implementing a shared folder that can be easily accessed and mapped directly to the local host machine. This setup will enable seamless collaboration and file management, allowing users to efficiently store, retrieve, and share files across different devices.

The project aims to enhance the experience of setting up a file server by focusing on several key components:

- **Installing Roles and Features for File Sharing**: This involves selecting and implementing the necessary server roles and features that facilitate efficient file sharing across the network. 

- **Setting Up User Permissions**: In this step, we will assign the appropriate permissions to users, drives, and folders. This ensures that users have the right level of access to the shared resources, enhancing both security and functionality.

- **Creating and Mapping Shared Folders**: We will establish a shared folder that multiple users can access. The process also includes mapping this shared folder from the Virtual Machine to the local host, allowing for seamless integration and ease of access.

This project aims to streamline the learning process and effectively apply best practices for creating a robust file server. This includes understanding how to appropriately assign permissions and accurately map files and folders to optimize user experience and maintain system integrity.

[Tools Used]

VMware
Server Manager 
File Server Resource Manager
## Steps

[File Server Setup]
Start by launching your Virtual Machine. Once it's up and running, navigate to Server Manager, the central hub for managing your server environment. From there, locate and select the option to add roles and features. This feature allows you to expand the functionality of your server by installing various roles and features that suit your needs.

 ![image](https://github.com/user-attachments/assets/0b3494ce-f91c-4983-aa38-2cc363541426)
![image](https://github.com/user-attachments/assets/001e412f-49cb-4b19-af24-2d522f836df0)
![image](https://github.com/user-attachments/assets/01fe7490-c4e3-4586-b26d-8ef5f31202c3)

 
 

To proceed with the installation, navigate to the Server Roles section and select the following options: DNS Server, Files and Storage Services, File Server, File Server Resource Manager, and Storage Services. After making your selections, click "Next" to continue. Once the installation is complete, restart your computer to apply the changes effectively.

 
 

To access the File Resource Manager, begin by launching the Server Manager. Once you're in the Server Manager, navigate to the "Tools" menu at the top of the interface. From the dropdown options, select "File Resource Manager." This will open a comprehensive management console where you can effectively oversee all your file and storage resources, allowing you to monitor usage, set quotas, and manage access to ensure optimal performance and security.
 
 ![image](https://github.com/user-attachments/assets/1e05ab09-1d26-4a7b-9a61-740ba5aa0975)
![image](https://github.com/user-attachments/assets/29e17e24-2c55-431a-b993-20fe22a604c5)


To begin, launch the File Explorer on your computer and locate the Z drive in the navigation pane. Once you've accessed the Z drive, proceed to create a new project folder by right-clicking and selecting "New Folder." This folder will serve as the main directory for your project. Inside this newly created project folder, you'll need to establish a subfolder explicitly dedicated to Windows Server 2025. This subfolder will be the designated location for storing all files and resources related to that server version, ensuring they are organized and easily accessible.

![image](https://github.com/user-attachments/assets/36b581b7-a60a-46d0-94e1-5f67b47f39be)
![image](https://github.com/user-attachments/assets/009c96f6-9fc9-438e-bcbe-73eaecea68eb)


After creating the Windows Server 2025 folder, right-click on it and select the "Share" option from the context menu. This will allow us to set up sharing properties for the folder. Next, we will map the local server path to this shared folder and assign the necessary permissions to ensure proper access.

Once these steps are completed, a new network path will be created under Network, allowing users to easily access the Windows Server 2025 folder while on the same network.

 ![image](https://github.com/user-attachments/assets/7d5873cf-957e-4021-909e-ea4d66338361)
![image](https://github.com/user-attachments/assets/0f625125-1dba-4f98-844c-fa3edb7ccf4f)
![image](https://github.com/user-attachments/assets/ff380b71-0f5f-4d21-b387-756727aee700)
![image](https://github.com/user-attachments/assets/31fccad7-7af4-4841-8c1e-01584876a232)
![image](https://github.com/user-attachments/assets/a6150d0a-0124-4551-9c6f-53fd7d2cd938)
![image](https://github.com/user-attachments/assets/9efdc697-c910-4594-bd87-c21a5cd04fd3)



 
 

 
 
 



[Shared Folder to Local Host]

To get started, open VMware Workstation on your computer. Once the application is running, go to the menu and choose the option to edit the settings of your virtual machine. In the settings window, find the section labeled "Shared Folders." Enable the shared folders feature by selecting the option to keep it "always enabled." Additionally, check the box that allows you to map these shared folders as a network drive in your Windows guest operating system. After making these selections, click on the "Add Folder" button to specify which folders you would like to share.

 

 ![image](https://github.com/user-attachments/assets/bb689e4c-e044-4d7a-b357-99faaec247cb)

![image](https://github.com/user-attachments/assets/e40ba9c1-b78e-465e-bcd2-9a15fd657244)

![image](https://github.com/user-attachments/assets/a9d55da8-fa46-4c47-8b0f-73a02f4b64a5)

![image](https://github.com/user-attachments/assets/6a601e55-05e5-46a4-9c1a-3ee81361a1a6)



 

 

After you have successfully mapped your folder, click "OK" to finalize the process—next, open File Explorer on your local computer. In File Explorer, you will find the shared folder that has been mapped to your Windows server. 

Once you've located the folder, right-click on it to bring up a context menu. From this menu, select "Properties." This will open a new window where you can manage access rights for the folder. Navigate to the "Security" tab in this window and click on "Edit" to adjust permissions. Here, depending on your needs, you can grant different access levels to specified users, such as full access, read-only permissions, or even deny access altogether. This process ensures that only authorized individuals can interact with the folder in the way you intend.
 
 ![image](https://github.com/user-attachments/assets/5eb7f287-0b21-4042-af03-14b24152a7c4)

![image](https://github.com/user-attachments/assets/127553d7-3108-4f41-83ae-4e36e2070dcd)

![image](https://github.com/user-attachments/assets/1e5ad049-118a-47c8-a522-d50e74d1da37)
 

After the process is complete, click "OK" to proceed and access the designated folder. In this step, we will create several files within the shared folder located on our local host, which will allow us to view them on the VM Server. Once the files have been successfully created, launch your Windows Server. From there, navigate to the shared folder to see the files that have been imported or newly created on the local host. This will enable seamless interaction between the local environment and the virtual server setup.

**Local Host**

 ![image](https://github.com/user-attachments/assets/f9f057c1-0ab8-4cf5-83f2-d27333f8f554)



**VM Server**
 
 ![image](https://github.com/user-attachments/assets/087c7a27-f742-4081-add4-abe6a4883cf3)

 ![image](https://github.com/user-attachments/assets/0c34b4ab-f460-4cec-b874-aacb125a6032)
![image](https://github.com/user-attachments/assets/312732a2-5ccd-4eba-a28c-67340eaea604)


This concludes the process of transforming the Windows server into a fully functional file server. During this setup, a shared folder was successfully created, allowing easy access to resources on the local host. This configuration enables users to store, retrieve, and manage files efficiently within the shared environment. 
