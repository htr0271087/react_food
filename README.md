
#### Yelp API Helper
In the upcoming lecture, we will be signing up for a Yelp developer account. Depending on your location, some students may be blocked from creating an account. There are a few things you can try.

Students noted a workaround in this thread using their phone which will show a captcha:

https://www.udemy.com/course/the-complete-react-native-and-redux-course/learn/lecture/15707036#questions/8334522

Using a VPN for registration and making API calls should also work. Students mentioned they were able to successfully sign up for an API key using the Opera Browser's built-in VPN feature. Other students mentioned that they were able to use Tunnelbear's free tier.

Lastly, you can try just using my key:

MMMQuWnLGwlTYdSMtKujs774rvSF8-g78jwHgo35nIoahZ1df13ph_HxFOTGIpGD-_CVpb--RMaPA2clqd8koS8x58EPk6H9fkhW791Uws_LRizh44UyVyGh4feNX3Yx

If some students try to use this in production or abuse the key in some way, you may start getting 429 errors (too many requests)

#### React Navigation

updated 9-2-2020

Important Message about React Navigation v5
This project will be using the v4 version of React Navigation and not the v5 version which was released a few months ago. To date, this code still works as expected. The v4 version is still important to know and understand as it is used widely in existing codebases in many organizations. Stephen is aware of the interest in an update and will hopefully post a supplement at some time in the future. In the meantime, I highly encourage you to continue on with the course as it is so that you fully understand how React Navigation works. Once you have finished the course, you can use this is a self-study opportunity to attempt a migration of your finished working projects to v5. The docs provide some great resources on this: https://reactnavigation.org/docs/upgrading-from-4.x/.

1. React Navigation v4 Installation
note: You cannot mix Yarn and npm in the same project as it will break your dependencies. You must consistently use the same package manager. If you have yarn installed on your computer it will be used by default to generate the project. In this case, you must use Yarn to install your dependencies.

1. Install React Navigation

npm install react-navigation

or

yarn add react-navigation

2. Install Dependencies

expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view

3. Install React Navigation Stack

npm install react-navigation-stack @react-native-community/masked-view

or

yarn add react-navigation-stack @react-native-community/masked-view

4. Start the app and clear cache with expo r -c

2. Update Imports
Our imports in the upcoming lecture will now look like this:

import { createAppContainer } from 'react-navigation';
import { createStackNavigator } from 'react-navigation-stack';

Errors?
If you are still struggling with the React Navigation installation then there are likely some major dependency conflicts in your environment. In this case, we've made a boilerplate available so that you can continue with the course. Download the zip file attached to this lecture to somewhere in your C:\Users directory (Windows) or /Users directory (macOS)

Then, run npm install and then npm start.

React Navigation v4 Docs:
https://reactnavigation.org/docs/4.x/getting-started