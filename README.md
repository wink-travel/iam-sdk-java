[![wink.travel logo](https://res.cloudinary.com/traveliko/image/upload/c_scale,h_75/v1653285543/wink/logo_text.png)](https://wink.travel)

# Wink IAM Java SDK

Welcome to the Java SDK that enables you to communicate with all that the Wink platform has to offer.

## Getting started
This SDK contains libraries you can leverage to communicate with the Wink platform.

### Java Requirements
Maven artifacts were compiled with Java 17. Java 1.8 is the lowest supported version.

Spring is not required but we highly recommend you use. Our examples will be based on how to do it the "Spring way".

Download libraries from Maven Central Repository.

### OAuth2 Support

Spring-enabled OAuth2 bean that manages your keys.

```
<dependency>
<groupId>travel.wink</groupId>
<artifactId>iam-sdk-java</artifactId>
<packaging>jar</packaging>
<version><!-- see Releases --></version>
</dependency>
```

#### Usage

Using Spring, @Import(OAuth2WebClientConfiguration.class) or run a component scan over `travel.wink.sdk.support` and you let the library manage OAuth2 state for you.


## Configuration
You will need a client ID and a client secret to communicate with any of the Wink platform endpoints. You can create your account and get your credentials here:

[https://sell.wink.travel](https://sell.wink.travel)

Steps: 
1. Register your personal user account
2. Log in
3. Create your first account
4. Select that account
5. Choose to create an Application for that account 
6. The application will hold your credentials

### Spring users
Add your credentials to your property file:

1. wink.travel.client.id=YOUR_CLIENT_ID
2. wink.travel.client.secret=YOUR_CLIENT_SECRET

### Non-Spring users
Create 2 environment variables in your preferred way:

1. WINK_TRAVEL_CLIENT_ID=YOUR_CLIENT_ID
2. WINK_TRAVEL_CLIENT_SECRET=YOUR_CLIENT_SECRET

## You might also be interested in...
If you are developing for WordPress, we've [probably] got you covered. Check out our WordPress plugin:

- Wink Java SDK repo: [https://github.com/wink-travel/wink-sdk-java](https://github.com/wink-travel/wink-sdk-java)
- TripPay Java SDK repo: [https://github.com/wink-travel/trip-pay-sdk-java](https://github.com/wink-travel/trip-pay-sdk-java)
- Wink WordPress plugin repo: [https://github.com/wink-travel/affiliate-wordpress-plugin](https://github.com/wink-travel/affiliate-wordpress-plugin)
- Wink WordPress Divi plugin repo: [https://github.com/wink-travel/affiliate-wordpress-divi-plugin](https://github.com/wink-travel/affiliate-wordpress-divi-plugin)
- WordPress: [https://wordpress.org/plugins/iko-travel-affiliate/](https://wordpress.org/plugins/iko-travel-affiliate/) 
