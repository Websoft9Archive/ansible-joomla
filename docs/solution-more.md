# More

Each of the following solutions has been proven to be effective and we hope to be helpful to you.

## Domain binding

The precondition for **Domain binding** is have completed the **Domain resolution** for Joomla Instance.

From the perspective of server security and subsequent maintenance considerations, the **Domain Binding** step cannot be omitted.

Joomla domain name binding steps:

1. Connect your Cloud Server
2. Modify [vhost configuration file](/stack-components.md#apache), change the domain name item for you
   ```text
   #### Joomla (LAMP) bind domain #### 

     <VirtualHost *:80>
     ServerName joomla.mydomain.com # modify it for you
     DocumentRoot "/data/wwwroot/Joomla"
     ...
     
   #### Joomla (LEMP) bind domain #### 

     server {
      listen 80;
      server_name joomla.example.com; # modify it for you
     ...

   ```
3. Save it and restart [Web Service](/admin-services.md#apache)


## Joomla languages

Joomla supports multiple languages. Here are the main steps to install and set up multiple languages:

1. Log in Joomla, go to【Extension】>【Language(s)】>【installed】, install the languages you want
  ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-bkinstalllan-websoft9.png)

2. Then set your default language of Joomla Site or Administrator
  ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-bkenablelang-websoft9.png)

## Joomla extension

[Joomla! Extensions Directory™](https://extensions.joomla.org/) provided lots of extensions for you:

1. Log in Joomla
2. Go to【Extensions】>【Install】>【Install from Web】and search the extensions
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-bkinstallext-websoft9.png)
3. Install them online

## Joomla install template

You can upload your template package to install it:

1. Prepare your template (.zip file)

2. Log in Joomla backend

3. Open 【Extensions】>【Install】, select the tab【Upload package file】to install template
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-upload_install.png)

4. When have completed the installation, go to 【Extensions】>【Templates】>【Styles】, enable your template as default template
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-bkenabletemplate-websoft9.png)

> Some template zip package may have the Joomla source code, at this time **Install template=Install Joomla**

## Joomla Cache

Joomla backend have cache management function, refer to this picture:

![](https://libs.websoft9.com/Websoft9/DocsPicture/en/joomla/joomla-opencache-websoft9.png)

## Joomla reset administrator password

If you don't remember your administrator password, please refer to the docs [here](https://docs.joomla.org/How_do_you_recover_or_reset_your_admin_password%3F/) to reset it