# Software Quality Assurance (SQA) - Manual Testing Project

## 📌 Project Overview
This repository contains a comprehensive manual testing report for an Android audio utility application (referred to here under the dummy name **"Audio Master: Sound Booster"** to maintain developer confidentiality). The objective of this audit was to identify functional, UI/UX, and performance-related defects to ensure a safe and high-quality user experience.

## 📱 Testing Environment
- **Device:** Vivo Y50
- **OS Version:** Android 10
- **Testing Type:** Manual Testing (Black Box), Functional Testing, UI/UX Testing, Performance Testing.

---

## 🐞 Bug Reports Summary
A total of **07 unique bugs** were identified during the testing phase. 

| Bug ID | Bug Title | Severity |
| :--- | :--- | :--- |
| **BUG-01** | Background audio pauses when advertisement starts. | High |
| **BUG-02** | Selected language does not apply to application UI. | High |
| **BUG-03** | High Battery Drain (~10.1 mAh) & Unexpected Data Usage (155.87 MB). | High |
| **BUG-04** | Volume increases without user confirmation after safety warning. | High |
| **BUG-05** | Background audio does not resume after advertisement ends. | Medium |
| **BUG-06** | Edge Light “Hole” effect is misaligned with camera cutout. | Medium |
| **BUG-07** | Text wrapping issue in “Waterdrop” label. | Low |

> *Note: Detailed execution steps, expected results, and actual results for each bug are documented in the testing files.*

---

## 📝 Test Cases Executed
**Core Feature Tested:** Boost system volume & app sound beyond default limits.

| Test Case ID | Test Scenario | Status |
| :--- | :--- | :--- |
| **TC-BST-01** | Verify boost limit restriction for free users. | Executed |
| **TC-BST-02** | Verify responsiveness of preset volume buttons. | Executed |
| **TC-BST-03** | Validate combined Boost and System volume calculation. | Executed |
| **TC-BST-04** | Verify functionality of the Mute button. | Executed |
| **TC-BST-05** | Verify automatic preset button selection based on combined levels. | Executed |

---

## 💡 Recommendations for Improvement

1. **Implement Gradual Volume Scaling (Safety First):** Volume should not increase immediately upon clicking a high-volume preset. Implement a 1-2 second ramp-up time *only after* the user taps the safety confirmation button to prevent sudden hearing damage.
   
2. **Optimize Background Data Management:** Restrict Ad SDKs and analytics from continuous background fetching to resolve the excessive 155MB data consumption and system power warnings.
   
3. **Enhance Localization & UI Scaling:** Correct the string mappings for language selection so the UI updates instantly. Utilize dynamic text scaling to prevent text wrapping issues (e.g., the "Waterdrop" label).

---

**👨‍💻 Tested By:** **Subhendu Bachhar Setu** *Software Quality Assurance Engineer (Intern) at SPARKTRO*

---

