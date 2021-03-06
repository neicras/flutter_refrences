
### Content
* ui_login [Login Page UI in Flutter, by Yogita Kumar, gitconnected, medium](https://levelup.gitconnected.com/login-page-ui-in-flutter-65210e7a6c90)
* navigation_push_pop & navigation_routes [Flutter - Navigation using push(), pop() and routes,by Yogita Kumar, medium](https://medium.com/faun/flutter-navigation-using-push-pop-and-routes-d49988098efe)
* package_sharedPreferences [SharedPreferences 設定檔資料存取](http://tw-hkt.blogspot.com/2019/08/flutter-sharedpreferences.html)
* package_provider [Flutter Provider的使用](https://segmentfault.com/a/1190000038446714)
* authtication_shuaib [Flutter Thursday 13: Building a User Registration and Login Process with provider and external API](https://medium.com/@afegbua/flutter-thursday-13-building-a-user-registration-and-login-process-with-provider-and-external-api-1bb87811fd1d)
* ui_basicWidgets [Flutter Layout Basics (4:01)](https://www.youtube.com/watch?v=uisLoOmtISk) [Flutter Layout Design Tutorial || Top 5 Widgets (21:04)](https://www.youtube.com/watch?v=-z26yE9g0Hg)
* package_imagePicker [Official Docs - Image Picker plugin for Flutter](https://pub.dev/packages/image_picker)
* tutorial_theme_switcher using provider with shared preferences [Building theme switcher using Provider and Shared Preferences](https://codesource.io/building-theme-switcher-using-provider-and-shared-preferences/)

### Flutter Installation
1. copy stable flutter version from git
- MacBook-Pro-2:Flutter-QuickStart EricSan$ git clone https://github.com/flutter/flutter.git -b stable --depth 1

2. update path and run flutter
- export PATH="$PATH:`pwd`/flutter/bin"
- flutter
- flutter doctor

> ✗ Flutter plugin not installed; this adds Flutter specific functionality.
> ✗ Dart plugin not installed; this adds Dart specific functionality.
- just run in the terminal this command
`ln -s ~/Library/Application\ Support/Google/AndroidStudio4.1/plugins ~/Library/Application\ Support/AndroidStudio4.1` ([StackOverflow](https://stackoverflow.com/questions/51860845/flutter-plugin-not-installed-error-when-running-flutter-doctor))

> [!] Connected device: is not available.
* Android Studio > AVD Manager > Run

### Create an app
- flutter create myapp

### Boot up the app
1. export PATH="$PATH:`pwd`/flutter/bin"
2. cd decg_main
3. andriod studio
    Android Studio > Any Project > Wait for "loading devices"
    Device > AVD Manager > Run
4. flutter devices 
    MacBook-Pro-2:decg_main EricSan$ flutter devices
    3 connected devices:

    sdk gphone x86 (mobile) • emulator-5554 • android-x86    • Android 11 (API 30) (emulator)
    Web Server (web)        • web-server    • web-javascript • Flutter Tools
    Chrome (web)            • chrome        • web-javascript • Google Chrome 87.0.4280.88
5. flutter run
    Using hardware rendering with device sdk gphone x86. If you notice graphics artifacts, consider enabling software rendering with
    "--enable-software-rendering".
    Launching lib/main.dart on sdk gphone x86 in debug mode...
    Running Gradle task 'assembleDebug'...                                 ⣻

### Turn on Android Emulators in Android Studio 
(
    <problem with running android studio>
    questions/63517294/the-ide-cannot-create-the-directory-possible-reason-parent-directory-is-read-o/64802591#64802591
    give permission for the cache file
)

Android Studio > Any Project > Wait for "loading devices"
Device > AVD Manager > Run

flutter emulators (list and start any available device emulators)
flutter emulators --create Pixel_2_API_30

flutter devices
flutter run -d <device name>

Flutter run key commands.
r Hot reload. 🔥🔥🔥
R Hot restart.
h Repeat this help message.
d Detach (terminate "flutter run" but leave application running).
c Clear the screen
q Quit (terminate the application on the device).
An Observatory debugger and profiler on sdk gphone x

### VS Code
- install flutter and reload

### Run Chrome Webapp
- https://flutter.dev/docs/get-started/codelab-web

flutter emulators --launch  Pixel_2_API_30
flutter devices
flutter run -d "sdk gphone x86"
flutter run -d chrome


### Flutter release web project
https://itnext.io/setup-a-flutter-web-project-on-github-pages-58b3118b0a28

flutter build web --release
cd build/web
git commit -m "xxx"
git push

git push -f origin

### Further References
Flutter---Google推出的跨平台框架，Android、iOS一起搞定 系列
https://ithelp.ithome.com.tw/users/20119550/ironman/2221