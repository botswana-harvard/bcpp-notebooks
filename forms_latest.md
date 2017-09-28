# Forms
## HIV care and adherence
"A model completed by the user on the participant's access to
    and adherence to HIV care.
    

<b>Section: Main</b>

<b>1.0.</b> subject visit
* db_table: bcpp_subject_hivcareadherence
* column: subject_visit
* column_type: OneToOneField
---

<b>2.0.</b> When was your first positive HIV test result?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Note: If participant does not want to answer or is unable to estimate date, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: first_positive
* column_type: DateField
* format: YYYY-MM-DD
---

<b>Section: Care</b>

<b>3.0.</b> Have you ever received HIV-related medical or clinical care, for such things as a CD4 count (masole), IDCC/ PMTCT registration, additional clinic-based counseling?

&nbsp;&nbsp;&nbsp;&nbsp;<i>if 'YES', answer HIV medical care section</i>
* db_table: bcpp_subject_hivcareadherence
* column: medical_care
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>4.0.</b> If 'No', what is the main reason you have not received HIV-related medical or clinical care?
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care
* column_type: CharField
* length: 70
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `Did not feel sick`: <i>Did not feel sick</i> 
  - `Did not know I should get HIV care`: <i>Did not know I should get HIV care</i> 
  - `Did not have time due to work responsibilities`: <i>Did not have time due to work responsibilities</i> 
  - `Did not have time due to family/childcare responsibilities`: <i>Did not have time due to family/childcare responsibilities</i> 
  - `Transportation costs`: <i>Transportation costs</i> 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: <i>Was afraid of someone (friends/family) seeing me at the HIV clinic</i> 
  - `Traditional healer advised against going`: <i>Traditional healer advised against going</i> 
  - `Religious beliefs`: <i>Religious beliefs</i> 
  - `Cultural beliefs`: <i>Cultural beliefs</i> 
  - `Not provided free of charge for non-citizens`: <i>Not provided free of charge for non-citizens</i> 
  - `OTHER`: <i>Other, specify:</i> 
  - `not_sure`: <i>I am not sure</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>4.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care_other
* column_type: CharField
* length: 35
* responses: <i>free text</i>
---

<b>5.0.</b> Have you ever been recommended by a doctor/nurse or other healthcare worker to start antiretroviral therapy (ARVs), a combination of medicines to treat your HIV infection? 

&nbsp;&nbsp;&nbsp;&nbsp;<i>Common medicines include: combivir, truvada, atripla, nevirapine, dolutegravir</i>
* db_table: bcpp_subject_hivcareadherence
* column: ever_recommended_arv
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>6.0.</b> Have you ever taken any antiretroviral therapy (ARVs) for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp;<i>For women, do not include treatment that you took during pregnancy to protect your baby from HIV</i>
* db_table: bcpp_subject_hivcareadherence
* column: ever_taken_arv
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>7.0.</b> If 'No', What was the main reason why you have not started ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv
* column_type: CharField
* length: 75
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `Did not feel sick`: <i>Did not feel sick</i> 
  - `Was afraid treatment would make me feel bad/sick`: <i>Was afraid treatment  would make me feel bad/sick</i> 
  - `Difficulty finding someone to go with me for counseling (mopati)`: <i>Difficulty finding someone to go with me for counseling (mopati)</i> 
  - `Hard due to work responsibilities`: <i>Hard due to work responsibilities</i> 
  - `Hard due to family/childcare responsibilities`: <i>Hard due to family/childcare responsibilities</i> 
  - `Transportation costs`: <i>Transportation costs</i> 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: <i>Was afraid of someone (friends/family) seeing me at the HIV clinic</i> 
  - `Sexual partner advised against taking`: <i>Sexual partner advised against taking</i> 
  - `Family or friends advised against taking`: <i>Family or friends advised against taking</i> 
  - `Traditional healer advised against taking`: <i>Traditional healer advised against taking</i> 
  - `Religious beliefs`: <i>Religious beliefs</i> 
  - `Cultural beliefs`: <i>Cultural beliefs</i> 
  - `High CD4`: <i>High CD4</i> 
  - `Cost`: <i>Cost</i> 
  - `OTHER`: <i>Other, specify:</i> 
  - `not_sure`: <i>I am not sure</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>7.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv_other
* column_type: CharField
* length: 35
* responses: <i>free text</i>
---

<b>Section: Antiretiroviral Therapy</b>

<b>8.0.</b> Are you currently taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes, need to answer next two questions.</i>
* db_table: bcpp_subject_hivcareadherence
* column: on_arv
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `DWTA`: <i>Don't want to answer</i> 
  - `N/A`: <i>Not applicable</i> 
---

<b>9.0.</b> <span style="color:orange;">Interviewer: </span> Is there evidence that the participant is on therapy?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Examples of evidence might be OPD card, tablets, masa number, etc.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_evidence
* column_type: CharField
* length: 3
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `N/A`: <i>Not applicable</i> 
---

<b>10.0.</b> When did you first start taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Note: If participant does not want to answer or is unable to estimate date, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: first_arv
* column_type: DateField
* format: YYYY-MM-DD
---

