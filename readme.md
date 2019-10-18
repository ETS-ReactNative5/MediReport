<h1>MediReport</h1>
Easy and understandable medical records


<h1>Description</h1>
An application which enables end users to interpret the meanings of various medical/physiological parameters which are present in their medical reports or prescriptions.


<h1>Abstract</h1>
Everyone cannot read or understand the various medical jargon and paramters mentioned in their medical reports (lipid profile, CBC report, LFT, RFT, etc.). They usually have to take a day off from their schedules and visit their doctor/medical practioner to get a sense of their annual health reprts or even results of important tests. Our solution will save people time and money of a doctor's visit, by making an informed decision about their health using their medical reports. This will be useful particularly in the case of polulation located in remote areas where medical facilities are sparse.

We propose to build a React-based UI where user can upload their medical reports. React native will be used to implement the solution, which will enable the application to be ported to mobile platforms as well. 
Tesseract OCR and Aspose APIs will be used to extract medical report data while scanning the report. We will store RDF medical data from DBpedia and other datasets in MarkLogic. 
We will also be using various NLP/NLG libraries such as Apache OpenNLP, SimpleNLP etc., to generate human-like response for the user. 
Our Java-based system will interface with the RDF database and NLP/NLG libraries to send back repose to the UI.

We will provide support for multiple space-delimited languages for example, English, Spanish and all Indian languages. We will not able to support languages like Chinese, Japanese, Korean, Thai, Khmer whose writing systems that don't use spaces, since OpenNLP performs space-level token parsing.

<h1>Business Value</h1>
Limited literacy skills are one of the strongest predictors of poor health outcomes for patients. Studies have shown that when patients have low reading fluency, they know less about their chronic diseases, they are worse at managing their care<sup>[1]</sup>.


Overall, studies of patient-accessible medical records suggest modest improvements in doctor-patient communication, adherence, patient empowerment, and patient education<sup>[2]</sup>. 

MediReport will solve the following use cases - 

| Actor      | Use case |
| ----------- | ----------- |
| Patient trying to understand a medical report      | Patients often have difficulties understanding the clinical data presented in portals. In response, increasingly, patients either ignore their reports or go online<sup>[3]</sup> to make sense of this data. Medical infromation provided online in forums and discussion groups can lead to patient anxiety or such information may not always be applicable. Medireport will give the a one-stop solution for patients to understand their medical reports, the meaning and impact of each term (for ex., Bilirubin, Creatinine etc.) as well as ways to manage it  |
| Patient trying to understand a doctor's prescription   |  40-80% of medical information provided by healthcare practitioners is forgotten immediately. The greater the amount of information presented, the lower the proportion correctly recalled;<sup>[4]</sup> furthermore, almost half of the information that is remembered is incorrect.<sup>[5]</sup> To help patients in recalling and undestanding each prescribed medicine, MediReport will augment the prescription with explantion, categorization (antibiotic, antibacterial etc.) side-effects, medical usage, mode of action etc.        |
| Physicians trying to make a diagnosys | A study by Meyer and Payne<sup>[6]</sup> suggests that the association between physicians’ diagnostic accuracy and their confidence in that accuracy may be poor and that physicians may not request the required additional resources (ie, additional tests, second opinions, curbside consultations, referrals, and reference materials) to facilitate diagnosis when they most need it. These mismatched associations might prevent physicians from reexamining difficult cases when their diagnosis is incorrect. Improving these associations and the use of potential resources in handling difficult cases could potentially reduce diagnostic error. Medireport will help reduce diagnostic error by providing the physician the additional resources such as Signs and symptoms, Virology, Pathophysiology, Diagnosis, Prevention, Treatment, Management, Prognosis, etc. |
| Insurance company validating a claim | The insurers know a lot about you, based on claims. They aggregate data, such as imaging, medications, referrals, admissions, and emergency department visits, as well as quality metrics around severity-adjusted episodes of care for specific diagnoses<sup>[7]</sup>. MediReport will help insurance companies in making decisions about pre-existing conditions, valid claims, reporting malpractise etc. by providing them with a clear understanding of the thousands of medical terms and jargon that can be difficutl to remember. It will save insuracne company a lot of money by reducing work hours in understaning medical cases and well as reduce dependence on consultants that need to be paid high salaries. |

<h1>Architecture</h1>

![](https://github.com/SJSUFall2019-CMPE272/MediReport/blob/master/MediReport_archi_diagram.png)

<h1>Technology stack</h1>
React, OCR, OpenNLP, SimpleNLP Linked Open Data/Semantic Graph.

<h2>Technology choices</h2>
  | Actor      | Use case |
| ----------- | ----------- |
| x | x

<h1>Feedback</h1>
Professor Ranjan's initial reaction:

> I love this idea. Use NLG to generate commentary for users. I would stick to mobile app and make it useful for
> underprivileged users in rural area and support multiple languages such as spanish, hindi, tamil, telugu etc... 

<h1>Team</h1>

1. [Animesh Swain]()
1. [Anjana Menon Cherubala](https://github.com/AnjanaMenonCherubala)
1. [Sakshi Mahendru](https://github.com/sakshimahendrusjsu)
1. [Vini Aswal](https://github.com/vaswal)


<h1>References</h1>

1. Graham, S., & Brookey, J. (2008). Do patients understand?. The Permanente journal, 12(3), 67–69. doi:10.7812/tpp/07-144

2. Ross, S. E., & Lin, C. T. (2003). The effects of promoting patient access to medical records: a review. Journal of the American Medical Informatics Association : JAMIA, 10(2), 129–138. doi:10.1197/jamia.m1147

3. Reynolds, T. L., Ali, N., McGregor, E., O'Brien, T., Longhurst, C., Rosenberg, A. L., … Zheng, K. (2018). Understanding Patient Questions about their Medical Records in an Online Health Forum: Opportunity for Patient Portal Design. AMIA ... Annual Symposium proceedings. AMIA Symposium, 2017, 1468–1477.

4. McGuire LC. Remembering what the doctor said: organization and older adults' memory for medical information. Exp Aging Res 1996;22: 403-28

5. Anderson JL, Dodman S, Kopelman M, Fleming A. Patient information recall in a rheumatology clinic. Rheumatol Rehabil 1979;18: 245-55

6. Meyer AND, Payne VL, Meeks DW, Rao R, Singh H. Physicians’ Diagnostic Accuracy, Confidence, and Resource Requests: A Vignette Study. JAMA Intern Med. 2013;173(21):1952–1958. doi:10.1001/jamainternmed.2013.10081

7. Kaufman J. M. (2015). How to work with insurance companies. Neurology. Clinical practice, 5(5), 448–453. doi:10.1212/CPJ.0000000000000179
