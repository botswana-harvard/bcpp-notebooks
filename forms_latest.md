# Forms
## HIV care and adherence
"A model completed by the user on the participant's access to
    and adherence to HIV care.
    
*Instructions*: Please complete the questions below. Required questions are in bold. When all required questions are complete click SAVE. Based on your responses, additional questions may be required or some answers may need to be corrected.

*Additional instructions*: This section is only to be completed by HIV-positive participants who knew that they were HIV-positive before today. Section should be skipped for HIV-negative participants and participants who first tested HIV-positive today.<H5><span style="color:orange;">Read to Participant</span></H5>I am now going to ask you some questions about care you may have been given for your HIV infection.


**Section: Main**

**1.0.** subject visit
* db_table: bcpp_subject_hivcareadherence
* column: subject_visit
* type: OneToOneField
---

**2.0.** When was your first positive HIV test result?

&nbsp;&nbsp;&nbsp;&nbsp; *Note: If participant does not want to answer or is unable to estimate date, leave blank.*
* db_table: bcpp_subject_hivcareadherence
* column: first_positive
* type: DateField
* format: YYYY-MM-DD
---

**Section: Care**

**3.0.** Have you ever received HIV-related medical or clinical care, for such things as a CD4 count (masole), IDCC/ PMTCT registration, additional clinic-based counseling?

&nbsp;&nbsp;&nbsp;&nbsp; *if 'YES', answer HIV medical care section*
* db_table: bcpp_subject_hivcareadherence
* column: medical_care
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `DWTA`: *Don't want to answer* 
---

**4.0.** If 'No', what is the main reason you have not received HIV-related medical or clinical care?
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care
* type: CharField
* length: 70
* responses:
  - `N/A`: *Not applicable* 
  - `Did not feel sick`: *Did not feel sick* 
  - `Did not know I should get HIV care`: *Did not know I should get HIV care* 
  - `Did not have time due to work responsibilities`: *Did not have time due to work responsibilities* 
  - `Did not have time due to family/childcare responsibilities`: *Did not have time due to family/childcare responsibilities* 
  - `Transportation costs`: *Transportation costs* 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: *Was afraid of someone (friends/family) seeing me at the HIV clinic* 
  - `Traditional healer advised against going`: *Traditional healer advised against going* 
  - `Religious beliefs`: *Religious beliefs* 
  - `Cultural beliefs`: *Cultural beliefs* 
  - `Not provided free of charge for non-citizens`: *Not provided free of charge for non-citizens* 
  - `OTHER`: *Other, specify:* 
  - `not_sure`: *I am not sure* 
  - `DWTA`: *Don't want to answer* 
---

**4.1.** If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care_other
* type: CharField
* length: 35
* responses: *free text*
---

**5.0.** Have you ever been recommended by a doctor/nurse or other healthcare worker to start antiretroviral therapy (ARVs), a combination of medicines to treat your HIV infection? 

&nbsp;&nbsp;&nbsp;&nbsp; *Common medicines include: combivir, truvada, atripla, nevirapine, dolutegravir*
* db_table: bcpp_subject_hivcareadherence
* column: ever_recommended_arv
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `DWTA`: *Don't want to answer* 
---

**6.0.** Have you ever taken any antiretroviral therapy (ARVs) for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp; *For women, do not include treatment that you took during pregnancy to protect your baby from HIV*
* db_table: bcpp_subject_hivcareadherence
* column: ever_taken_arv
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `DWTA`: *Don't want to answer* 
---

**7.0.** If 'No', What was the main reason why you have not started ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv
* type: CharField
* length: 75
* responses:
  - `N/A`: *Not applicable* 
  - `Did not feel sick`: *Did not feel sick* 
  - `Was afraid treatment would make me feel bad/sick`: *Was afraid treatment  would make me feel bad/sick* 
  - `Difficulty finding someone to go with me for counseling (mopati)`: *Difficulty finding someone to go with me for counseling (mopati)* 
  - `Hard due to work responsibilities`: *Hard due to work responsibilities* 
  - `Hard due to family/childcare responsibilities`: *Hard due to family/childcare responsibilities* 
  - `Transportation costs`: *Transportation costs* 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: *Was afraid of someone (friends/family) seeing me at the HIV clinic* 
  - `Sexual partner advised against taking`: *Sexual partner advised against taking* 
  - `Family or friends advised against taking`: *Family or friends advised against taking* 
  - `Traditional healer advised against taking`: *Traditional healer advised against taking* 
  - `Religious beliefs`: *Religious beliefs* 
  - `Cultural beliefs`: *Cultural beliefs* 
  - `High CD4`: *High CD4* 
  - `Cost`: *Cost* 
  - `OTHER`: *Other, specify:* 
  - `not_sure`: *I am not sure* 
  - `DWTA`: *Don't want to answer* 
---

**7.1.** If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv_other
* type: CharField
* length: 35
* responses: *free text*
---

**Section: Antiretiroviral Therapy**

**8.0.** Are you currently taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp; *If yes, need to answer next two questions.*
* db_table: bcpp_subject_hivcareadherence
* column: on_arv
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `DWTA`: *Don't want to answer* 
  - `N/A`: *Not applicable* 