<b>11.0.</b> When did you stop taking ARV's?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If not applicable, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_date
* column_type: DateField
* format: YYYY-MM-DD
---

<b>12.0.</b> If 'stopped', what was the main reason why you stopped taking ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop
* column_type: CharField
* length: 80
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `Did not feel they were helping`: <i>Did not feel they were helping</i> 
  - `ARVs made me feel bad or sick`: <i>ARVs made me feel bad or sick</i> 
  - `Difficulty finding someone to go with me for counseling (mopati)`: <i>Difficulty finding someone to go with me for counseling (mopati)</i> 
  - `Hard due to work responsibilities`: <i>Hard due to work responsibilities</i> 
  - `Hard due to family/childcare responsibilities`: <i>Hard due to family/childcare responsibilities</i> 
  - `Doctor or nurse at clinic told me to stop`: <i>Doctor or nurse at clinic told me to stop</i> 
  - `Transportation costs`: <i>Transportation costs</i> 
  - `Cost/could not afford`: <i>Cost/could not afford</i> 
  - `Was afraid of someone (friends/family) seeing me at the HIV clinic`: <i>Was afraid of someone (friends/family) seeing me at the HIV clinic</i> 
  - `Sexual partner advised against taking`: <i>Sexual partner advised against taking</i> 
  - `Family or friends advised against taking`: <i>Family or friends advised against taking</i> 
  - `Traditional healer advised against taking`: <i>Traditional healer advised against taking</i> 
  - `Religious beliefs`: <i>Religious beliefs</i> 
  - `Cultural beliefs`: <i>Cultural beliefs</i> 
  - `OTHER`: <i>Other, specify:</i> 
  - `not_sure`: <i>I am not sure</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>12.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_other
* column_type: CharField
* length: 35
* responses: <i>free text</i>
---

<b>13.0.</b> What ARV regimen are you currently prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: arvs
* column_type: ManyToManyField
* responses: <i>Select all that apply</i>
  - `Efavirenz`: <i>EFV (Stocrin, Sustiva)</i> 
  - `Zidovudine/lamivudine`: <i>ZDV/3TC or AZT/3TC (Combivir)</i> 
  - `Lopinavir/ritonavir`: <i>LPV/r (Aluvia, Kaletra)</i> 
  - `Abacavir/lamivudine`: <i>ABC/3TC (Epzicom)</i> 
  - `Lamivudine`: <i>3TC (Epivir)</i> 
  - `Atazanavir`: <i>ATV (Reyataz)</i> 
  - `Tenofovir/emtricitabine`: <i>TDF/FTC (Truvada)</i> 
  - `Saquinavir`: <i>SQV (Invirase)</i> 
  - `Dolutegravir`: <i>DTG (Tivicay)</i> 
  - `Zidovudine`: <i>ZDV or AZT (Retrovir)</i> 
  - `Nevirapine`: <i>NVP (Viramune)</i> 
  - `Ritonavir`: <i>RTV or r (Norvir)</i> 
  - `Tenofovir`: <i>TDF (Viread)</i> 
  - `Stavudine`: <i>D4T (Zerit)</i> 
  - `OTHER`: <i> OTHER drug not listed: specify below ...</i> 
  - `Raltegravir`: <i>RAL (Isentress)</i> 
  - `Abacavir`: <i>ABC (Ziagen)</i> 
  - `Darunavir`: <i>DRV (Prezista)</i> 
  - `Didanosine`: <i>ddI (Videx)</i> 
---

<b>13.1.</b> If other ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp;<i>use three letter abbrevitions, if known.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_other
* column_type: CharField
* length: 25
* responses: <i>free text</i>
---

<b>14.0.</b> Is this the first regimen that you were prescribed for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If the participant answered NO to the question above, record prior regimen and timing of switch.</i>
* db_table: bcpp_subject_hivcareadherence
* column: is_first_regimen
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes, this is the first regimen</i> 
  - `No`: <i>No, I previously took at least 1 different ARV (and was switched to this regimen)</i> 
---

<b>15.0.</b> Date switched to currently prescribed regimen above?
* db_table: bcpp_subject_hivcareadherence
* column: prev_switch_date
* column_type: DateField
* format: YYYY-MM-DD
---

<b>16.0.</b> What ARV regimen were you previously prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: prev_arvs
* column_type: ManyToManyField
* responses: <i>Select all that apply</i>
  - `Efavirenz`: <i>EFV (Stocrin, Sustiva)</i> 
  - `Zidovudine/lamivudine`: <i>ZDV/3TC or AZT/3TC (Combivir)</i> 
  - `Lopinavir/ritonavir`: <i>LPV/r (Aluvia, Kaletra)</i> 
  - `Abacavir/lamivudine`: <i>ABC/3TC (Epzicom)</i> 
  - `Lamivudine`: <i>3TC (Epivir)</i> 
  - `Atazanavir`: <i>ATV (Reyataz)</i> 
  - `Tenofovir/emtricitabine`: <i>TDF/FTC (Truvada)</i> 
  - `Saquinavir`: <i>SQV (Invirase)</i> 
  - `Dolutegravir`: <i>DTG (Tivicay)</i> 
  - `Zidovudine`: <i>ZDV or AZT (Retrovir)</i> 
  - `Nevirapine`: <i>NVP (Viramune)</i> 
  - `Ritonavir`: <i>RTV or r (Norvir)</i> 
  - `Tenofovir`: <i>TDF (Viread)</i> 
  - `Stavudine`: <i>D4T (Zerit)</i> 
  - `OTHER`: <i> OTHER drug not listed: specify below ...</i> 
  - `Raltegravir`: <i>RAL (Isentress)</i> 
  - `Abacavir`: <i>ABC (Ziagen)</i> 
  - `Darunavir`: <i>DRV (Prezista)</i> 
  - `Didanosine`: <i>ddI (Videx)</i> 
