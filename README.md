# Study Planner Final Course Project

Ashlie M Wyse — SDEV 264 Mobile Application Development

Study Planner helps students organize assignment titles, courses, due dates, priorities, notes, and completion status. This final project contains four Android activities with fragments, SQLite records, explicit Intent data, and persistent Preferences DataStore settings.

## Download and run

1. Download [StudyPlanner-Final-Wyse-A.zip](StudyPlanner-Final-Wyse-A.zip).
2. Extract the ZIP, then open its `StudyPlanner` folder in Android Studio.
3. Install Android SDK Platform 35 and select an installed JDK 21 as the Gradle JDK. Any JDK 21 vendor is supported. The project uses Gradle 8.12 and Android Gradle Plugin 8.8.0.
4. Let Gradle sync, choose the `app` configuration and an emulator running Android 8.0/API 26 or higher, then click Run.

The ZIP includes the complete portable source and Gradle wrapper. Android Studio creates `local.properties` for the local Android SDK. No API key, internet service, or account is required to use the app. Gradle may need internet access when downloading build dependencies for the first time.

## Required activities

- **Main:** shows saved assignments and the unfinished count; opens Add Assignment, Preferences, Help, or a selected assignment.
- **Assignment Details:** Main passes an assignment ID through an explicit Intent; the detail screen loads that record and supports validated editing, Save, Cancel, and date selection.
- **Preferences:** default sort is earliest due date, completed records are hidden, and new assignments have Medium priority. Save retains both changed and unchanged values. Settings affect list ordering/filtering and default priority; existing record priorities stay unchanged.
- **Help:** display-only instructions explain the purpose, all preferences, saving, and Back behavior.

Version 1.0, version code 5. Production application ID is `com.ashliewyse.studyplanner`; debug builds use `com.ashliewyse.studyplanner.final` to isolate test data.

## Verification

Fresh final verification on October 16, 2026 (America/Chicago): successful debug and test APK builds, 5/5 unit tests, 8/8 emulator tests, and 0 lint errors. The final screenshot acceptance workflow also passed separately. Seven lint advisories concern dependency updates, backup configuration, and overdraw; none prevented the build or tests.

A force-stop followed by a cold launch retained the test records and preference values. The screenshots are original emulator captures from this final build and show illustrative test records, not a report of actual coursework completion. See [Verification.txt](Verification.txt).

## Screenshots

Each screenshot is supplied individually in this repository and separately from the Android project ZIP.

- [01-Main-Activity](01-Main-Activity.png)
- [02-Preferences-Defaults](02-Preferences-Defaults.png)
- [03-Preferences-Reopened-Saved-Choices](03-Preferences-Reopened-Saved-Choices.png)
- [04-Assignment-Input-And-Default-Priority](04-Assignment-Input-And-Default-Priority.png)
- [05-Main-Saved-Assignment-Output](05-Main-Saved-Assignment-Output.png)
- [06-Secondary-Activity-Selected-Record-From-Intent](06-Secondary-Activity-Selected-Record-From-Intent.png)
- [07-Main-Due-Date-Order-And-Completed-Shown](07-Main-Due-Date-Order-And-Completed-Shown.png)
- [08-Preferences-Changed-Sort-And-Filter-Input](08-Preferences-Changed-Sort-And-Filter-Input.png)
- [09-Main-Preference-Effects-Output](09-Main-Preference-Effects-Output.png)
- [10-Main-Relaunched-With-Saved-Data](10-Main-Relaunched-With-Saved-Data.png)
- [11-Preferences-Retained-After-Relaunch](11-Preferences-Retained-After-Relaunch.png)
- [12-Help-Opened-From-Main](12-Help-Opened-From-Main.png)
- [13-Help-Explains-Preferences](13-Help-Explains-Preferences.png)
- [14-Returned-To-Main](14-Returned-To-Main.png)
- [15-Main-After-Full-Process-Restart](15-Main-After-Full-Process-Restart.png)
