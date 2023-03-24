# sso_process_okta_to_aws
sso_process_okta_to_aws

##Step:-1 Enable IAM Identity Center (successor to AWS Single Sign-On) at AWS Portal
![image](https://user-images.githubusercontent.com/53860717/227470847-29618c04-e326-4ee3-93d9-5b04c9a8646f.png)


After select enable then client Choose your identity source option
![image](https://user-images.githubusercontent.com/53860717/227471450-0d742072-65b5-4b74-a406-193ff3970600.png)

then, click action and change identity source
![image](https://user-images.githubusercontent.com/53860717/227471749-441b2ec6-59ce-40dd-b55a-a2ef3f5a1afc.png)

after that select external identity provider 
![image](https://user-images.githubusercontent.com/53860717/227472032-f07e62c7-ae60-4ff3-8b0c-2b505bbed8fa.png)

next, note the acs and issuer url 

![image](https://user-images.githubusercontent.com/53860717/227472592-85143c45-91cb-4d01-aac0-5f806da44ae2.png)

Step:2 Okta  Need to add aws identity center
![image](https://user-images.githubusercontent.com/53860717/227474253-e8bed870-40f0-49a0-b431-a46808fe48a8.png)

ADD integrations > done

![image](https://user-images.githubusercontent.com/53860717/227474512-060ac16d-1d52-413b-ae89-c8386f647a33.png)

select sign on > click edit 
![image](https://user-images.githubusercontent.com/53860717/227474741-29b1b312-ba21-410f-8bee-ef8ce34223c5.png)

enter above aws acs and issuer url at advanced sign on settings 
![image](https://user-images.githubusercontent.com/53860717/227475317-a5f3f60d-7f93-44a7-9b6b-2b2f1935f522.png)

Then save 
![image](https://user-images.githubusercontent.com/53860717/227475497-4f9d8e6f-77f4-48da-bac0-331665701630.png)

under saml signning certificate download and view ldp metadata
![image](https://user-images.githubusercontent.com/53860717/227475931-963e0c8d-6459-4277-b263-859c35f6abb9.png)
note issue and sign url 
![image](https://user-images.githubusercontent.com/53860717/227476723-02125b7e-c3e2-41c4-ac58-7941d64f48de.png)

enter okta sign and issue url and upload the okta ldp certifcate under identity provider metadata
![image](https://user-images.githubusercontent.com/53860717/227477508-9c8acb22-1d66-4ee2-936f-8ee8e7753e8e.png)





