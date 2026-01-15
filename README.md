Calmio
Calmio is a modern Android app designed to help users improve pelvic floor strength (Kegel exercises) and practice meditation/breathing exercises while providing daily health facts. The app is offline-first, user-friendly, and focuses on habit-building and wellness.

📱 Features
Personalized Greeting: Based on phone time (Good Morning / Afternoon / Evening / Night)
User Setup: Users can enter their name and select exercises they want to do (Kegel, Meditation, or both)
Kegel Exercises: Multiple levels with timers, stop/resume functionality, and level progression based on completion
Meditation/Breathing Exercises: Users can choose a duration with safety check for long sessions
Daily Health Fact: 30 rotating health tips, updated every 24 hours with light animations
About/References: Shows sources for scientific information, with optional internet redirect for journals
Offline-First: No server or cloud database required; all data stored locally using SharedPreferences/DataStore
Stop & Resume: Stop means the session must be completed later; Resume means users can start over anytime
🗂 Folder Structure
app/src/main/
├─ java/com/example/calmio/
│ ├─ MainActivity.java // Home screen
│ ├─ SetupActivity.java // Name & exercise selection
│ ├─ ExerciseActivity.java // Kegel / Meditation screens
│ ├─ AboutActivity.java // About / scientific references
│ ├─ data/ // Local storage & model classes
│ │ ├─ UserProfile.java
│ │ ├─ ExerciseProgress.java
│ │ └─ HealthFactManager.java
│ ├─ utils/ // Helper classes
│ │ ├─ TimeUtils.java
│ │ ├─ AnimationHelper.java
│ │ └─ Constants.java
│ └─ ui/ // UI components (Kotlin)
│ ├─ kegel/
│ │ ├─ KegelSessionView.kt
│ │ └─ KegelLevelManager.kt
│ ├─ meditation/
│ │ ├─ MeditationTimerView.kt
│ │ └─ MeditationConfig.kt
│ └─ widgets/
│ ├─ GreetingCard.kt
│ └─ DailyFactCard.kt
└─ res/
├─ layout/ // XML layouts for screens
├─ values/ // Colors, strings, themes
├─ drawable/ // Images & icons
└─ mipmap/ // Launcher icons
⚙️ Technologies Used
App Language: Java (backend, activities, models, utils)
UI: Jetpack Compose (Kotlin) for modern UI components
Local Storage: SharedPreferences / DataStore
Build System: Gradle (Kotlin DSL)
Min SDK: 24+
📝 Development Phases
Phase 0: Project setup, folder structure, baseline README
Phase 1: Splash animation, Name Setup, Home Screen with greeting and daily health fact
Phase 2: Kegel exercise module with levels, timers, stop/resume
Phase 3: Meditation module, timers, and user-selected durations
Phase 4: About section, scientific references, optional internet redirect
Phase 5: Future improvements: notifications, stats, cloud backup
💡 Notes & Guidelines
Daily facts rotate every 24 hours with a small loading animation
Level progression: Users are promoted after completing exercises 14 times
Stop & Resume: Designed to let users pause or restart sessions without losing progress
User choice: Kegel and Meditation exercises are independent; users can select one or both
Offline-first: Users never need a network except for accessing journal references
🎨 App Name & Branding
App Name: Calmio
Theme: Modern, calm colors, simple animations, user-friendly layout
UI Design: Figma → design reference → implemented in XML/Compose
🔮 Future Enhancements
Statistics tracking & charts for exercise progress
Push notifications for daily exercises
Multi-user support or cloud backup
Extra exercises or meditation programs
📚 References (for scientific content)
Kegel exercises: peer-reviewed studies on pelvic floor strength and level progression
Meditation: peer-reviewed studies on breathing exercises, session duration, and mental wellness
Note: Daily health tips are general health guidance and do not require references.
