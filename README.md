# IIS_WebApplication_Project

Simple ASP.NET web application created using Visual Studio Community 2022 ASP.NET default sample.

## Description

Follow these steps to deploy the ASP.NET default sample on Windows Server running IIS Manager.

## Requirements
- [Git for Windows](https://objects.githubusercontent.com/github-production-release-asset-2e65be/23216272/29132429-5073-44c9-955b-32f89e6f7730?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20220602%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220602T201651Z&X-Amz-Expires=300&X-Amz-Signature=4f662e154753f77a434937e1d1f569f32dc35e7a5c0b36e3038753b182c11385&X-Amz-SignedHeaders=host&actor_id=106191513&key_id=0&repo_id=23216272&response-content-disposition=attachment%3B%20filename%3DGit-2.36.1-64-bit.exe&response-content-type=application%2Foctet-stream)
- Windows Server 2019 with IIS (Internet Information Services) Web Server role installed.
- DotNet 6.0 framework for the sample to work on the server , Download and install from [Here](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-6.0.300-windows-x64-installer)

# Installation and Configuration

#### Step 1 - Clone project.
- Create a folder for this project (Preferablly under C:\ or your OS DRIVE)
- Clone this repository locally by running ```git clone https://github.com/BenTest12/IISWebApplication.git``` in git.

#### Step 2 - Install and configure IIS.
 - Open the server manager , Sometimes the icon is not found at the desktop so we have to search it in the OS by pressing the start button and typing ```Server Manager``` , then in the server manager click on : ```Add feature and roles``` , Follow [This Guide](https://www.youtube.com/watch?v=s6pNP2x-lNY) to proceed with the installation procedure.

#### Step 3 - Add your web application to the IIS Manager.
- Open IIS manager
- Open your local connection.
- Right click on ``` Sites```
- Select add website
- Fill the website form.
  - ```Site name``` - Your website name.
  - ```Physical path``` - The path to your website folder (Preferablly (OSDRIVE:\inetpub\wwwroot)
  - ```port``` - Website port (For this project , Use port 5100)

#### Step 4 - Browse to the application

- From your local Microsoft machine Browse to ```http://localhost:5100/```
- You should be able to view the project in the browser.