---

<b>16.1.</b> If other previous ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp;<i>use three letter abbrevitions, if known.</i>
* db_table: bcpp_subject_hivcareadherence
* column: prev_arv_other
* column_type: CharField
* length: 25
* responses: <i>free text</i>
---

<b>Section: Adherence</b>

<b>17.0.</b> During the past 4 days, on how many days have you missed taking all your doses of antiretroviral therapy (ART)?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_day
* column_type: CharField
* length: 25
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `Zero`: <i>Zero days</i> 
  - `One day`: <i>One day</i> 
  - `Two days`: <i>Two days</i> 
  - `Three days`: <i>Three days</i> 
  - `Four days`: <i>Four days</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>18.0.</b> Thinking about the past 4 weeks, on average, how would you rate your ability to take all your medications as prescribed?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_wk
* column_type: CharField
* length: 25
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `Very poor`: <i>Very poor</i> 
  - `Poor`: <i>Poor</i> 
  - `Fair`: <i>Fair</i> 
  - `Good`: <i>Good</i> 
  - `Very good`: <i>Very good</i> 
  - `DWTA`: <i>Don't want to answer</i> 
---

<b>Section: Hospitalization</b>

<b>19.0.</b> Were you admitted to the hospital during the ~6 months following the date on which you started ART

&nbsp;&nbsp;&nbsp;&nbsp;<i>If not applicable, skip to next section.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start
* column_type: CharField
* length: 25
* responses:
  - `Yes`: <i>Yes</i> 
  - `No`: <i>No</i> 
  - `N/A`: <i>Not applicable</i> 
---

<b>20.0.</b> About how many weeks or months after starting ART were you admitted to the hospital

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission. Format is phrase 'NN weeks' or 'NN months', e.g '5 months' or '13 weeks', etc.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_duration
* column_type: CharField
* length: 25
* responses: <i>free text</i>
---

<b>21.0.</b> What was the primary reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason
* column_type: CharField
* length: 25
* responses:
  - `N/A`: <i>Not applicable</i> 
  - `tb`: <i>Tuberculosis (TB, MTB)</i> 
  - `pneumonia`: <i>Pneumonia</i> 
  - `crypto_meningitis`: <i>Cryptococcal meningitis</i> 
  - `IRIS`: <i>Immune Reconstitution Inflammatory Syndrome (IRIS)</i> 
  - `OTHER_hiv_related`: <i>Other HIV-related illness</i> 
  - `pregnancy_related`: <i>Pregnancy-related care, including delivery</i> 
  - `injury_accident`: <i>Injury or accident</i> 
  - `chronic_disease`: <i>Chronic disease related care, including high blood pressure, diabetes, cancer, mental illness (specify which)</i> 
  - `stroke`: <i>Stroke (or suspected stroke)</i> 
  - `medication_toxicity`: <i>Medication toxicity (specify)</i> 
  - `OTHER`: <i>Other (specify)</i> 
  - `dont_know`: <i>Don't know</i> 
---

<b>21.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason_other
* column_type: CharField
* length: 35
* responses: <i>free text</i>
---

<b>22.0.</b> If reason for hospitalization was related to a chronic disease, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: chronic_disease
* column_type: CharField
* length: 25
* responses: <i>free text</i>
---

<b>23.0.</b> If reason for hospitalization was related to medication toxicity, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: medication_toxicity
* column_type: CharField
* length: 25
* responses: <i>free text</i>
---

<b>24.0.</b> What is the source of evidence for reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence
* column_type: CharField
* length: 25
* responses:
  - `Self-report`: <i>Self report</i> 
  - `Medical-card`: <i>Medical Card</i> 
  - `Both`: <i>Both</i> 
  - `OTHER`: <i>Other reason, specify</i> 
---

<b>24.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence_other
* column_type: CharField
* length: 35
* responses: <i>free text</i>
---

<b>Section: Clinic</b>

<b>25.0.</b> Which clinic facility are you already receiving therapy from?
* db_table: bcpp_subject_hivcareadherence
* column: clinic_receiving_from
* column_type: CharField
* length: 50
* responses: <i>free text</i>
---

<b>26.0.</b> When is your next appointment at this facility?
* db_table: bcpp_subject_hivcareadherence
* column: next_appointment_date
* column_type: DateField
* format: YYYY-MM-DD
---


Rendered on 20170928170147
