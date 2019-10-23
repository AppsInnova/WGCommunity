# WGCommunity
The WeGamers embedded community has provided mobile players with a powerful and easy-to-access community. Players do not require another platform or need to stay in-game to continue chatting with other players; they can do so via WeGamers. For the operation work, WeGamers can also be used to gather feedback or post news about events, etc. easily. All of this can be done with a few hours of work with this SDK. Your game(s) will offer a better service and all of this is free.

# How to use

Simply add the repository to your build.gradle file:

repositories {
    maven {
        url "https://raw.githubusercontent.com/AppsInnova/WGCommunity/master/"
    }
}

dependencies {
    implementation fileTree(include: ['*.jar'], dir: 'libs')
    api 'com.appsinnova.wegamers:community:1.0'

    //other public libraries
    implementation 'com.android.support:appcompat-v7:28.0.0'
    implementation ('com.squareup.retrofit2:converter-gson:2.2.0'){
        exclude group: 'com.squareup.okhttp3'
    }
    implementation 'com.squareup.retrofit2:adapter-rxjava:2.2.0'
    implementation 'com.squareup.okhttp3:logging-interceptor:3.6.0'
    implementation 'io.reactivex:rxandroid:1.2.0'
    implementation 'com.google.dagger:dagger:2.2'
    implementation 'org.greenrobot:eventbus:3.0.0'
}