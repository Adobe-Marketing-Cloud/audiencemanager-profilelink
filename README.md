<h1> Lab scenario </h1>

Congrats! You have been appointed as the new Marketing Manager on PopularRetailer. It’s now your mission to individualize your customer experiences on your brand.
As part of your journey, you will need to understand your audience, spot those traits that best define it and perform segmentation based on the different interests. Using these segments, you will be able to delight your consumers with personalized offers and products across devices.
Luckily, you have an ace in the sleeve and that is: Adobe Audience Manager.

---
![slide03](https://cloud.githubusercontent.com/assets/952836/24138447/7525687c-0dd5-11e7-81be-3f76d54727f2.jpg)
---

---

<h1>Chapter 1 - Onsite personalization based on cross device activity</h1>

Objectives:
- Collect unauthenticated data across devices and merge it together with authenticated data
- Perform onsite personalization based on the merged profiles 

---

<h1>Login to Adobe Audience Manager</h1>
PopularRetailer is using Adobe Audience Manager to segment and activate their audiences.

Open the Google Chrome browser and go to the Audience Manager website: [https://bank-beta.demdex.com](https://bank-beta.demdex.com). 

For this demo we are going to use the Beta environment in Audience Manager, which is sandboxed from production. This is the place where we get to experiment with AAM, play with new features and ideas.

Your iMac is assigned a number between 1 and 50. Find out your number and use it to login:

- **Username:** summit2017-**99** (replace **99** with your iMac number)
- **Password:** AdobeSummit$2017

_Note: If your computer number is less than 10, let‘s say 5, then use 05._

<div align="center"><img src="https://cloud.githubusercontent.com/assets/952836/24138632/35fe96d6-0dd6-11e7-89a0-c7ece2a2e93f.png" align="AAM Login" height="300px" width="300px" ></div>

---

![slide05](https://cloud.githubusercontent.com/assets/952836/24138735/9a5ce632-0dd6-11e7-88bf-c9d920e69b31.jpg)

---

<h1>About Adobe Audience Manager (part 2)</h1>

**1. Create traits**

- These are the building blocks for understanding your audience
- Examples: 
  - Trait 1: Gender is female
  - Trait 2: Is athletic

**2. Create a profile merge rule**

- The traits can be stored in different kind of profiles such as:
  - Authenticated profiles (contain authenticated activity only, using a masked identifier)
  - Device-level profiles (contain only anonymous activity)
- The profile merge rule defines the way we combine these profiles together

**3. Create segments**

- You can segment your audience based on the individual traits
- Examples:
  - Segment1: Trait1 AND Trait2 (All the athletic females in the audience)
  - In order to know which profiles to use, each segment is linked to a profile merge rule

---

<h1>Step 1. Create traits</h1>

- To speed things up, we have pre-created for you the traits needed for this demo.
- Feel free to navigate and inspect them in the Audience Manager User Interface.
- You may also create new traits.

![AAM Traits](https://cloud.githubusercontent.com/assets/952836/24138849/1a31d5ca-0dd7-11e7-9e2a-aba32f0f84c9.png)

---

<h1>Step 2. Create a profile merge rule</h1>

- The profile merge rules defines the way we combine the different kind of profiles.
- When creating a profile merge rule, you need to pay attention to the sensitivity and context of your product. How you might want to combine data across devices might differ very much depending on whether you are selling ringtones or whether you are selling wedding rings. If I found out that my sister is interested in Rihanna, that would not be at all a surprise. If your girlfriend finds out that you are about to propose to her because of some activity where you were searching for wedding rings on another device, that would be pretty upsetting.
- For our demo, the PopularRetailer wants to go broad and use the data that’s available in the authenticated profile along with the data present in the device-level profiles.

---

<h1>Step 2. Create a profile merge rule (part 2)</h1>

- In the AAM User Interface, click on the “Profile Merge Rules” tab.
<div align="center"><img src="https://cloud.githubusercontent.com/assets/952836/24138964/76f5d7de-0dd7-11e7-8fb1-c8ee23041d11.png" align="Merge Rule" height="342px" width="433px" ></div>
- Then in the UI, on the right click “Add new rule”
<div align="center"><img src="https://cloud.githubusercontent.com/assets/952836/24138969/79d87b0a-0dd7-11e7-84fc-46417fb1124f.png" align="New Merge Rule" height="150px" width="350px" ></div>
- You should now be seeing the Profile merge rule creation wizard.

---

<h1>Step 2. Create a profile merge rule (part 3)</h1>

![New Merge Rule 2](https://cloud.githubusercontent.com/assets/952836/24139043/c68f96b8-0dd7-11e7-85f7-0d36ecbe7985.png)

---

<h1>Step 2. Create a profile merge rule (part 4)</h1>

- Congrats, you have now created your first profile merge rule for PopularRetailer.

- _Note: The number of profile merge rules that can be created is set to 3. This means you are not going to be able to save your profile merge rule. No need to worry though, we have pre-created the same profile merge rule to be used on the demo website._

---

<h1> Step 3. Segments </h1>

Step 3. Segments
**For our demo, we have already pre-created 6 segments:**

1. Athletes
Segment rule: Athletic trait
2. Female Athletes
Segment rule: Athetlic trait AND Female trait
3. Male Athletes
Segment rule: Athetlic trait AND Male trait
4. Sales
Segment rule: Interested in Season Sales trait
5. Female Athletes interested in the Season Sales
Segment rule: Athetlic trait AND Female trait AND Interested in Season Sales trait
6. Male Athletes interested in the Season Sales
Segment rule: Athetlic trait AND Male trait AND Interested in Season Sales trait

![Male Athletes interested in the Season Sales](https://cloud.githubusercontent.com/assets/952836/24139214/800b096a-0dd8-11e7-8de8-c5c620215cef.png)


---

<h1>Time to go on the demo website.</h1>


**Demo step 1.** Open the Google Chrome browser.

**Demo step 2.** In the Bookmarks bar, you should see the Demo Website. Click on it, or click here [AAM Demo Website](http://summit.demdextest.com). Since you are a first time user, you should now be presented with the "Common" experience.

![Common Experience](https://cloud.githubusercontent.com/assets/952836/24172744/94ccb0d8-0e46-11e7-9f28-9f57e7bd0ce0.png)


---

<h1>Demo step 3</h1>

Let's get you qualified for the "Athletes" trait. On the bottom, you should see a blog article: Tips for athletes. Click on it.

![Athletic trait](https://cloud.githubusercontent.com/assets/952836/24139326/e8820886-0dd8-11e7-8bc3-851e1e6178b5.png)

---

<h1>Spotlight</h1>

- We have instrumented the Athletes blog page to send a signal to Audience Manager. Based on this signal, your profile has been augmented with the “Athletes” trait. This trait was precreated in the UI.
- Note that you can enhance your audience profiles even further, by acquiring 3rd party data through Audience Marketplace. This can be geographic, demographic and behavioral data. It includes location, age, gender, income, spending patterns and more.

![Athletic trait](https://cloud.githubusercontent.com/assets/952836/24139349/041ce390-0dd9-11e7-980f-d28728f20fa5.png)

---

<h1>Demo Step 4</h1>

Go to the home page by clicking the brand logo. Based on the Athletic trait, you should now see a customized offer with workout clothes for men & women.

![Athletic clothes for both man and women](https://cloud.githubusercontent.com/assets/952836/24172806/d8b2173e-0e46-11e7-97e7-63e8f36534fc.png)

---

<h1>Spotlight</h1>

- Based on the Athletic trait that we have qualified for, we’re also qualifying for the Athletic segment. We don’t know yet if the end-user is a man or a woman, hence we’re displaying the workout clothes for both genders.
- To achieve the onsite personalization, the Audience Manager segments can be exported to Adobe Target, which has powerful ways of achieving customizations based on this information. You can notice the power of this Marketing Cloud integration. You can choose to export your Audience Manager segments to any other destination you would like, including 3rd party solutions.

---

<h1>Demo step 5</h1>

- Let’s now authenticate on the PopularRetailer demo website. Click on the Login button at the top of the demo website.

Your iMac is assigned a number between 1 and 50. Find out your number and use it to login:

- **Username:** summit2017-99-female (replace 99 with your iMac number)
- **Password:** Adobe#2017


_Note: If your computer number is less than 10, let‘s say 5, then use 05._

---

<h1>Demo step 5 (continued)</h1>

Once you login, you become known to the website on the current device. This means, we can now present an offer by combining your authenticated profile and the device profile. The authenticated profile contains a trait: Gender is female. The device profile contains the Athletic trait. Based on these two, we can now present an offer with Workout clothes for women.

![Workout clothes for women](https://cloud.githubusercontent.com/assets/952836/24139488/7cce18ae-0dd9-11e7-9cff-689fe3a32b04.png)

---

<h1>Spotlight</h1>

- We’ve now actually been using the profile merge rule that we have defined earlier. This combines the Authenticated profile with the Device Profile. The Authenticated profile contains the Gender is female trait. The device profile contains the Athletic trait.
- By combining these two together, we’re getting qualified for the Women athletes segment. Based on this segment, we perform the website customization, resulting in the offer for Workout clothes for women.

---

<h2>What happened here?</h2>

- By sending a cross-device customer id (`d_cid`) we have notified Audience Manager that this represents authenticated activity. This means all traits will be stored keyed of the authenticated id. 
- Moreover since we included both a device id (`d_mid`) and a customer id (`d_cid`), an id synchronization was performed, tying these two ids together.
- You can see that two profiles were detected: one representing the unauthenticated device profile (`89334862240161643561259517779946724685`) and the other one representing the authenticated profile (`summit-110-female`).
- Our profile merge rule specifies that these two profiles should be merged together. This means all the traits will be merged together in a super-set, before applying the segment rules.
- We can see that the [Athletes (ID: 5923408)](https://bank-beta.demdex.com/portal/Segments/SegmentBuilder.ddx#view/5923408) segment was qualified.

<h2>PII data</h2>

- In our case the customer id (`summit2017-99-female`) is a safe alphanumeric string, which does not contain [PII data](https://en.wikipedia.org/wiki/Personally_identifiable_information). In order to comply with regulations, Audience Manager prohibits onboarding PII data. 
- If the customer ids were to contain PII information (eg. real names, email addresses etc.), we would first ngeed to perform a [one-way hash](https://en.wikipedia.org/wiki/Cryptographic_hash_function) of the PII data (which will make it infeasible to invert) before sending it to Audience Manager.
- Therefore, instead of sending `d_cid=...john.smith@gmail.com` we would send `d_cid=...one_way_hashed_version_of_the_email_address`.

---

<h1>Demo step 6</h1>

- Log off from the current account. Click the “Logout” button at the top.
- Once you log off, we are not going to take into account the authenticated profile anymore. This is because the profile merge states we should use the Current Auhenticated Profile + Device profile. Therefore, while logged out, we only have access to the Device profile (which contains the Athletic trait). We are ignoring the contact to the authenticated profile, which states the the current visitor is a woman. As such, the experience changes back to Workout clothes for both men & women.

![Athletic clothes for both man and women](https://cloud.githubusercontent.com/assets/952836/24172806/d8b2173e-0e46-11e7-97e7-63e8f36534fc.png)

---

<h1>Spotlight</h1>

- It’s possible to use the authenticated profile even after the customer has logged off. This is achieved by creating a profile merge rule that is setup to use the **Last authenticated profile**, rather than the Current authenticated profile. In this hands on lab, we’re sticking with the Current authenticated profile only. 
- However even after the session ends, you will still have access to this demo. Feel free to take the time and explore these concepts further.

---

<h1>Demo step 7</h1>

After logging of, let’s now login with a different account, which is already qualified for the **Male** trait.

- **Username:** summit2017-99-male (replace 99 with your iMac number)
- **Password:** Adobe#2017

After you login, go to the home page, by clicking on the PopularRetailer brand logo on top left. You should be seeing an offer with Athletic clothes for men.

![Athletic clothes for men](https://cloud.githubusercontent.com/assets/952836/24172888/2c0944fc-0e47-11e7-9117-bc5e45429312.png)

---

<h1>Spotlight</h1>

- After logging in with the male account, the Authenticated profile has actually changed. This profile now contains the **Gender is male trait**. This trait was onboarded from the PopularRetailer CRM.
- By combining the **Male** trait with the **Athletic** trait, we’re now getting qualified for the **Men athletes segment**. As such, we’re now displaying an offer with _Athletic clothes for men_.

---

<h1>About the widget</h1>

- When navigating on the demo website, we are displaying a widget which fetches realtime data from Audience Manager. The widget displays the information stored in the various profiles used in the segmentation process. Its purpose is to make it easy to understand how data is stored in the backend and how it gets combined.
- Let's take a look at the various components of the widget:

![Widget](https://cloud.githubusercontent.com/assets/952836/24185637/70df6cc4-0e91-11e7-898b-3ee00ee73c0d.jpg)

---

<h1>Demo step 8</h1>

- Let’s switch devices.
- So far we have been accessing the website from a single device. Let’s see what happens when we visit it from a different device. For this purpose, you can either open up a new browser (Mozilla Firefox) or, if you will, you can access the demo website from your personal device such as your smartphone or laptop.
- When you access the website from a different device, you are again a first time user. As such, the common experience is being presented to you, with no personalization taking place just yet. 

![Common Experience](https://cloud.githubusercontent.com/assets/952836/24172744/94ccb0d8-0e46-11e7-9f28-9f57e7bd0ce0.png)


---

<h1>Demo Step 9</h1>

In the top bar, click the **SALES** tab.

When clicking on the sales tab, you will get qualified for the “Interested in the Season Sales” trait.

![Sales](https://cloud.githubusercontent.com/assets/952836/24172914/45506f4e-0e47-11e7-910b-8f1f5e5fd196.png)

---

<h1>Demo step 10</h1>

- Go on the PopularRetailer demo website home page. For this, click on the "PopularRetailer" on the top left.
g- You should now see an offer for items on sale for both men & women on the landing page.

![Sales](https://cloud.githubusercontent.com/assets/952836/24172946/6236a308-0e47-11e7-93de-dc5d44448dd5.png)

---

<h1>Demo step 11</h1>

On this new device, let’s authenticate with the same account as before.

Your iMac is assigned a number between 1 and 50. Find out your number and use it to login:

- **Username:** summit2017-99-**female** (replace 99 with your iMac number)
- **Password:** Adobe#2017

This is where the cross-device magic happens. With the power of this common login, we’re able to link this device with the previous one and merge these 3 profiles:
- The Authenticated Profile. Contains the **Gender is female** trait.
- The Device1 profile. Contains the **Athletic** trait.
- The Device2 profile. Contains the **Is interested in the season** sales trait.

**By merging these 3 together, we’re able to display an offer for "Season sales for women sportswear"**

---

<h1>Demo step 12</h1>

And Voila! We’re now performing personalization based on cross device activity. Notice how the ad takes into account the gender along with the interests in the season sales and athletic items. This enables us to discuss with our customer as a person, rather than target her as individual devices.

![picture18](https://cloud.githubusercontent.com/assets/952836/24139684/4c4ea828-0dda-11e7-915d-93e7ec1703f5.png)

---

<h1>Chapter 2 - Frequency capping</h1>

Let's see now a cool use case on how to optimize your ad spending, while at the same time offering relevant ads to your prospects, without the risk of getting them fatigued.

Objectives:
- Display ads based on prospect interests
- Perform recency frequency capping (stop showing the ad if the user is not interacting)

---

<h1>Demo step 13</h1>

Let's put ourselves in the shoes of the prospect. As a PopularRetailer potential customer, we see a pair of sunglasses which we find attractive and decide to check it out.

At this point, you should be authenticated. If you are not, let's authenticate on the PopularRetailer demo website. Click on the Login button at the top of the demo website.


Your iMac is assigned a number between 1 and 50. Find out your number and use it to login:

- **Username:** summit2017-99-female (replace 99 with your iMac number)
- **Password:** Adobe#2017

After you make sure to be authenticated, go on the home page and click on the **My Lady Sunglasses** item, on the bottom left.

![Click Sunglasses](https://cloud.githubusercontent.com/assets/952836/24173326/dd85dafa-0e48-11e7-84ef-af58182b5718.jpg)

---

<h1>Spotlight</h1>

- Once we click on the Sunglasses item, we will get qualified for the **Interested in "My Lady" Retro Sunglasses**.
- We'll now create a segment to display an ad for this item. The ad banner will be displayed on the "Women's" section. The segment has been pre-created, but feel free to look over its configuration here: [Sunglasses Ad Segment](https://bank-beta.demdex.com/portal/Segments/SegmentBuilder.ddx#view/5923420)

---

<h1>Demo step 14</h1>

- Let's now go to the Women's section, by clicking on the "Women's" tab on the top bar present on the demo website. We should now see an ad for the sunglasses we've just inspected.

![Sunglasses Ad](https://cloud.githubusercontent.com/assets/952836/24174052/e5f2bb88-0e4b-11e7-97cb-f58665240fce.jpg)

---

<h1>Demo step 15</h1>

- Here's the catch. We don't want to show this ad indefinitely. If our user goes 100 times to the "Women's" section, we don't want to show the ad 100 times. First of all, this will start upsetting our prospect. Secondly, if this were to be off-site targeting, we would waste a lot of money, displaying the same ad over and over again, without seeing an interaction from the user. For this reason, we can put a limit on the number of impressions for each ad, at a per user level. Note: we say per user, not per device. In our case, if the user has 5 devices, we want to show the ad 10 times across all their devices. If the user sees the ad 7 times on her tablet and 3 times on her laptop, that's it. We'll stop showing the ad.

- Feel free to refresh the page, while on the "Women's" section. You can do this across multiple devices/browsers. Make sure to be authenticated with the same account on the various browsers/devices.
- With each ad view, you should see the number of trait qualifications increase in the widget.
- After 5 page views, you will see that the ad will change a bit, displaying a 10% off discount. This is because we have created a secondary segment which targets all the users that have seen the ad at least 5 times: [Sunglasses Ad Segment #2 - 10% off](https://bank-beta.demdex.com/portal/Segments/SegmentBuilder.ddx#view/5923421)

- After 10 page views, the ad will stop being displayed completely. This is because we have not seen an interaction with the ad and as such we decide to stop showing it for now.

- After 3 days however, the ad will be shown again. This is because our segment rules have been designed to have a lookback period of 3 days, when it looks for ad views for each user.

---

![slide30](https://cloud.githubusercontent.com/assets/952836/24139709/6e878fea-0dda-11e7-9811-aab7812c9be9.jpg)

---

<h1>Why Adobe Audience Manager?</h1>

- By helping you build unique audience profiles, you can identify your most valuable segments and use them across any digital channel.
- Audience Manager combines the various silos, whether first, second or third party data, which were previously not talking with each other, and makes it easy for you to act upon.
- Regardless of your data source, destination or how you want to push the data out, Audience Manager will connect. You can send back information to your own systems for site customization or to ad networks for ad targeting. We know you work with different tools, so Audience Manager is designed to connect with anything. This neutral stance is critically important. You want interoperability and the option to leverage new tools or partners as designed. This decouples audience management from media.
- Audience Manager is integrated with the Adobe Marketing Cloud solutions, offering seamless import, segmentation and export.

---

<h1>Optional tasks</h1>

<h2>How are we qualifying for the "Athletes" trait?</h2>

When the browser loads the Athletes blog article, an HTTP call is being made to Adobe Audience Manager.
This HTTP call contains two important pieces of information:
- the Audience Manager user id
- the data signals

<h2>What is an Audience Manager ID?</h2>
The AAM ID is NOT a cross device id. Therefore, if the user has 3 devices, it will have (at least) 3 AAM IDs. The AAM ID is stored in a third party cookie. If you happen to have and use two browsers on your device, these will not share the cookie storage. As such, we will get two distinct Audience Manager IDs, one for each browser. 
<h2>What happens on mobile apps, where we don't have cookies?</h2>
The mobile apps using the AAM SDK, will store the Audience Manager ID in the app's internal storage. Multiple apps installed on the same device, will have different AAM ids.
<h2>How do we obtain an AAM id?</h2>
In our case we are dealing with a website. The website is integrated with the VisitorID.js library, maintained by the Adobe Audience Manager team. This javascript library takes care of generating an Audience Manager ID, when none is available. It does so by triggering a call from the browser to the Visitor ID service.

<h3>Optional task 1:</h3>
Emulate the Visitor ID call to Audience Manager, which the VisitorID.js library is making from the browser.

Open up the Terminal app on your iMac. Then copy paste this HTTP call command and press enter:
```
curl "http://dcs-beta.demdex.net/id?d_visid_ver=2.0.0&d_rtbd=json&d_ver=2&d_orgid=A71B5B5B54F607AB0A4C98A3%40AdobeOrg"
```

HTTP parameters sent:

| Name                  | Description   |
| --------------------- | ------------- |
| d_visid_ver=2.0.0     | The VisitorID.js library version |
| d_rtbd=json           | This parameter instructs AAM to return a json response |
| d_orgid=...           | Represents the IMS organization id, which uniquely identifies the Audience Manager client which is making the call (eg. PopularRetailer) |


Notice that the HTTP API contains `demdex.net`, which is the Audience Manager's domain.

The formatted Visitor ID json response will look like this:

```json
{  
   "d_mid":"88819962471507989271280036438453367558",
   "id_sync_ttl":604800,
   "d_blob":"cIBAx_aQzFEHcPoEv0GwcQ",
   "dcs_region":7,
   "d_ottl":7200,
   "ibs":[  
      {  
         "id":"411",
         "ttl":10080,
         "tag":"img",
         "fireURLSync":1,
         "syncOnPage":1,
         "url":[  
            "//cm.everesttech.net/cm/dd?d_uuid=89334862240161643561259517779946724685"
         ]
      }
   ],
   "subdomain":"aamsummit"
}
```

Notice the `d_mid` parameter, which represents the Marketing Cloud ID. The MID can be decoded by Audience Manager to obtain an AAM ID.

<h2>We have an AAM ID. How do we send the data?</h2>
In our situation, we want to notify Audience Manager that the current visitor has looked over the Athletes blog article. We do this by making a data collection HTTP call to Audience Manager.

<h3>Optional task 2: Send realtime data to Audience Manager</h3>

Open up the Terminal app on your iMac. Then copy paste this HTTP call command and press enter:
```
curl -v "https://dcs-beta.demdex.net/event?d_mid=88819962471507989271280036438453367558&d_orgid=A71B5B5B54F607AB0A4C98A3@AdobeOrg&d_rtbd=json&d_full=1&c_page=athletes-blog"
```

HTTP parameters sent:

| Name                  | Description   |
| --------------------- | ------------- |
| c_page=athletes-blog  | The signal sent to AAM. This notifies AAM that the visitor has looked over the athletes blog. We have already created [a trait](https://bank-beta.demdex.com/portal/Traits/Traits.ddx#view/5923404) which rule's states that `c_page == "athletes-blog"`. Because of this we will qualify this device for the Athletes gtrait. |
| d_rtbd=json           | This parameter instructs AAM to return a json response |
| d_orgid=...           | Represents the IMS organization id, which uniquely identifies the Audience Manager client which is making the call (eg. PopularRetailer) |
| d_mid=...             | Represents the Marketing Cloud ID. Audience Manager will decode this id and will obtain an AAM ID. The resulting trait will be stored keyed of this device id. |



The formatted json response will look like this:
```json
{
   "uuid":"89334862240161643561259517779946724685",
   "dcs_region":7,
   "data_collection":{  
      "traits":[  
         {  
            "id":{  
               "id":"89334862240161643561259517779946724685"
            },
            "new_traits":[  
               {  
                  "id":5923404
               },
               {  
                  "id":5923375
               }
            ]
         }
      ],
      "merge_rules":[  
         // contains all the segments qualified
      ]
   }
}
```

Notice the `new_traits` field. This contains two newly qualified gtraits:
- [Athletes trait (ID: 5923404)](https://bank-beta.demdex.com/portal/Traits/Traits.ddx#view/5923404)
- [Activity trait (ID: 5923375)](https://bank-beta.demdex.com/portal/Traits/Traits.ddx#view/5923375). This trait gets qualified automatically for any interaction. It is useful as it gives a metric on the total amount of visitors. 


---

<h1>Optional tasks</h1>

<h2>What's happening behind the scenes, when we authenticate?</h2>
In the previous HTTP calls made to Audience Manager, we noticed the marketing cloud identifier was being sent to Audience Manager (the `d_mid` parameter).
It turns out we can actually send multiple identifiers to AAM in a single HTTP call:
- device identifiers (Marketing Cloud IDs / AAM IDs)
- cross-device ids (eg. CRM id)
- mobile ids (eg. Apple's IDFA or Google's Advertising Id)

For PopularRetailer, whenever an user authenticates, we get access to the authenticated id (the customer id): **summit2017-99-female**. Since this same customer id can be used to authenticate from multiple devices, we call it a cross-device id.

<h2>How to send a customer id to Audience Manager?</h2>


<h2>Optional task 3</h2>

Open up the Terminal app on your iMac. Then copy paste this HTTP call command and press enter:

```
curl -v "https://dcs-beta.demdex.net/event?d_mid=88819962471507989271280036438453367558&d_orgid=A71B5B5B54F607AB0A4C98A3@AdobeOrg&d_rtbd=json&d_full=1&d_cid=126066%01summit-110-female"
```

HTTP parameters sent:

| Name                  | Description   |
| --------------------- | ------------- |
| d_rtbd=json           | This parameter instructs AAM to return a json response |
| d_orgid=...           | Represents the IMS organization id, which uniquely identifies the Audience Manager client which is making the call (eg. PopularRetailer) |
| d_mid=...             | Represents the Marketing Cloud ID. Audience Manager will decode this id and will obtain an AAM ID. |
| d_cid=126066%01summit-110-female | Represents the cross-device customer id. <a href="https://marketing.adobe.com/resources/help/en_US/aam/cid.html" target="_blank">Visit the documentation page here</a>. Authenticated activity is stored keyed of cross-device ids, unauthenticated activity is stored keyed of device ids. If the HTTP call contains a valid cross-device customer id, AAM treats the call as authenticated activity. As a result, since our call does have a cross-device id declared on the HTTP call, the traits will be stored keyed of this cross-device customer id. The traits will NOT be stored on the device id for this specific call, since the cross-device id takes precedence. |



The formatted json response will look like this:
```json
{
   "uuid":"89334862240161643561259517779946724685",
   "dcs_region":7,
   "data_collection":{  
      "traits":[  
         {  
            "id":{  
               "namespace":126066,
               "id":"summit-110-female"
            },
            "new_traits":[  
               {  
                  "id":5923407
               },
               {  
                  "id":5923375
               }
            ]
         },
         {  
            "id":{  
               "id":"89334862240161643561259517779946724685"
            },
            "existing_traits":[  
               {  
                  "id":5923404,
                  "frequencies":[  
                     {  
                        "day":3001,
                        "realizations":1
                     }
                  ]
               }
            ]
         }
      ],
      "merge_rules":[  
          ...
          "segments":[  
               {  
                  "id":5923408,
                  "status":"REACQUIRED"
               }
         ]
      ]
   }
}
```