---

**9.0.** <span style="color:orange;">Interviewer: </span> Is there evidence that the participant is on therapy?

&nbsp;&nbsp;&nbsp;&nbsp; *Examples of evidence might be OPD card, tablets, masa number, etc.*
* db_table: bcpp_subject_hivcareadherence
* column: arv_evidence
* type: CharField
* length: 3
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `N/A`: *Not applicable* 
---

**10.0.** When did you first start taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp; *Note: If participant does not want to answer or is unable to estimate date, leave blank.*
* db_table: bcpp_subject_hivcareadherence
* column: first_arv
* type: DateField
* format: YYYY-MM-DD
---

**11.0.** When did you stop taking ARV's?

&nbsp;&nbsp;&nbsp;&nbsp; *If not applicable, leave blank.*
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_date
* type: DateField
* format: YYYY-MM-DD
---

**12.0.** If 'stopped', what was the main reason why you stopped taking ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop
* type: CharField
* length: 80
* responses:
  - `N/A`: *Not applicable* 
  - `Did not feel they were helping`: *Did not feel they were helping* 
  - `ARVs made me feel bad or sick`: *ARVs made me feel bad or sick* 
  - `Difficulty finding someone to go with me for counseling (mopati)`: *Difficulty finding someone to go with me for counseling (mopati)* 
  - `Hard due to work responsibilities`: *Hard due to work responsibilities* 
  - `Hard due to family/childcare responsibilities`: *Hard due to family/childcare responsibilities* 
  - `Doctor or nurse at clinic told me to stop`: *Doctor or nurse at clinic told me to stop* 
  - `Transportation costs`: *Transportation costs* 
  - `Cost/could not afford`: *Cost/could not afford* 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: *Was afraid of someone (friends/family) seeing me at the HIV clinic* 
  - `Sexual partner advised against taking`: *Sexual partner advised against taking* 
  - `Family or friends advised against taking`: *Family or friends advised against taking* 
  - `Traditional healer advised against taking`: *Traditional healer advised against taking* 
  - `Religious beliefs`: *Religious beliefs* 
  - `Cultural beliefs`: *Cultural beliefs* 
  - `OTHER`: *Other, specify:* 
  - `not_sure`: *I am not sure* 
  - `DWTA`: *Don't want to answer* 
---

**12.1.** If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_other
* type: CharField
* length: 35
* responses: *free text*
---

**13.0.** What ARV regimen are you currently prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: arvs
* type: ManyToManyField
* responses: *Select all that apply*
  - `Efavirenz`: *EFV (Stocrin, Sustiva)* 
  - `Zidovudine/lamivudine`: *ZDV/3TC or AZT/3TC (Combivir)* 
  - `Lopinavir/ritonavir`: *LPV/r (Aluvia, Kaletra)* 
  - `Abacavir/lamivudine`: *ABC/3TC (Epzicom)* 
  - `Lamivudine`: *3TC (Epivir)* 
  - `Atazanavir`: *ATV (Reyataz)* 
  - `Tenofovir/emtricitabine`: *TDF/FTC (Truvada)* 
  - `Saquinavir`: *SQV (Invirase)* 
  - `Dolutegravir`: *DTG (Tivicay)* 
  - `Zidovudine`: *ZDV or AZT (Retrovir)* 
  - `Nevirapine`: *NVP (Viramune)* 
  - `Ritonavir`: *RTV or r (Norvir)* 
  - `Tenofovir`: *TDF (Viread)* 
  - `Stavudine`: *D4T (Zerit)* 
  - `OTHER`: * OTHER drug not listed: specify below ...* 
  - `Raltegravir`: *RAL (Isentress)* 
  - `Abacavir`: *ABC (Ziagen)* 
  - `Darunavir`: *DRV (Prezista)* 
  - `Didanosine`: *ddI (Videx)* 
---

**13.1.** If other ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp; *use three letter abbrevitions, if known.*
* db_table: bcpp_subject_hivcareadherence
* column: arv_other
* type: CharField
* length: 25
* responses: *free text*
---

**14.0.** Is this the first regimen that you were prescribed for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp; *If the participant answered NO to the question above, record prior regimen and timing of switch.*
* db_table: bcpp_subject_hivcareadherence
* column: is_first_regimen
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes, this is the first regimen* 
  - `No`: *No, I previously took at least 1 different ARV (and was switched to this regimen)* 
---

**15.0.** Date switched to currently prescribed regimen above?
* db_table: bcpp_subject_hivcareadherence
* column: prev_switch_date
* type: DateField
* format: YYYY-MM-DD
---

