# Demo Page

## Assumption
+ Install Sitecore Link Manager SC 9.1-v1.0.zip first, If you want to follow this demo. Please install Sitecore 9.1.0 (rev. 001564) and Sitecore Habitat Demo Site(Habitat 1.7 Release).

## Getting Started

1. Login to the Sitecore Client using your prefered browser.

![image](https://cloud.githubusercontent.com/assets/2329372/26075898/d4ffd252-396b-11e7-8b89-5388328049e4.png)

2. In Sitecore Launchpad click on **Desktop**.

![image](https://user-images.githubusercontent.com/2329372/29325656-16fda4fc-821b-11e7-8270-b68963439398.png)

3. In Sitecore Desktop Click "Sitecore Icon" and then select Content Editor

![image](https://user-images.githubusercontent.com/2329372/29325732-5c1b6f2e-821b-11e7-853a-5d5af02a77d8.png)

4. In Sitecore Content tree in the left panel click on **sitecore/content/Habitat/Global/Teasers**. 

5. Since we are using Sitecore Habitat and Link Manager only work with external link we need to access Global where Teasers folder is located.

![image](https://user-images.githubusercontent.com/2329372/29325830-c23e4c86-821b-11e7-9d1b-486beee888f2.png)

6. Inside Teasers folder are Teaser component which is using external link in their content.
Click About Habitat(component) in the Content panel right below **Quick Info** click **Content** and scroll down look for **Teaser Link** and on Teaser Link kindly click **Insert external link**.

![image](https://user-images.githubusercontent.com/2329372/29325901-07469a22-821c-11e7-9d69-1064416fe7da.png)

![image](https://user-images.githubusercontent.com/2329372/29325882-f0a51b40-821b-11e7-8d84-85a4fdbfc580.png)

7. Inside "Insert External Link" dialog in the bottom part you can see we added Trigger Goal, Trigger Page Event, and Trigger Campaign and GTM(Google Tag Manager) using a CheckBox and also List of Goal, Page Event, Campaign and GTM using ComboBox.

8. Goal: if you check ✔ the checkBox it will set "True" and if not, It will set "False". If True you want to trigger the Goal; If False you don't want to trigger the goal. Goals are added to Combobox to create a list of Goal and it also uses a javascript that allows the user to "AutoComplete".

9. Page Event: if you Check ✔ the checkBox it will set "True" and if not, It will set "False". If True you want to trigger the Page Event; If False you don't want to trigger the Page Event. Page Events are added to Combobox to create a list of Page Event where user can select and it also uses a javascript that allows the user to "AutoComplete".

10. Campaign: if you Check ✔ the checkBox it will set "True" and if not, It will set "False". If True you want to trigger the Campaign; If False you don't want to trigger the Campaign. Campaigns are added to Combobox to create a list of Camapaign where user can select and it also uses a javascript that allows the user to "AutoComplete".

11. GTM(Google Tag Manager): if you Check ✔ the checkBox it will set "True" and if not, It will set "False". If True you want to trigger the Google Tag Manager; If False you don't want to trigger the Google Tag Manager. Since GTM allows you to trigger multiple events we added and list box so user can add multiple events.

12. If you click "Insert" it will create a "OnClick" from About Habitat Link in the Landing Page of the site. In this Image example I triggered the Goal, Page Event, Campaign and GTM at once, By checking each of designated CheckBox ✔ and Select a Goal(**Brochures Request**), Page Event(**Begin Transaction**), Campaign(**Register Page**) and lastly select two event in GTM which is (**Add_Campaign_Contacts_UploadGmail** and **Add_Campaign_Contact_Back**) and click **Insert** to update the changes in the external link.

![image](https://user-images.githubusercontent.com/2329372/29325940-27164816-821c-11e7-998d-7aa05417b440.png)

![image](https://user-images.githubusercontent.com/34522951/52430415-f92eb580-2b40-11e9-984f-2e1681942f61.png)

13. Click **Save** to save the changes. And Click Publish to publish the changes you made from the **Web**.

14. After clicking Publish button select **Publish Item** to publish the item you changes and the Publish dialog will pop out.

![image](https://user-images.githubusercontent.com/2329372/29326022-859bcb0e-821c-11e7-9778-6343299506d1.png)

15. In the **Publishing** select **Smart publish** and check ✔ the Publish subitems and Publish related items and then click **Publish** Button and click Yes.

![image](https://user-images.githubusercontent.com/2329372/29326104-d8b00a80-821c-11e7-8a43-4aa5e6390759.png)

16. After Publishing you will see a dialog box that indicates the item you publish and since I just update 1 Item only.

![image](https://user-images.githubusercontent.com/2329372/29326135-f9731ad2-821c-11e7-8167-bf1d22a6f556.png)

17. After Successfully publishing your changes. To your Instance web http://habitat.sc/ and in this Demo we are using Sitecore Habitat Demo Site. In the landing page, you can locate **About Habitat** below Sitecore Habitat Home Page in the footer section.

![image](https://user-images.githubusercontent.com/2329372/29326266-6846902e-821d-11e7-94aa-8f4404400bdd.png)

18. To check if the Teaser Link Button added OnClick Attribute on the html structure please use developer tool in Google Chrome F12. Use inspect button to inspect the Link.

![image](https://user-images.githubusercontent.com/34522951/52433480-22067900-2b48-11e9-9513-a5c77f850883.png)

19. To check if the Goal, Page Event, Campaign, and GTM is triggered, You need to click the Button first and look at the Sitecore Habitat Information Bar in the Right panel of the Site.

![image](https://user-images.githubusercontent.com/34522951/52435057-c9d17600-2b4b-11e9-9e78-898234e30b43.png)

20. After clicking the Information Bar just click **Refresh** and Click **Onsite Behavior Panel** to see the Triggered Goals and Page Events.

![image](https://user-images.githubusercontent.com/2329372/29326373-db4bce0e-821d-11e7-8dfc-159c4865cde0.png)

21. Goals that had been triggered.

![image](https://user-images.githubusercontent.com/2329372/29326417-fd57ee10-821d-11e7-9f2f-ef20160de85c.png)

22. Page Events that had been triggered.

![image](https://user-images.githubusercontent.com/2329372/29326445-1c154d5c-821e-11e7-87ce-893f7a37e3f9.png)

23. You can check triggered campaign in **Referral Panel**.

![image](https://user-images.githubusercontent.com/2329372/29326461-2ccd2796-821e-11e7-887a-95ca048f6e1b.png)

24. You can check triggered GTM in Google Chrome Console Tab by just typing **dataLayer**.

![image](https://user-images.githubusercontent.com/34522951/52434739-0fda0a00-2b4b-11e9-9692-40bc1853af34.png)

25. End

## Supports
+ For support please email the author or [create an issue](https://github.com/JairoSolutions/LinkManager/issues/new).
+ Tested on Sitecore.NET 9.1.0 (rev. 001564) with Habitat Demo Site(Habitat 1.7 Release. A Sitecore project implemented on the Sitecore Experience Platform using Helix Framework).

THIS MODULE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT SUPPORT, WARRANTIES OR CONDITIONS OF ANY KIND.