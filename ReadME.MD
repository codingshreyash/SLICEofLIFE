<p align="center">
    <img src="assets/README/Banner.jpg" width="400">
</p>
# Slice of Life

## Home Page

This website is our submission for the Future Business Leaders of America state and national leadership conferences. Per the 2022-2023 prompt, this website serves as a business tool for the community to ____ at Slice of Life to 
* Access Slice of Life's appetizer, ontray, and dessert menu
* Order or book a table 
* Find more information regarding the history of Slice of Life
* Read our customer's most recent reviews on quality of food, atmposphere, and service
* Contact and location information

### About

- Android 7.0 lollipop or higher
    - Unrestricted internet connection
- In order for the app to fully function on an android studio emulator, the following requirements:
    - The latest version of android studio is installed
    - API 22 is the android emulator's target API

## Book a Table

- Download the app-release.apk file to your computer
- Enable usb storage on the target android device (API 22+)
- Connect the target android device to the computer, wait for installation
- Copy the .apk from the computer to the target android device
- Turn off usb storage on the target android device and disable usb storage
- Disconnect the target android device from the computer
- Enable application installation from "unknown sources" in the target android device's settings
- Navigate to the .apk in the target android device's file manager
- Click on the .apk, choose to install it
- Back out of the file manager, the app should now be installed on the target android device

* In the event the .apk fails to run on an android device:
    - Clone the repository
    - Create a new android virtual device using API 22 and starting 
    - cd into `kolbacademy\Client\clientReactNative`
    - run `npm install`
    - run `react-native run-android`
    - The application should build and open on the android emulator


### Menu
<p align="center">
    <img src="./Screenshots/login_demo.gif" width="300">
</p>
The application's authentication system is integrated with Google Firebase. As such when a user logs in with his or her credentials, they are sent to Firebase and verified against an encrypted keystore. If the credentials are valid, Firebase returns a unique client ID corresponding to the user. The application then uses this client ID to query the DynamoDB users table through the API to obtain identification information about the user (name, email, title, profile picture etc). This information is passed throughout the application, thereby allowing each user to have an customized experience unique to him or her.

#### Reviews
<p align="center">
    <img src="./Screenshots/homescreen_demo.png" width="300">
</p>
On the home screen, users can view identification information like their title and email address. They also have the ability to report bugs to the developer for continuous improvement.

#### Contact Us
<p align="center">
    <img src="./Screenshots/schedule_demo.gif" width="300">
</p>

When users click on the schedule tab, they have the ability to view their list of classes filtered by each day of the school week. This view succinctly presents key information about each class, and lets users quickly view a their classes' name, time, location, teacher, and period.

Users can also click the floating action button in the bottom-right corner to open a modal containing a detailed, editable view of his or her courses. Here, they can efficiently slide through their class list, and edit specific attributes.

Changes to course details are updating in real-time and users can view their updated schedule immediately.


#### Email Screen
<p align="center">
    <img src="./Screenshots/email_demo.gif" width="300">
    <p align = "center">
        Image 1: viewing messages, filtering inbox, responding to email as a student
    </p>
</p>

<p align="center">
    <img src="./Screenshots/email_demo_2.gif" width="300">
    <p align = "center">
        Image 2: viewing email response from image 1 as a teacher
    </p>
</p>

<p align="center">
    <img src="./Screenshots/email_demo_3.gif" width="300">
    <p align = "center">
        Image 3: drafting and sending a new email
    </p>
</p>

On the email tab, users can email their teachers and fellow students. When the tab is clicked, users arrive at their inbox and can see their email threads in sequential order. Users can filter their inbox by sender, subject, and message content.

When an email is clicked, a modal appears showing a detailed view of the selected email. Here, users can view the entire message thread and respond to the most recent email. When a response is sent, it appears in the recipient's inbox in real-time.

Users can also draft new emails and begin message threads by clicking the plus button in the bottom right corner.

 

## Built with

#### Frontend
I programmed the user interface of this application in a [React Native](https://reactnative.dev/), a free, open-source JavaScript framework developed by Facebook based on the popular web development framework React. When deciding how to best develop this mobile application, I decided to deviate from the more conventional Android Studio and Xcode development environments for 2 main reasons: **cross platform compatibility** and exposure to the **open-source community**.

**Cross Platorm**
Because of React Native's *learn once, write anywhere* philosophy, my application's source code was written (and can be further extended upon) only once, but is able to <ins>run on both ios and Android operating systems</ins>.

**Open Source**
Since React Native is itself and open-source framework, it can be built upon and further improved by members of the general software engineering community. As such, the tools and libraries available to me are far greater than those inherently provided by Android and ios.

### Backend
I developed the backend of my application using Amazon Web Services' [Serverless Application Model](https://aws.amazon.com/serverless/sam/). Given that much of the business world is shifting to the cloud, I was eager to get exposure to AWS and learn more about the different services it offers. My backend is currently comprised of API Gateway, Lambda, DynamoDB, and S3. I decided to build my backend in a serverless manner because of its **scalable nature**, and **cost-effective pricing** (which is great for a broke student like me).   

<p align="center">
    <img src="https://dashbird.io/wp-content/uploads/2020/10/api-gateway-proxy-database-architecture-diagram-1.gif" width="500">
    <p align = "center">
        Backend Application Architecture
    </p>
</p>

### Future Development
In my future devolpment I would like to add more features to app such as viewing grades, a module for teacher access, diffrent view modes for parents so they can help their child stay on top of their assigments and more. In the next stage of the app I also want to add an area for students to get hall passes, bathroom passes, and get push notfications about assigments. This app will become a "one-stop shop" for all student, teacher and parent needs relating to school. 

## Authors

* **Shreyash Ranjan** 
[Github](https://github.com/codingshreyash)
[LinkedIn](https://www.linkedin.com/in/shreyash-ranjan/)
* **Jack Gurczynski** 
[Github](https://github.com/codingjackg)
[LinkedIn](www.linkedin.com/in/jack-gurczynski)
* **Ohm Patel** 
[Github](https://github.com/ohm7p)
[LinkedIn](https://www.linkedin.com/in/ohm-patel-011bb6258/)

## Acknowledgments

I would like to sincerely thank a few people, without whom this project would not have been possible:
* Mr. Ryan Kolb | AP Computer Science Teacher
* Ms. Linda Westerlund | FBLA Advisor
