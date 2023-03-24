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

then client next, enter acept and click change identity source
![image](https://user-images.githubusercontent.com/53860717/227478087-ac1afd8b-b1eb-4e7a-b0b3-5e8dc2268fdc.png)

after client enable automatic provissiong 
![image](https://user-images.githubusercontent.com/53860717/227478362-211063cb-724a-4fe2-bc54-978c524218df.png)

note the scim endpoint and token 
![image](https://user-images.githubusercontent.com/53860717/227478637-55dc77df-7d2d-4511-9136-14cf0a58e3da.png)

Step:-3 select provision and select configure api configuration
![image](https://user-images.githubusercontent.com/53860717/227479388-e2e27588-c4b2-4eeb-a148-bdcca897bac7.png)

select enable api integrations and enter endpoint with / after v2 like below and token then test api cred and save 
![image](https://user-images.githubusercontent.com/53860717/227480778-4f56cedd-eb93-4d9d-82f0-22f5c2233e91.png)


after that click edit and select create and update deactive users options 
![image](https://user-images.githubusercontent.com/53860717/227481261-7d78a33a-7268-4db2-aa87-4830e5d1b3fe.png)

![image](https://user-images.githubusercontent.com/53860717/227481419-92c688d3-f4e9-4a05-88dc-cc72ee7c89c9.png)

Sync okta to aws
![image](https://user-images.githubusercontent.com/53860717/227481551-1395d513-7d07-4758-8c17-7244784ea1ac.png)

Pushing the okta groups to aws like below by name 

![image](https://user-images.githubusercontent.com/53860717/227481810-ae5ed35a-06c0-4589-9033-8cfe37449ee5.png)


![image](https://user-images.githubusercontent.com/53860717/227482110-97a94a70-2c3b-4233-9baa-7209adf22cff.png)

save
![image](https://user-images.githubusercontent.com/53860717/227482273-a35248b3-7135-4ca1-b2eb-8e4a8cd8cfee.png)

![image](https://user-images.githubusercontent.com/53860717/227482333-14df7d99-79b1-4aee-bee2-41fced1bb627.png)

sync scim

![image](https://user-images.githubusercontent.com/53860717/227482600-ac8ebedb-144f-4ad9-bdaa-528404ed4ba6.png)




