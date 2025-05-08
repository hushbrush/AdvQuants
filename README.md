# What You Trust Is Who You Are: Predicting Political Ideology Using Institutional Confidence


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

I looked at all the 'trust in' variables--13 of them, and dummy coded to the highest value. Then I also dummy coded whether someone thinks of themselves as a liberal or a conservative.
<img width="744" alt="clean_data" src="https://github.com/user-attachments/assets/81673dbc-0eda-401e-9cb0-00ac20d5fb63" />

In Literature Review--
https://gss.norc.org/content/dam/gss/get-documentation/pdf/reports/social-change-reports/SC54%20Trends%20in%20Confidence%20in%20Institutions.pdf
<img width="774" alt="Screenshot 2025-05-08 at 3 52 24 PM" src="https://github.com/user-attachments/assets/231e614e-81ea-44bc-b8f5-6a4455c3961c" />


Then I tried a couple of methods--

1. OLS(waste of time because binary output--we learnt this already but I still wanted to try.):
   
![auc_olsFInal](https://github.com/user-attachments/assets/823bb3d0-4e72-4c63-8bae-b332959d7b47)

3. Logit:
   
![auc_logstic](https://github.com/user-attachments/assets/1e0f1127-184f-430a-9f4e-b326a4d52b8f)


4. Random Forests:
   
![RandomForests_auc](https://github.com/user-attachments/assets/ba03fd9e-e5c9-497b-86c1-b31739e28419)


## Key Findings 

1. Trust in exec_branch_of_fed_govt in 2016 made you most likely to be liberal- explains about 31%--checks out, because back then there was a Democrat President. 
2. Trust in Organised Religion, Military, and Major companies makes you more likely to be a Conservative.
3. Trust in Scientific Community, Press, and Organized labour come in next.
4. Introducing controls for demographic factors changed the model: Race('white' or 'other') and sex were not statistically significant, but confidence in press becamse insignificant. 
5. Trust in press is interesting because it has definitely changed a lot in the past 10 years

![Americans-Trust-in-Mass-Media-1972-2024](https://github.com/user-attachments/assets/45f29efe-7a7f-46fa-b6de-06237aa15bd2)
![Partisans-Trust-in-Mass-Media-1972-2024](https://github.com/user-attachments/assets/f6f5e5f2-9192-4356-ac74-f0a34a892b70)

## Conclusion 

Ideally, in a democracy, everybody, regardless of political leaning would have trust in media. So the fact that having faith in the media is indicative of a DEMOCRATIC political leaning, though unfortunate, makes a lot of sense. 
A 79% accuracy is pretty huge, it's safe to assume that having weak opinions on some of the more indicative variables could get you 'othered' by either side. 

The model definitely highlights a dichotomous difference in values, which, reinforces the idea of polar politics that pervades the world today, so I think if this was done today it might even be more dichotomous than it currently is. 
Not being able to trust certain baseline institutions in a country further drives home the polarization: Not being able to trust the same reality, it means there cannot be a conversation based on a shared understanding of the country they both reside in. 

You should care because if I know this with 10 lines of code, these institutions and the people who want to affect your opinion definitely know this. In this age of technology, your trust in different institutions and lack of in different institutions definitely makes it much easier to know what one can do to affect your opinion on a topic. It's one random forest algorithm away. 



Any implications, surprises, or next steps?

