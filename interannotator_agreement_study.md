# Inter annotator Agreement Study

## Inter annotator Agreement score

1. Inter annotator agreement score is calculated using the AnnotationTask package of NLTK
2. Please find the calculated S, pi, kappa and alpha scores below.

```
S score:  0.6856323802832042
Pi score:  0.7078020445822651
Kappa score:  0.5714285714285714
Alpha score:  0.20427287589125628
```

1. We can see that pi score is `70.1`. pi score is calculated when there are more than two coders.
2. S score is `68.6`, which is calculated based on the expected likelihood.
3. alpha score is low because it provides distance function, and it is **based on disagreement instead of agreement**. Assuming all mistakes are equally wrong.

## Results

1. Inter annotator agreement, pi score s around `0.71` which is comparatively very high.
2. As the job description some skills were tagged ambiguously  and those definitely are a reason for a lowered score. 
3. They are many reason like human error, many of us felt libraries like sklearn felt as a tag and some felts it being part of pythin should only be a tag.(some conflicts like this can be a reason for lower score as well)