# MAX – Offline Android Project (Starter)

ही **पहिली सुरक्षित पायाभूत आवृत्ती** आहे; मूळ Panda अॅपची पूर्ण duplicate आवृत्ती किंवा installable APK नाही.

## या आवृत्तीत काय आहे
- Android Studio साठी स्वतंत्र Kotlin प्रोजेक्ट.
- अॅपचे नाव `MAX`.
- Manifest मध्ये `INTERNET` permission नाही.
- Android backup बंद (`allowBackup=false`).
- Network cleartext बंद.
- Android Keystore आधारित AES-256-GCM local encryption helper.
- कोणतेही subscription, ads किंवा billing SDK नाहीत.

## काय अजून तयार नाही
- मूळ अॅपमधील सर्व AI/Agent फीचर्स.
- Offline AI model आणि inference runtime.
- Wake-word व offline speech-to-text / text-to-speech.
- Accessibility automation service.
- Browser automation.
- Backup/restore UI व recovery tests.
- मूळ अॅपशी feature-by-feature parity.

मूळ APK मधील online/cloud AI, Firebase, web search आणि integrations इंटरनेटशिवाय चालणार नाहीत. त्यांना स्वतंत्र offline पर्याय किंवा स्पष्टपणे वगळणे आवश्यक आहे. मूळ अॅपचे private server/API किंवा subscription checks bypass केलेले नाहीत.

## Build करण्याची पद्धत
1. Android Studio उघडा.
2. `Open` निवडा आणि हा `MAX_Android_Project` फोल्डर निवडा.
3. Gradle sync पूर्ण होऊ द्या (पहिल्या build साठी Android Gradle Plugin/Kotlin plugin डाउनलोड करावे लागू शकतात).
4. `Build > Build APK(s)` निवडा.
5. APK `app/build/outputs/apk/debug/` मध्ये तयार होईल.

या environment मध्ये Android SDK/Gradle build tool उपलब्ध नसल्यामुळे इथे APK compile करून तपासलेला नाही.

## सुरक्षा सूचना
- Keystore key export करता येत नाही; app uninstall/data clear केल्यास encrypted data recover न होण्याची शक्यता असते.
- Encryption helper अजून app database शी integrate केलेला नाही.
- Release build साठी signing key स्वतः सुरक्षित ठेवा; APK मध्ये key कधीही embed करू नका.
- Accessibility service जोडण्यापूर्वी प्रत्येक action, permission screen, disclosure आणि user consent review करणे आवश्यक आहे.
- Offline असल्याचे प्रत्यक्ष verify करण्यासाठी manifest, APK permission list आणि runtime network tests करणे आवश्यक आहे.

## मूळ APK
या project मध्ये मूळ APK चे code/assets copy केलेले नाहीत. हे स्वतंत्र implementation आहे.
