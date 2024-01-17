![LogoTitle](Screenshots/Docucare_LogoTitle.png)

# Details

**Project** : DocuCare, trademark pending, is a Doctor Platform that transforms recorded medical information into concise summaries and actionable insights for both doctors and patients. The doctor is provided with immediate patient information, a summary of their past visits, real time analysis, and potential diagnosis. DocuCare aims to enhance the doctor-patient relationship through intelligent data utilization./ 

**Team Number** : 9  

**Team Name** : NA ACQ SA  

**Demonstration Video** : _Insert link to demonstration video_  

# Overview

DocuCare, trademark pending, is a Doctor-Patient Platform that transforms recorded medical information into concise summaries and actionable insights for both doctors and patients. Doctors can analyze similar symptoms across patients, while patients can ask follow-up questions based on their history, fostering efficient and informed healthcare communication. DocuCare aims to enhance the doctor-patient relationship through intelligent data utilization.

# Justification
 
DocuCare significantly enhances the patient experience in healthcare by providing immediate access to patient histories, in-depth real-time analyses, and potential diagnoses. Addressing the critical aspect of ‘Telemed Care Quality’, it ensures accurate remote diagnoses through intelligent data tools, thus improving the reliability of telemedicine. Additionally, it empowers lower-level care providers, like Nurse Practitioners and Physicians Assistants, with advanced analytical tools to improve their service standards. This innovation optimizes patient outcomes and boosts overall healthcare efficiency, marking DocuCare as a transformative force in medical consultations and patient care management.

Just like Docucare shows, MongoDB’s developer data platform allows organizations to integrates all of the data services you need to build modern applications in a unified developer experience. It handles transactional workloads, full-text search, AI-enhanced experiences, stream data processing, and more, all while reducing data infrastructure sprawl and complexity!

# Detailed Application Overview

Docucare uses a majority of Atlas components to achieve enhanced communication. Upon logging in, the doctor view is presented with a list of patients and a search bar all facilitated by App services HTTP endpoints and functions. A search bar powered by Atlas search for any mistakes (fuzzy matching) and autocomplete features to make our doctor's life easier. 

Once in a single patient view, the doctor has an overall view of the patient together with an AI generated summary covering his previous visits, any current medication, diagnosis etc. For patients with wearable devices, charts powered by Atlas charts connected to time series collections with continous vitals are also presented for the doctor to evaluate. The doctor then has a notepad to take notes during a visit, whereby we have combined AI to summarize the notes, but also in conjunction with our knowledge base using vector search to come up with potential conversational key topics to discuss as they work together towards a diagnosis. All this happens instantaneously using our app services. At the end of a session, a potential diagnosis and treatment option is presented as a potential path forward for the patient.

![Architecture Diagram](Screenshots/Docucare_Arch.png)


Docucare uses the following components:

* Atlas Database
* Atlas Full Text Search
* Atlas Vector Search
* Atlas App Services (functions, HTTP Endpoints)
* Azure OpenAI
* Kafka, Atlas Stream Processing and Time Series


# Roles and Responsibilities

* Aashish Regmi
   * Role: Backend Developer
   * Responsibility: write backend API endpoints, Atlas functions and HTTPS endpoints, search queries, prompt engineering with RAG
* Adlai Gordon
   * Role: Front Developer
   * Responsibility: react frontend development, graphic design 
* Allan Schiebold
   * Role: Data Engineer
   * Responsibility: generate sample Data, write aggregation queries, architecture diagram, documentation, presentation slides, Charts design
* Brent Dorenkamp
   * Role: Data Engineer
   * Responsibility: generate sample data, video recording, documentation, presentation slides 
* Clarence Ondieki
   * Role: Backend Tech Lead
   * Responsibility: led backend tasks planning/assignment, tech support to the team, backend API endpoints development, Atlas HTTPS endpoints, Atlas functions, full text and vector search queries, contribute to README.md   
* Michael Pepe
   * Role: Domain Expert, Tech Consultant
   * Responsibility: architecture diagram, script generation, healthcare consulting, use case development
* Travis Williams
   * Role: Frontend Tech Lead, General Coach
   * Responsibility: led hackathon planning, tech support to the team, Azure openAI lead, application architecture design, react frontend development
* Yang Li
   * Role: Backend Developer 
   * Responsibility: load data, generate embeddings, search queries, Atlas functions, contribute to README.md and architecture diagram  
* Younes Berrada
   * Role: Frontend and Backend Developer
   * Responsibility: IoT gateway, time series, Atlas Charts, Kafka connector, Atlas Stream Processing

# Demonstration Script

[Link to Demo Script](https://docs.google.com/document/d/1S3HQ6OyRCZbtwYpagZiMd62OquFzhko6_jHgirLheAY/edit?usp=sharing)
