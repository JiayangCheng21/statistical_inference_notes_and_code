Three paths to get to the truth using stats?

- Path of action:
    - Search for rules to govern behavior
    - Use P-value and alpha level —> accept or reject
    - we can’t know whether we are right or wrong in the current test, but we will not be wrong too often over a large number of tests.
- Path of knowledge:
    - Compare the likelihood of different hypo, given the data
- Path of belief
    - Have a prior belief, data don’t really change it.
    - This is Bayesian statistics: express evidence in terms of ‘degrees of belief’
- Not either or! You can combine the approaches (Frequentist & Bayesian)


What is P-value? 

- Tell you how **surprising** the data is, **assuming there is no effect**
    - Definition: The probability of getting the **observed or more extreme data**, assuming **null hypothesis is true**
    - * A p-value is the probability of the **data**, **not** the **theory**
        - P-value < 0.05  ≠ effect 95% likely to be true
        - P(Data* | Hypo) (p value)  ≠ P(Hypo | Data)
        - P-value > 0.05 does not mean there is not a true effect. You need larger samples to detect small effect.
- How to use: use it to guide behavior in the long run
    - P < alpha: act if data is not noise
    - P > alpha: remain uncertain or as if the data is noise
    
    
What are Type 1 and 2 error?

- Alpha: probability of a signifiant result when H0 is true (Type 1 error rate)
- Beta: probability of a non-significant result, given that H1 is true (Type 2 error rate)
    - 1-Beta: the probability of a significant result when H1 is true (statistical power)
- Error rates are frequentist concepts: they are about the long run
    - For each case, you either make a mistake or you don’t, the rate applies to the long term
- The error rate should be set based on the specific goals and available resources


What is Lindley’s paradox. When P-value close to 0.05 (eg, 0.045), what does it mean?
- A result can be unlikely when the null hypothesis is true, but it can be even more unlikely assuming the alternative hypothesis is true, and power is very high
    - some researchers have suggested using lower alpha levels in very large sample sizes, and this is probably sensible advice. Other researchers have suggested using Bayesian statistics (which we will encounter in assignment 2.2), which is also sensible advice
- In our simulations, we know there is a true effect or not, but in the real world, you don’t know. When you have very high power, use an alpha level of 0.05, and find a p-value of p= .045, the data is surprising, assuming the null hypothesis is true, but it is even **more surprising**, assuming the alternative hypothesis is true. This shows how a significant pvalue is **not always evidence for the alternative hypothesis.**
