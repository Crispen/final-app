<!--
Care-Less
-->
# final-app-name
![Swift](https://img.shields.io/badge/swift-5.5-brightgreen.svg) ![Xcode 13.2+](https://img.shields.io/badge/xcode-13.2%2B-blue.svg) ![iOS 15.0+](https://img.shields.io/badge/iOS-15.0%2B-blue.svg) ![watchOS 8.0+](https://img.shields.io/badge/watchOS-8.0%2B-blue.svg) ![CareKit 2.1+](https://img.shields.io/badge/CareKit-2.1%2B-red.svg) ![ci](https://github.com/netreconlab/CareKitSample-ParseCareKit/workflows/ci/badge.svg?branch=main)

## Description
<!--
The goal of Care-Less is to enable users to collect their heath data, combined with daily check-ins to create a long-term insights into their health. Changes in blood pressure, weight, or even sleeping habits can be collated into a single place, and thus equipping users to have a more unified understanding of their overall health. Furthermore, using daily check-ins builds retenetion, and allows the ability to capture some health events that might not typically be recorded, such as a mild ankle sprain. With Care-Less users areable to track a snapshot of their health over time![image](https://user-images.githubusercontent.com/1577486/167020123-8460e7e0-bc3c-440d-a0a9-e4deaba73d55.png)

-->
An example application of [CareKit](https://github.com/carekit-apple/CareKit)'s OCKSample synchronizing CareKit data to the Cloud via [ParseCareKit](https://github.com/netreconlab/ParseCareKit).

### Demo Video
<!--
Add the public link to your YouTube or video posted elsewhere.
-->
To learn more about this application, watch the video below:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=mib_YioKAQQ
" target="_blank"><img src="http://img.youtube.com/vi/mib_YioKAQQ/0.jpg" 
alt="Sample demo video" width="240" height="180" border="10" /></a>

### Designed for the following users
<!--
Care-Less is for everyone. The goal is to empower the user to better understand their overall health over time, and monitor any changes. Building solid data and organizing it in a single place equips users of any age to better understand changes to their health, and knowingly track the improvements they have made.
-->

<!--
In addition, you can drop screenshots directly into your README file to add them to your README. Take these from your presentations.
-->
<img src="https://user-images.githubusercontent.com/8621344/101721031-06869500-3a75-11eb-9631-88927e9c8f00.png" width="300"> <img src="https://user-images.githubusercontent.com/8621344/101721111-33d34300-3a75-11eb-885e-4a6fc96dbd35.png" width="300"> <img src="https://user-images.githubusercontent.com/8621344/101721146-48afd680-3a75-11eb-955a-7848146a9d6f.png" width="300"><img src="https://user-images.githubusercontent.com/8621344/101721182-5cf3d380-3a75-11eb-99c9-bde40477acf3.png" width="300">

<!--
List all of the members who developed the project and
link to each members respective GitHub profile
-->
Developed by: 
- [member1](https://github.com/Crispen) - University of Kentucky`, `Computer Science`

ParseCareKit synchronizes the following entities to Parse tables/classes using [Parse-Swift](https://github.com/parse-community/Parse-Swift):

- [x] OCKTask <-> Task
- [x] OCKHealthKitTask <-> HealthKitTask 
- [x] OCKOutcome <-> Outcome
- [x] OCKRevisionRecord.KnowledgeVector <-> Clock
- [x] OCKPatient <-> Patient
- [x] OCKCarePlan <-> CarePlan
- [x] OCKContact <-> Contact

**Use at your own risk. There is no promise that this is HIPAA compliant and we are not responsible for any mishandling of your data**

<!--
What features were added by you, this should be descriptions of features added from the [Code](https://uk.instructure.com/courses/2030626/assignments/11151475) and [Demo](https://uk.instructure.com/courses/2030626/assignments/11151413) parts of the final. Feel free to add any figures that may help describe a feature. Note that there should be information here about how the OCKTask/OCKHealthTask's and OCKCarePlan's you added pertain to your app.
-->
## Contributions/Features

## Final Checklist
<!--
This is from the checkist from the final [Code](https://uk.instructure.com/courses/2030626/assignments/11151475). You should mark completed items with an x and leave non-completed items empty
-->
- [x] Signup/Login screen tailored to app
- [x] Signup/Login with email address
- [x] Custom app logo
- [x] Custom styling
- [x] Add at least **5 new OCKTask/OCKHealthKitTasks** to your app
  - [x] Have a minimum of 7 OCKTask/OCKHealthKitTasks in your app
  - [x] 3/7 of OCKTasks should have different OCKSchedules than what's in the original app
- [x] Use at least 5/7 card below in your app
  - [x] InstructionsTaskView - typically used with a OCKTask
  - [ ] SimpleTaskView - typically used with a OCKTask
  - [x] Checklist - typically used with a OCKTask
  - [x] Button Log - typically used with a OCKTask
  - [x] GridTaskView - typically used with a OCKTask
  - [ ] NumericProgressTaskView (SwiftUI) - typically used with a OCKHealthKitTask
  - [x] LabeledValueTaskView (SwiftUI) - typically used with a OCKHealthKitTask
- [x] Add the LinkView (SwiftUI) card to your app
- [x] Replace the current TipView with a class with CustomFeaturedContentView that subclasses OCKFeaturedContentView. This card should have an initializer which takes any link
- [x] Tailor the ResearchKit Onboarding to reflect your application
- [x] Add tailored check-in ResearchKit survey to your app
- [x] Add a new tab called "Insights" to MainTabView
- [x] Replace current ContactView with Searchable contact view
- [x] Change the ProfileView to use a Form view
- [x] Add at least two OCKCarePlan's and tie them to their respective OCKTask's and OCContact's 

## Wishlist features
<!--
Describe at least 3 features you want to add in the future before releasing your app in the app-store
-->
1. Expanding the HealthKit functionality to allow additional biometrics to be tracked.
2. Allow for longer time windows for Insights - to better provide users' information on changes over time.
3. The ability to log Minor/Major health events to codify dates that might signify impacts onto biometrics

## Challenges faced while developing
<!--
Describe any challenges you faced with learning Swift, your baseline app, or adding features. You can describe how you overcame them.
-->
Customizing ResearchKit and syncing with HealthKit was often a difficult task. Trying to identify the specifics of a single property often led to a an investigation of a series of extensions or inheritance to finally arrive at perhaps the correct information. 

## Setup Your Parse Server

### Heroku
The easiest way to setup your server is using the [one-button-click](https://github.com/netreconlab/parse-hipaa#heroku) deplyment method for [parse-hipaa](https://github.com/netreconlab/parse-hipaa).


## View your data in Parse Dashboard

### Heroku
The easiest way to setup your dashboard is using the [one-button-click](https://github.com/netreconlab/parse-hipaa-dashboard#heroku) deplyment method for [parse-hipaa-dashboard](https://github.com/netreconlab/parse-hipaa-dashboard).
