# Initial Installation

If you have completed the Joomla deployment on Cloud Platform, the following steps is for you to start use it quikly

## Preparation

1. Get the **Internet IP** on your Cloud Platform
2. Check you **[Inbound of Security Group Rule](https://support.websoft9.com/docs/faq/tech-instance.html)** of Cloud Console to ensure the TCP:80 is allowed
3. Make a domain resolution on your DNS Console if you want to use domain for Joomla

## Joomla Installation Wizard

1. Using local Chrome or Firefox to visit the URL *https://domain* or *https://Internet IP*, start to install  

2. Set the site information and select language,then Cick “Setup Login Data” button
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard1-websoft9.png)

3. Set the user account inforamton
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard2-websoft9.png)
   > Email is your login ID, not collected by anyone because it stored in your Cloud Server

4. Then configure the database connection information([Don't know password?](/stack-accounts.html#mysql))
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard3-websoft9.png)

5. Click "Extra steps: Install languages" to install extra language 
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard4-websoft9.png)
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard5-websoft9.png)

6. Follow the prompts to set whether to enable the multi-language feature of the website and set the default front-back language

7. Click the “Remove installation folder” button

8. Log in Joomla backend (URL is *http://domain/administrator*)
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard6-websoft9.png)

9. You can use the Joomla backend to setup your site now
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-wizard7-websoft9.png)

> Refer to [Joomla admin_manual](https://docs.joomla.org/Main_Page) to get more details

## Q&A

#### I can't visit the start page of Joomla?

Your TCP:80 of Security Group Rules is not allowed so there no response from Chrome or Firefox

#### Which database does this Joomla package use?

MySQL

#### Can I use Cloud database for Joomla?

Yes

#### Joomla not the latest version?

Completed the Joomla initial installation, the login console can be updated online to the latest version with one click.