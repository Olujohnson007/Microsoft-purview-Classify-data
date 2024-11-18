
In this project I learned how to Identify sensitive content using trainable classifiers in Microsoft Purview information protection, governance and label application.

Trainable classifiers are machine learning models that are trained to categorize or classify data based on patterns and features identified during the training process. They are widely used in applications such as email filtering, document classification, and fraud detection.

 ![image](https://github.com/user-attachments/assets/b373d540-3eff-47f0-ae8f-15f18ef79362)

 ![image](https://github.com/user-attachments/assets/86279511-e0bd-442b-9a2e-ad564f992711)

 ![image](https://github.com/user-attachments/assets/88e3f7a7-7aaf-4a7f-a7b2-4ae85d641fad)



The agreement classifier Detects contents related to legal agreements, such as non-disclosure agreements and statement of work
 

 ![image](https://github.com/user-attachments/assets/680e67b9-ac68-4528-9cc1-959e6afba384)
 
![image](https://github.com/user-attachments/assets/887f66ff-fcd8-426f-8083-d92ed282dfdc)

![image](https://github.com/user-attachments/assets/9628f080-156b-4679-9d9b-4c040488aee3)

![image](https://github.com/user-attachments/assets/44bd578e-9fb9-4cda-8761-88aeb1cb6de2)

![image](https://github.com/user-attachments/assets/4f2724fe-6231-49b1-8b4b-d9578f480686)


 

 

 




The first Tab displays the documents metadata and the second  Source code Classifier page detects items that contain programming code in any of the 23 languages

![image](https://github.com/user-attachments/assets/4668fd04-0762-4469-9664-7bd3385055f3)

![image](https://github.com/user-attachments/assets/fec158b1-a414-466f-97b9-37078d4021b0)

 
 
In this next display I would begin to create a custom trainable classifier.
Trainable classifiers are machine learning models that are trained to categorize or classify data based on patterns and features identified during the training process. They are widely used in applications such as email filtering, document classification, and fraud detection.

 ![image](https://github.com/user-attachments/assets/c993e645-ec90-4313-bd3b-cb29cf39d010)


After clicking create, you would be required to provide a name and description of the Trainable classifier.
 
 ![image](https://github.com/user-attachments/assets/a355215b-23ab-4d4a-a37c-96941464f41e)


After putting in the name and description, I  would then provide seed content.
Purpose of "Seed Content"
•	Trainable classifiers in Microsoft Purview require seed content to learn and identify patterns in data. The classifier uses this content to train its model to recognize and classify files with similar characteristics.
Why Provide Seed Content from SharePoint?
1.	Content Source:
o	Seed content must come from a SharePoint site (or similar repository) because it serves as a centralized storage location for structured files like Word documents, PDFs, Excel sheets, and PowerPoints.
2.	Training Process:
o	The classifier analyzes the seed content to understand the defining features of files that fall under the category you want to classify. This step helps it generalize and classify other documents accurately.
3.	Enough content (between 50–500 files) ensures the model has enough data to learn effectively.
4.	Microsoft Purview will automatically process up to 500 of the most recently created files if the site contains more than 500 documents. This ensures that the classifier focuses on recent and relevant data.

![image](https://github.com/user-attachments/assets/c110a251-405f-4eb6-ba46-6eee6c6307c3)

 ![image](https://github.com/user-attachments/assets/c7f79e59-ccd6-4ddd-9578-f71c29b88739)


 


Click and add 

 ![image](https://github.com/user-attachments/assets/3346c2f9-854f-44b4-8490-0859f8ae97bf)



Select the folder containing the content

![image](https://github.com/user-attachments/assets/bb9d90e7-97ca-4308-9cb2-93ff5e61585e)
 

Click and add 

 ![image](https://github.com/user-attachments/assets/bb93570b-f43a-4a55-a82e-9f8e57399598)

![image](https://github.com/user-attachments/assets/8f988360-6d08-4c3a-a8f0-bd75ed2f4ada)

 

Review the Detailers and create the classifies

 ![image](https://github.com/user-attachments/assets/393ef433-599c-433e-a4b6-31f3c2dd6665)


The trainable classifier was successfully created.
Microsoft Purview is now processing the seed content provided in the earlier steps. This process involves:
Analyzing patterns in the seed files.
Building a predictive model capable of classifying other files with similar characteristics.
Processing Time
The process can take between 1 to 24 hours, depending on the amount and complexity of the seed content.

Next Steps
1.	Monitoring Progress:
o	The classifier's status will appear as "In progress" on the dashboard. You can revisit this status to see when the classifier is ready for testing.
2.	Testing the Classifier:
o	After the model is trained, you can test it on other content to ensure it accurately classifies documents according to your defined criteria.

 ![image](https://github.com/user-attachments/assets/3ffad87d-4e5a-4d4a-b048-f90048470cd0)




Next ,lets filter the list to find the classifier we just created

![image](https://github.com/user-attachments/assets/94ef9104-ed43-4969-9ea5-76aad9ccfce9)

![image](https://github.com/user-attachments/assets/1cae80e0-6d44-41f0-b2a5-330017cc81f7)
 

 

When the Classifier is finished processing the seed data the status changes to Need  test items
 ![image](https://github.com/user-attachments/assets/b99ed39b-0358-4a2e-94ad-af77f38f9398)

 
Next, add items to test the classifier
To train your Microsoft Purview content classifier:
1.	Gather data: Collect at least 200 test items, including good and bad examples.
2.	Organize: Create a dedicated SharePoint Online folder for test items.
3.	Train: Follow prompts to add locations and run the test.
4.	Review: Monitor performance, provide feedback, and refine the classifier.
Tips:
•	Diverse and balanced data is key.
•	Continuous improvement is essential.
By following these steps, you can create a powerful classifier to categorize your data effectively.

 ![image](https://github.com/user-attachments/assets/d6e04018-24f1-4a2e-9c9b-ca908fcf0467)

![image](https://github.com/user-attachments/assets/92e4fd72-7cb4-474b-8919-ae36e1f191d3)

 ![image](https://github.com/user-attachments/assets/fabdf3e0-32b9-4236-8687-7bbf4bbbca28)

 ![image](https://github.com/user-attachments/assets/3ce59c85-63f2-4ec7-8869-ce6b83e2120c)

![image](https://github.com/user-attachments/assets/70e17526-f67b-4aa6-9b77-65ab6e982f2b)

 ![image](https://github.com/user-attachments/assets/9206a9a8-5362-4514-a76a-6abf9bcb5607)

 

 

The predicted results are ready to review. To increase the test sample size, you can add items at the top of the page. The trainable classifier will take up to an hour to process the test files 

 ![image](https://github.com/user-attachments/assets/0dba048d-d43f-4922-8400-54ca1aedb1d9)



Next, Select Tested items to review
 ![image](https://github.com/user-attachments/assets/841cbf87-9b42-4c00-911c-617449c09f77)

 ![image](https://github.com/user-attachments/assets/d8234f79-88c8-4936-adaf-448db7ba63dd)

 
Next, you can indicate whether to agree or disagree with the match or if you are not sure
Microsoft Purview will automatically retrain the model based on your feedback  

 ![image](https://github.com/user-attachments/assets/24e1f90d-84f6-4ddd-89da-5cd129c3d59c)

 ![image](https://github.com/user-attachments/assets/748262b1-98f2-48b0-b6ec-234604ccc962) 

 ![image](https://github.com/user-attachments/assets/6e7a6e1c-0216-4cdc-ab69-8dffd06dbdbf)

 ![image](https://github.com/user-attachments/assets/dd881573-5a6b-47d6-9161-96234b5b9a77)





 
 
 


Based on the result of the review, a classifier accuracy score is generated 
 
  ![image](https://github.com/user-attachments/assets/16a3f024-bdbb-45bc-87ce-94102a6e869b)


  ![image](https://github.com/user-attachments/assets/6c3d4aa6-5950-4635-869b-f00a6c960158)

  ![image](https://github.com/user-attachments/assets/cdb3318e-a3f1-49bf-9220-d4ee04eb5550) 

  ![image](https://github.com/user-attachments/assets/47af020d-8c0c-42df-93d3-de9bb7ca5c5a)

  ![image](https://github.com/user-attachments/assets/abc445cc-dfa6-487e-8baf-948eb48486f5)


  



 
 
 

To examine the content collected by a trainable classifier, navigate to content explorer 

![image](https://github.com/user-attachments/assets/e6c554f4-d072-4dd0-b579-d1bb186483b0)



 

Collapse the section and select the source code classifier 

 ![image](https://github.com/user-attachments/assets/1f38d187-5f6b-4c22-a5e1-4f84d0b8f77f)

 ![image](https://github.com/user-attachments/assets/1843285a-5ac3-4bb1-ae08-8f7558653950)


 
Drill into the SharePoint folder
 
 ![image](https://github.com/user-attachments/assets/b0aa8223-f29a-45bc-9d9d-d617bbfd9a0a)

 ![image](https://github.com/user-attachments/assets/7eb7ad1f-597a-44d7-a752-6383f4f9b1f5)



Creating Label:   Let’s explore Microsoft Purview Information Protection and learn how to create a label using a trainable classifier.
 ![image](https://github.com/user-attachments/assets/7189b4ca-6d93-44d4-b122-fc32a0b13d89)

 ![image](https://github.com/user-attachments/assets/499aeaca-4411-48de-b8b2-45719e401cb6)


 



Next, create a sublabel within the group.

![image](https://github.com/user-attachments/assets/6759a713-ac56-49e0-aaa3-a53e2cacc417)


 
First, provide a name, display name and description

![image](https://github.com/user-attachments/assets/fae0c0d2-89ea-4e89-994f-c64c62679c8d)

 
Next, define the scope of the label. In this case we will keep the default
 
 ![image](https://github.com/user-attachments/assets/7064ad0f-a3e7-4435-8578-48bb12ec474a)



You can configure encryption and content marking settings to protect labelled items (skip)

 ![image](https://github.com/user-attachments/assets/e68c5590-5a44-4694-bc70-a757af77dd63)



Next enable auto-labeling for files and emails
 
 ![image](https://github.com/user-attachments/assets/cc089bbf-5120-43ae-b4f7-d63bb60e06b6)


Add a condition to detect content identified by the source code trainable classifier
 
![image](https://github.com/user-attachments/assets/24acd3e7-83fb-40fc-ada5-ae768523d6ac)

 ![image](https://github.com/user-attachments/assets/b1aed435-aea5-41fb-8162-ef9eaff4fbeb)

 ![image](https://github.com/user-attachments/assets/b68895b0-df65-4291-aac2-ab6f3afccb6c)

 ![image](https://github.com/user-attachments/assets/d1679fc3-d3bd-4f99-850b-b8d3b5a4bb86)

 ![image](https://github.com/user-attachments/assets/12142253-3a6a-44cc-85e7-de3a07798632)

 

Next specify what happens when the content matches the conditions
 ![image](https://github.com/user-attachments/assets/623dfa27-51b0-4a6f-809e-1d38724e8505)

 


In this case we recommend the users apply the label
 ![image](https://github.com/user-attachments/assets/d42af3c3-8055-45ff-a229-9bc828cbcdb3)



Next, enter a message to display to users when the label is applied
 ![image](https://github.com/user-attachments/assets/994468b9-1f4a-4746-bc9a-339f4dd4cc65)

 ![image](https://github.com/user-attachments/assets/75f07f1b-2ca9-4c5d-8829-5dba3f5279e6)

 

Here, you can specify the protection settings that should be applied when this label is used for teams, groups, or sites.
Technical note: These settings do not directly affect the files stored within these containers and do not impact downloaded copies of the files

 ![image](https://github.com/user-attachments/assets/e7db569d-0676-43ca-8c4d-fecd9edef5ac)


You can also enable auto labeling for schematized data assets in Microsoft purview data map

 ![image](https://github.com/user-attachments/assets/86203fd3-1ff7-40f2-8f4d-6258122cdafb)


Review setting and finish creating label
 ![image](https://github.com/user-attachments/assets/1266a402-7354-4bf9-aca2-c5551a84f1ef)

 ![image](https://github.com/user-attachments/assets/6045b9ee-d799-4edc-8a8f-2709a6ed360a)

 
Now let’s create a policy to publish the label to user’s apps so they can apply it to content.
In the policy creation wizard first choose the sensitivity labels you want to publish.
 
![image](https://github.com/user-attachments/assets/40809459-8b90-4cfd-9e76-02c6a92bf26a)


Next, select the Confidential label and the Source code sublabel created
 ![image](https://github.com/user-attachments/assets/4be88648-42d2-4466-9227-a833d2f02d1b)



Continue to the next step

![image](https://github.com/user-attachments/assets/5c25b4e1-a1f0-4df6-aeef-be27faf59808)
 

Next choose the admin units or set of users you would like to assign this policy to.
In this case we will keep the default and continue through the next steps.

 ![image](https://github.com/user-attachments/assets/e67be7b2-b233-4df9-89a8-b76e570dcdad)

Next, choose the users and groups to make the labels available for. We will include all users and groups.

 ![image](https://github.com/user-attachments/assets/1efef14d-e06e-4071-99ed-49be7dc6e98e)



You also have the option to further configure the policy settings. (skip)

 ![image](https://github.com/user-attachments/assets/465fe01e-5984-47d0-a97e-aaba4f9e6bdb)


Next name your policy 

![image](https://github.com/user-attachments/assets/b707ef0b-26a5-4ad2-a390-313fec398ecd)

 
Finally click and summit

![image](https://github.com/user-attachments/assets/45603b52-25b8-4f2b-87c8-9013f053d682)

 
The policy has been created and the labels will be published to the selected users apps.
