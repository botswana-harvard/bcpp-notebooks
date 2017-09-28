# Forms
## HIV care and adherence
"A model completed by the user on the participant's access to
    and adherence to HIV care.
    

<b>Section: Main</b>

<b>1.0.</b> subject visit
* db_table: bcpp_subject_hivcareadherence
* column: subject_visit
* column_type: OneToOneField

<b>2.0.</b> When was your first positive HIV test result?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Note: If participant does not want to answer or is unable to estimate date, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: first_positive
* column_type: DateField
* format: YYYY-MM-DD

<b>Section: Care</b>

<b>3.0.</b> Have you ever received HIV-related medical or clinical care, for such things as a CD4 count (masole), IDCC/ PMTCT registration, additional clinic-based counseling?

&nbsp;&nbsp;&nbsp;&nbsp;<i>if 'YES', answer HIV medical care section</i>
* db_table: bcpp_subject_hivcareadherence
* column: medical_care
* column_type: CharField
* length: 25

<b>4.0.</b> If 'No', what is the main reason you have not received HIV-related medical or clinical care?
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care
* column_type: CharField
* length: 70

<b>4.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: no_medical_care_other
* column_type: CharField
* length: 35

<b>5.0.</b> Have you ever been recommended by a doctor/nurse or other healthcare worker to start antiretroviral therapy (ARVs), a combination of medicines to treat your HIV infection? 

&nbsp;&nbsp;&nbsp;&nbsp;<i>Common medicines include: combivir, truvada, atripla, nevirapine, dolutegravir</i>
* db_table: bcpp_subject_hivcareadherence
* column: ever_recommended_arv
* column_type: CharField
* length: 25

<b>6.0.</b> Have you ever taken any antiretroviral therapy (ARVs) for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp;<i>For women, do not include treatment that you took during pregnancy to protect your baby from HIV</i>
* db_table: bcpp_subject_hivcareadherence
* column: ever_taken_arv
* column_type: CharField
* length: 25

<b>7.0.</b> If 'No', What was the main reason why you have not started ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv
* column_type: CharField
* length: 75

<b>7.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: why_no_arv_other
* column_type: CharField
* length: 35

<b>Section: Antiretiroviral Therapy</b>

<b>8.0.</b> Are you currently taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes, need to answer next two questions.</i>
* db_table: bcpp_subject_hivcareadherence
* column: on_arv
* column_type: CharField
* length: 25

<b>9.0.</b> <span style="color:orange;">Interviewer: </span> Is there evidence that the participant is on therapy?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Examples of evidence might be OPD card, tablets, masa number, etc.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_evidence
* column_type: CharField
* length: 3

<b>10.0.</b> When did you first start taking antiretroviral therapy (ARVs)?

&nbsp;&nbsp;&nbsp;&nbsp;<i>Note: If participant does not want to answer or is unable to estimate date, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: first_arv
* column_type: DateField
* format: YYYY-MM-DD

<b>11.0.</b> When did you stop taking ARV's?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If not applicable, leave blank.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_date
* column_type: DateField
* format: YYYY-MM-DD

<b>12.0.</b> If 'stopped', what was the main reason why you stopped taking ARVs?
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop
* column_type: CharField
* length: 80

<b>12.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: arv_stop_other
* column_type: CharField
* length: 35

<b>13.0.</b> What ARV regimen are you currently prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: arvs
* column_type: ManyToManyField

<b>13.1.</b> If other ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp;<i>use three letter abbrevitions, if known.</i>
* db_table: bcpp_subject_hivcareadherence
* column: arv_other
* column_type: CharField
* length: 25

<b>14.0.</b> Is this the first regimen that you were prescribed for your HIV infection?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If the participant answered NO to the question above, record prior regimen and timing of switch.</i>
* db_table: bcpp_subject_hivcareadherence
* column: is_first_regimen
* column_type: CharField
* length: 25

<b>15.0.</b> Date switched to currently prescribed regimen above?
* db_table: bcpp_subject_hivcareadherence
* column: prev_switch_date
* column_type: DateField
* format: YYYY-MM-DD

<b>16.0.</b> What ARV regimen were you previously prescribed? Select each ARV in the regimen
* db_table: bcpp_subject_hivcareadherence
* column: prev_arvs
* column_type: ManyToManyField

<b>16.1.</b> If other previous ARV, or ARVs, not listed above, specify:

&nbsp;&nbsp;&nbsp;&nbsp;<i>use three letter abbrevitions, if known.</i>
* db_table: bcpp_subject_hivcareadherence
* column: prev_arv_other
* column_type: CharField
* length: 25

<b>Section: Adherence</b>

<b>17.0.</b> During the past 4 days, on how many days have you missed taking all your doses of antiretroviral therapy (ART)?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_day
* column_type: CharField
* length: 25

<b>18.0.</b> Thinking about the past 4 weeks, on average, how would you rate your ability to take all your medications as prescribed?
* db_table: bcpp_subject_hivcareadherence
* column: adherence_4_wk
* column_type: CharField
* length: 25

<b>Section: Hospitalization</b>

<b>19.0.</b> Were you admitted to the hospital during the ~6 months following the date on which you started ART

&nbsp;&nbsp;&nbsp;&nbsp;<i>If not applicable, skip to next section.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start
* column_type: CharField
* length: 25

<b>20.0.</b> About how many weeks or months after starting ART were you admitted to the hospital

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission. Format is phrase 'NN weeks' or 'NN months', e.g '5 months' or '13 weeks', etc.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_duration
* column_type: CharField
* length: 25

<b>21.0.</b> What was the primary reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission.</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason
* column_type: CharField
* length: 25

<b>21.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_art_start_reason_other
* column_type: CharField
* length: 35

<b>22.0.</b> If reason for hospitalization was related to a chronic disease, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: chronic_disease
* column_type: CharField
* length: 25

<b>23.0.</b> If reason for hospitalization was related to medication toxicity, specify which?
* db_table: bcpp_subject_hivcareadherence
* column: medication_toxicity
* column_type: CharField
* length: 25

<b>24.0.</b> What is the source of evidence for reason for the hospitalization?

&nbsp;&nbsp;&nbsp;&nbsp;<i>If yes to question about hospital admission</i>
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence
* column_type: CharField
* length: 25

<b>24.1.</b> If Other, specify ...
* db_table: bcpp_subject_hivcareadherence
* column: hospitalized_evidence_other
* column_type: CharField
* length: 35

<b>Section: Clinic</b>

<b>25.0.</b> Which clinic facility are you already receiving therapy from?
* db_table: bcpp_subject_hivcareadherence
* column: clinic_receiving_from
* column_type: CharField
* length: 50

<b>26.0.</b> When is your next appointment at this facility?
* db_table: bcpp_subject_hivcareadherence
* column: next_appointment_date
* column_type: DateField
* format: YYYY-MM-DD


Rendered on 20170928150340