**16.0.** What ARV regimen were you previously prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: prev_arvs
* type: ManyToManyField
* responses: *Select all that apply*
  - `Efavirenz`: *EFV (Stocrin, Sustiva)* 
  - `Zidovudine/lamivudine`: *ZDV/3TC or AZT/3TC (Combivir)* 
  - `Lopinavir/ritonavir`: *LPV/r (Aluvia, Kaletra)* 
  - `Abacavir/lamivudine`: *ABC/3TC (Epzicom)* 
  - `Lamivudine`: *3TC (Epivir)* 
  - `Atazanavir`: *ATV (Reyataz)* 
  - `Tenofovir/emtricitabine`: *TDF/FTC (Truvada)* 
  - `Saquinavir`: *SQV (Invirase)* 
  - `Dolutegravir`: *DTG (Tivicay)* 
  - `Zidovudine`: *ZDV or AZT (Retrovir)* 
  - `Nevirapine`: *NVP (Viramune)* 
  - `Ritonavir`: *RTV or r (Norvir)* 
  - `Tenofovir`: *TDF (Viread)* 
  - `Stavudine`: *D4T (Zerit)* 
  - `OTHER`: * OTHER drug not listed: specify below ...* 
  - `Raltegravir`: *RAL (Isentress)* 
  - `Abacavir`: *ABC (Ziagen)* 
  - `Darunavir`: *DRV (Prezista)* 
  - `Didanosine`: *ddI (Videx)* 
---

**16.1.** If other previous ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp; *use three letter abbrevitions, if known.*
* db_table: bcpp_subject_hivcareadherence
* column: prev_arv_other
* type: CharField
* length: 25
* responses: *free text*
---

**Section: Adherence**

**17.0.** During the past 4 days, on how many days have you missed taking all your doses of antiretroviral therapy (ART)?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_day
* type: CharField
* length: 25
* responses:
  - `N/A`: *Not applicable* 
  - `Zero`: *Zero days* 
  - `One day`: *One day* 
  - `Two days`: *Two days* 
  - `Three days`: *Three days* 
  - `Four days`: *Four days* 
  - `DWTA`: *Don't want to answer* 
---

**18.0.** Thinking about the past 4 weeks, on average, how would you rate your ability to take all your medications as prescribed?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_wk
* type: CharField
* length: 25
* responses:
  - `N/A`: *Not applicable* 
  - `Very poor`: *Very poor* 
  - `Poor`: *Poor* 
  - `Fair`: *Fair* 
  - `Good`: *Good* 
  - `Very good`: *Very good* 
  - `DWTA`: *Don't want to answer* 
---

**Section: Hospitalization**

**19.0.** Were you admitted to the hospital during the ~6 months following the date on which you started ART

&nbsp;&nbsp;&nbsp;&nbsp; *If not applicable, skip to next section.*
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start
* type: CharField
* length: 25
* responses:
  - `Yes`: *Yes* 
  - `No`: *No* 
  - `N/A`: *Not applicable* 
---

**20.0.** About how many weeks or months after starting ART were you admitted to the hospital

&nbsp;&nbsp;&nbsp;&nbsp; *If yes to question about hospital admission. Format is phrase 'NN weeks' or 'NN months', e.g '5 months' or '13 weeks', etc.*
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_duration
* type: CharField
* length: 25
* responses: *free text*
---

**21.0.** What was the primary reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp; *If yes to question about hospital admission.*
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason
* type: CharField
* length: 25
* responses:
  - `N/A`: *Not applicable* 
  - `tb`: *Tuberculosis (TB, MTB)* 
  - `pneumonia`: *Pneumonia* 
  - `crypto_meningitis`: *Cryptococcal meningitis* 
  - `IRIS`: *Immune Reconstitution Inflammatory Syndrome (IRIS)* 
  - `OTHER_hiv_related`: *Other HIV-related illness* 
  - `pregnancy_related`: *Pregnancy-related care, including delivery* 
  - `injury_accident`: *Injury or accident* 
  - `chronic_disease`: *Chronic disease related care, including high blood pressure, diabetes, cancer, mental illness (specify which)* 
  - `stroke`: *Stroke (or suspected stroke)* 
  - `medication_toxicity`: *Medication toxicity (specify)* 
  - `OTHER`: *Other (specify)* 
  - `dont_know`: *Don't know* 
---

**21.1.** If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason_other
* type: CharField
* length: 35
* responses: *free text*
---

**22.0.** If reason for hospitalization was related to a chronic disease, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: chronic_disease
* type: CharField
* length: 25
* responses: *free text*
---

**23.0.** If reason for hospitalization was related to medication toxicity, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: medication_toxicity
* type: CharField
* length: 25
* responses: *free text*
---

**24.0.** What is the source of evidence for reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp; *If yes to question about hospital admission*
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence
* type: CharField
* length: 25
* responses:
  - `Self-report`: *Self report* 
  - `Medical-card`: *Medical Card* 
  - `Both`: *Both* 
  - `OTHER`: *Other reason, specify* 
---

**24.1.** If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence_other
* type: CharField
* length: 35
* responses: *free text*
---

**Section: Clinic**

**25.0.** Which clinic facility are you already receiving therapy from?
* db_table: bcpp_subject_hivcareadherence
* column: clinic_receiving_from
* type: CharField
* length: 50
* responses: *free text*
---

**26.0.** When is your next appointment at this facility?
* db_table: bcpp_subject_hivcareadherence
* column: next_appointment_date
* type: DateField
* format: YYYY-MM-DD


*Rendered on 2017-09-28 21:03*

---