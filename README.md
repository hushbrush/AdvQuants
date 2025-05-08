# What You Trust Is Who You Are: Predicting Political Ideology Using InstitutionalConfidence


I’m trying to learn whether despite institutional trust levels being at al all time low in the
recent decades, trust in certain institutions is an indication of political leanings.
It is important because the relationship between certain institutions and political leaning
could affect the federal funding of those institutions(eg. the recent Harvard debacle).
Further, certain institutions like the press, which are considered pillars of democracy,
would ideally indicate whether a society believes itself to uphold a democracy or not,
which is inherently a political in nature.





## Research Questions

How much of a person's political identity depends on their trust?
Since trust in institutions is at an all time low in the past decade, the motivation is to learn about what value it holds in the political lives of Americans 



## Method 

I looked at all the 'trust in' variables--13 of them, and dummy coded to the highest value. Then I also dummy coded whether someone thinks of themselves as a liberal or a conservative
<img width="744" alt="clean_data" src="https://github.com/user-attachments/assets/81673dbc-0eda-401e-9cb0-00ac20d5fb63" />

Then I tried a couple of methods--
1. 

## Key Findings 

1. OLS(waste of time because binary output--we learnt this already but I still wanted to try.):
![auc_olsFInal](https://github.com/user-attachments/assets/823bb3d0-4e72-4c63-8bae-b332959d7b47)

2. Logit:
![auc_logstic](https://github.com/user-attachments/assets/1e0f1127-184f-430a-9f4e-b326a4d52b8f)

3. Random Forests:
   ![RandomForests_auc](https://github.com/user-attachments/assets/ba03fd9e-e5c9-497b-86c1-b31739e28419)

Conclusion (1 minute)

So what? Why should we care?

Any implications, surprises, or next steps?

