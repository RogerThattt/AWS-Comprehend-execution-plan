# AWS-Comprehend-execution-plan

Demo Execution Plan: Amazon Comprehend Analysis
This plan outlines the process for demonstrating the text analysis capabilities of both the standard and medical versions of Amazon Comprehend using three distinct text examples.

Phase 1: Introduction and Setup (2 minutes)
Welcome & Disclaimer:
Welcome the audience to the demo.
State the disclaimer: "All text used in this demo is for reference purposes only, and I do not own or claim copyright for them."
Prerequisites:
Mention that a basic knowledge of Amazon Comprehend is helpful.
Reference an overview tutorial for beginners and provide a link.
Navigate to Comprehend:
Go to the AWS Management Console and navigate to the Amazon Comprehend service.
Briefly point out the two versions available on the landing page: the standard version and Comprehend Medical.
Phase 2: Standard Comprehend Analysis (5 minutes)
Launch Standard Comprehend:
Click on "Launch Amazon Comprehend" to enter the standard analysis console.
Use Case 1: Letter of Recommendation (Positive Sentiment)
Prepare Text: Have the text for a positive letter of recommendation ready to copy.
Analyze:
In the console, locate the "Input text" box for real-time analysis.
Delete the default sample text.
Paste the letter of recommendation text.
Click the "Analyze" button.
Review Results: Walk through each analysis tab:
Entities: Point out identified entities like PERSON, ORGANIZATION, and DATE.
Key Phrases: Read a few key phrases that Comprehend has extracted (e.g., "tremendous student," "huge asset").
Language: Show that the language was detected as "English" with high confidence.
PII: Check the PII tab and note that it correctly identified the person's name.
Sentiment: Emphasize that, as expected, the sentiment is overwhelmingly Positive with a high confidence score.
Syntax: Briefly show the syntax analysis, pointing out nouns and adjectives.
Use Case 2: Customer Review (Negative Sentiment)
Prepare Text: Have the text for a negative customer review ready.
Analyze:
Clear the previous text from the input box.
Paste the negative review text.
Click "Analyze".
Review Results:
Entities: Note that no entities were found (if they were intentionally removed from the source text).
Key Phrases: Highlight phrases that convey negative sentiment (e.g., "worst customer service," "need to be shut down").
Language: Confirm the language is English.
PII: Note the absence of PII.
Sentiment: Show that the sentiment is correctly identified as Negative with a high confidence score.
Phase 3: Comprehend Medical Analysis (5 minutes)
Launch Comprehend Medical:
Navigate back to the Comprehend landing page.
Select and launch Comprehend Medical.
Use Case 3: Clinical Trial Report
Prepare Text: Have the text from a clinical trial report ready.
Analyze:
Clear the default sample text.
Paste the clinical trial text into the input box.
Click "Analyze".
(Contingency): If the UI freezes, refresh the page, re-paste the text, and analyze again. You can mention this as a live "bug discovery."
Review Medical-Specific Results:
PHI / Entities: Show the detected medical entities. Point out MEDICATION (drug names), MEDICAL_CONDITION (e.g., pneumonia, infections), and TEST_TREATMENT_PROCEDURE.
RxNorm Concepts: Switch to this tab to show how the service links medications to their standardized RxNorm codes.
ICD-10-CM Concepts: Show how medical conditions are mapped to their standard ICD-10-CM diagnosis codes.
Suggest an Additional Use Case: Mention that this tool could be used to analyze a doctor's notes or prescription information to understand dosages, side effects, etc.
Phase 4: API Integration and Conclusion (1 minute)
Show API Integration:
Briefly navigate to the "Application integration" section in the console.
Explain that all the analysis shown can be performed programmatically using the Comprehend APIs.
Review API Response:
Show the example API call and the resulting JSON response, highlighting how the extracted entities and insights are structured.
Conclusion:
Summarize the demo, emphasizing the simplicity and power of using Amazon Comprehend for both standard and specialized medical text analysis.
Thank the audience for their time and conclude the demo.
