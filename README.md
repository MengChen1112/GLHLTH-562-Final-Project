Executive summary
================
Shurui Wang, Meng Chen
2023-04-13

## Dataset

The dataset comes from the publicly available National Survey on Drug
Use and Health (NSDUH). Sponsored by the Substance Abuse and Mental
Health Services Administration (SAMHSA), the NSDUH is an annual,
nationally representative survey of individuals aged 12 years or older
from all 50 US states and the District of Columbia. It gathers data on
substance use, mental health, and other health-related topics.

## Research Questions

- Is there a significant association between any mental health illness
  (AMI) and a history of cancer in the United States?
- What are the risk factors of AMI among the whole cohort and
  individuals with a history of cancer?

## Methodology

#### Study Sample

We identified 44457 adults who participated in the NSDUH during 2021,
and 1998 among them reported a cancer history. Respondents with a cancer
history were identified from a survey question that asked whether
respondents were ever told by a physician or other health care
professional that they had cancer or a malignancy of any kind.

#### Outcome of Interest

AMI were determined with a multivariable prediction model developed by
the SAMHSA on the basis of the World Health Organization Disability
Assessment Schedule (a measure of functional impairment), in combination
with the Kessler Psychological Distress Scale, past-year serious
suicidal thoughts, past-year major depressive episodes, and age.

#### Predictors of Interest

Key correlates of AMI included demographic, socioeconomic, and clinical
characteristics. Demographic measures included age category (“Age”), sex
(“Sex”), and race/ethnicity (“Race”). Measures of socioeconomic status
included educational levels (“Education”). Measures of clinical
characteristics included health behaviors, assessed by illicit drug use
(“Drug”) and mental health service acceptance (“MH_service”).

#### Statistical Analysis

Firstly, we used the ggplot function in R to visualize the data and
obtained the baseline characteristics of the whole cohort as well as the
differences in AMI prevalence between individuals with and without a
history of cancer. Then, we conducted the chi-square test and multiple
logistic regression model to examine the association between AMI and
cancer history, with adjustments for demographic characteristics and
socioeconomic status. Finally, we performed a multiple logistic
regression model exclusively among individuals with a cancer history in
the cohort to identify the risk factors for AMI in cancer survivors.

## Findings

The prevalence of AMI among individuals with and without a history of
cancer is 22% and 27.1%, respectively. According to the chi-square test,
there is a significant association between AMI and a history of cancer
(p \< 0.001). Based on the multivariable regression, a history of cancer
is a risk factor for AMI among the whole cohort (OR=1.26; 95% CI,
1.11-1.44). The risk factors for AMI among the whole cohort are similar
to those among individuals with a history of cancer. As for cancer
patients, illicit drug use and being female are risk factors (OR=1.87;
95% CI, 1.44-2.43; OR=1.68; 95% CI, 1.29-2.20, respectively). Not
receiving mental health services and being 65 years old or older are
protective factors (OR=0.05; 95% CI, 0.01-0.17; OR=0.22; 95% CI,
0.14-0.33, respectively).
