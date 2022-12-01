# CLOUD NETWORKING 101

- Access the IIS server and host a simple website on the server


## PROCEDURES FOR CONFIGURATION


### Install IIS(For Windows Users)
- From the Windows start menu, open Server Manager.
- Click Add roles and features.
- Select Role-based or feature-based installation, and choose your server.

 ![Role Services](./Images/Images/IIS iNSTALLATIONS.png)

- Scroll through Server Roles and click Web Server (IIS).
- Add any additional IIS features you wish to install.
- Click Install to start the installation process.

![Installation](./Images/Domain%20Setting.pngImages/IIS Installation Progress.png)


### Create the web application
- Using Windows Explorer, create a new folder in the default IIS web server directory to store your domain's web files. For example, you could create a folder named ` C:\kamilimu\example.com `

### Setup the IIS Site with your Domain Name
- Open the Windows start menu and navigate to the Windows Administrative Tools subgroup.
- Select Internet Information Services (IIS) Manager from the list.
- In the IIS Manager Window, click > next to your server name to expand the list.
- Expand Sites, and click Add Website on the right Actions bar.
- Enter your Web Application name in the Site Name: field.

- Under Content Directory, click ... to browse and set the Physical path: to your domain web files directory.
- Keep http as the Type under Binding, and 80 as the port.
- To assign your domain a specific IP address, select it from the drop-down list, or keep All Unassigned to use all Server IP addresses.
- Enter your domain name in the Hostname: field.
- Click OK to save changes and automatically start the website.
- Visit your domain to confirm successful integration.
