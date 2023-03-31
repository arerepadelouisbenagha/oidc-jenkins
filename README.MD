# SSO setup

Step - 1 Install `SSO plugin` on jenkins
Note: Install this lugin with a restart.
![pic-1](images/pic-1.png)

step - 2 Create Jenkins as a provider, click on `miniOrange SAML SSO`
![pic-2](images/pic-2.png)
![pic-5](images/pic-5.png)

step - 3 create an enterprise application in azure, and click on SSO to get started
copy over the details found on `miniOrange SAML SSO` to attribute claims in your enterprise application.
![pic-3](images/pic-3.png)
![pic-4](images/pic-4.png)

step - 4 copy the metadata over to jenkins from your app registration, paste it on `IDP configuration` in jenkins
paste it on `Enter metadata url:` then click on `validate metadata url` and click on save.
![pic-6](images/pic-6.png)

step 5 - go to manage jenkins and click on `miniOrange SAML SSO` click on it and test you configuration, it should be successful as shown below:
![pic-7](images/pic-7.png)
![pic-8](images/pic-8.png)
![pic-12](images/pic-12.png)

step - 6 Add users to your enterprise application , to allow users access to the jenkins SSO dashboard.
For external users, they get invited to your azure tenant via invite.

![pic-9](images/pic-9.png)


Note:
Invited users must accept thier invitations and also complete testing to jenkins SSO dashboard.

Successful login would look like this, users most lkely should have outlook emails.

![pic-10](images/pic-10.png)
![pic-11](images/pic-11.png)

