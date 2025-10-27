Active Directory Fundamentals: Creating Users and Handling Real-World IT Tickets

Let’s start with adding real users. I’ve successfully added users to my IT department, but I’m going to add more to my organization.

First, let’s add the Department as an OU.
![1_R3hKvoN5EeWHKJMPw9dZjg](https://github.com/user-attachments/assets/d6d6b911-93c1-4c89-9cd0-9470c051067e)
Right click the domain, select new, choose OU
![1_DRU4SyPZdXODg4tBjA0JhQ](https://github.com/user-attachments/assets/ff7fe433-52b3-4e6a-ab24-921d8f912407)
Make the OUs name

I have created the HR department and included HR Admins, HR Computers, HR Groups, and HR users.

Now let’s add users.
![1_xMsOb7CwfGoIsrd6QbazpA](https://github.com/user-attachments/assets/0d0e9110-541a-443d-9581-8521f57bf570)
Right click on OU you made, new, user
![1_MxxQK0EbJlWWoRk-s1REwg](https://github.com/user-attachments/assets/352e3a8f-994e-4db6-9e32-7af500762d6e)
![1_VyvclJS3doOyCF5BvQz_ww](https://github.com/user-attachments/assets/4584c591-f7d6-4aa8-a622-2c7f6a33fbcd)
Make sure you have a the “User must change password at the next login” checked.
![1_fMNhZEhZsFjOy42PILNnBA](https://github.com/user-attachments/assets/7a99e826-cd8d-48c2-9ec3-a4726edb07d7)
We have successfully added the new user to the HR Users!

While looking for Real World IT tickets scenarios that I may come across, I found this youtube: https://www.youtube.com/watch?v=Yb__4XttW7g

Following along with the video, we will use Find options, explore Advanced Features, and create Service Accounts.

***Find Objects: Users, Computers, Printers:***
A Ticket came in from Ava stating she is locked out of her account after having three failed attempts.

Right-click on your domain and select Find
![1_i20jvQEGDWQOMaUUsZO1xA](https://github.com/user-attachments/assets/4daa810b-b762-4aee-a3ec-20be2c5f4236)
Choose what you are looking for

![1_OKP36XIb9H5iPx4N3hOjFQ](https://github.com/user-attachments/assets/93e9f88a-c9e8-4a81-86c9-f892d9f46e40)

Click on the name to open an account
![1_uOtpN-Gb7ebFtNrkenFo0A](https://github.com/user-attachments/assets/ad85bd57-c2d5-43fa-99fc-e062567343f1)

Go to the “Account” tab and click the “Unlock account”, Apply the changes.
![1_2vKvgG1DnFLVhso8JPfmSA](https://github.com/user-attachments/assets/172fed0c-cdcb-4f81-83e0-b7658481147b)

Ava still can’t log in and needs to reset her password. This time in Find, right-click on her name and choose Reset Password.

![1_iKPTeF-mOkUa4i5szslH5w](https://github.com/user-attachments/assets/509605de-a696-4866-b222-dcd6080eed66)

This time we reset her password, and we will click “User must change password at next logon” as well as “Unlock the user’s account”

![1_pO_PPQoLUTuOmYQVMguGyg](https://github.com/user-attachments/assets/5c919de4-c935-40fa-a623-09e525f1c7d7)

Ava was able to log in and change her password!

A new ticket came in saying Ava is now moving from the HR department and going to the Service department.

We can make this change easily in AD
![1_xJaqrtrGv1Hl-LQG_8SBzQ](https://github.com/user-attachments/assets/a22ac783-5159-4343-ac83-e8ecd6709ea6)


We right-click her name and choose move. Then we select where we want to move her too!

![1_YV35wT1cOMAU2HbpgXyk0w](https://github.com/user-attachments/assets/6f627387-8059-4840-ad70-448c142b3ec1)

To double-check this move, we go to Service users.

![1_h1QjKAPjgEr8JwLEymTfLw](https://github.com/user-attachments/assets/e8aadbb8-3fa9-48c2-b4b2-ecbea0931f23)

She is in there! Now we want to make sure that she has the correct groups for her new role and remove any groups she can not have access to from her old role. We can do this by comparing Sage’s account to Ava’s and removing/adding the groups needed under the “Member Of” Tab.

***Advance Features***

![1_eJDxEIyIVVH5BpSXqFnpHA](https://github.com/user-attachments/assets/12bea801-acbb-4731-95a7-46ac4b9f1aa2)

Right now, we don’t see the Object Tab. Let’s enable Advanced Features.

Click on “View” and choose Advance Features.
![1_XGi8tL1GyWvGIZjWP5caAA](https://github.com/user-attachments/assets/d37a2367-26f0-484b-8ff1-1ebad7daed85)

Advance Features will also show us more Tabs in properties. Let’s look at Attribute Editor.
![1_nPb_K7HzOMnEXCa2RpjmZg](https://github.com/user-attachments/assets/70f4f0a3-b18e-475e-9b42-13685847f0e6)

Attributes let us see and set more parameters for users. We can also set a filter by values to make searches easier.
![1_6max_uu3zDA9Atq-3Fx4Cg](https://github.com/user-attachments/assets/390b6c51-f5c4-43f7-b2fa-286e1d60b51d)

***Adding Service Accounts***
First, let’s create a new OU.

![1_ZJJfRf_OihVI6O9WcRWFrw](https://github.com/user-attachments/assets/043ee879-3221-4a8b-9f1a-72d8ee7f96fc)

And then add a new User
![1_maBPkPg-KsJ4YVnvQvIaxg](https://github.com/user-attachments/assets/dfdbab52-61ff-4b1e-a02f-dffc7e9d2713)


Special characters are used so we can tell which one is a server account and which ones are user accounts

![1_GhQRdGsxt6PA829HUXFYQQ](https://github.com/user-attachments/assets/ad7d48e8-523f-4ea2-8b16-bf29ec4d78b3)

When setting a password, make sure you uncheck “User must change password at next login” and check “password never expires”.
![1_4YADOeWTiD6cd-eps3-v1Q](https://github.com/user-attachments/assets/1f94d424-6d6b-4767-a973-c9b2b2d669e0)
Now, for this account, we can apply logon permissions.

Go to account, logon hours,
![1_b9F8VvnZcPpdAX4KDVufpw](https://github.com/user-attachments/assets/518737f6-83f2-42e8-a419-cbed1d01a537)



![1_ALDHOr5v4v7gKLDIxs3dyg](https://github.com/user-attachments/assets/b2f32c3f-cb6a-41b9-9d86-42a4792a40ca)

**Copy Users***
The Service department hired a new member. To make things easier, we are going to create the new user with all the permissions a current employee has.

![1_BPNc_cckKZEsC357VQcSUA](https://github.com/user-attachments/assets/55619612-5825-4af7-adf1-e8c0fe992b63)

Right-click on a member, copy, and create new account. Then double-check that all groups moved over all well.

***Wrap-Up***
By completing these tasks, I’ve practiced essential Active Directory operations that IT and help desk professionals handle daily — from managing users and OUs to resolving real-world tickets efficiently.

