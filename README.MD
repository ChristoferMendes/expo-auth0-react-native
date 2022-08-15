![React-Native-Badge](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
# Expo-Auth0 Integration template
> Please, check the main repository that I retrieve **all** this information from: [https://github.com/expo/examples/tree/master/with-auth0][MainRepo]




<hr />

## Installation

### If you haven't installed **Expo**, please, type the following command on your **_root directory_**: 
```
npm install --global expo-cli
```

Clone the repo:

```wsl
git clone git@github.com:ChristoferMendes/react-native-expo-auth0.git
```
Install dependencies

```
yarn
```

> ## Runnig the Project
> - Create your own app on [**Auth0**][Auth0].
> - Add the `AuthSession` auth URL to `Allowed Callback URLs` on [**Auth0**][Auth0].
> - Open **App.tsx** → replace `auth0ClientId` and `authorizationEndpoint` with your respectives **Auth0 App Settings**
> - _Follow the_ <a href='#auth0-integration'>Auth0 Integration section</a> _for a better step by step on how to get these settings_

## ***Extra***
<details>
    <summary><b>Running an Expo project</b></summary>
    <ul> 
        <li> <code>expo start --tunnel</code></li>
        <li>Install the <b>Expo Go</b> app in your smartphone and scan the <em>QR Code</em> that shows up</li>
    </ul>
</details>

<hr />

<center>
 
## **Auth0 Integration**
### Create an account on [**Auth0**][Auth0] or Log in

## Click on Applications tab (on the left of the site)

![Auth0-Dashboard][Auth0-Dashboard]

</center>


> Hit `Aplications` → `Create application` → Select **Native**, give it a name and create the Application


## **Retrieving important info for App.tsx**
### After create the Application, just grab Domain and your Client ID!
- BE AWARE! The domain here is necessary to have _https:://_**dev-uotzwyb3.us.auth0.com**_/authorize_
  - ie, grab your **Domain** and add `https:://` in the beginning and `/authorize` in the end

<center>

![Domain-and-ClientId-Screenshot][Domain-and-ClientId-Screenshot]

> You can see this information better in **Advanced Settings**, on the same page:
>
> ![Auth0-Advanced-Settings][Auth0-Advanced-Settings]

</center>

[MainRepo]:https://github.com/expo/examples/tree/master/with-auth0
[Auth0]:https://auth0.com/
[Domain-and-ClientId-Screenshot]:https://i.ibb.co/qFLJ1X9/Screenshot-140.png
[Auth0-Advanced-Settings]:https://i.ibb.co/7tCH05k/Screenshot-141.png
[Auth0-Dashboard]:https://i.ibb.co/3RKY3qj/Screenshot-138.png
