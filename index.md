Hands-on exercies for the Animal Science and Ethics Day in Bern. 

Estimate the required sample size using [this web app](http://powerandsamplesize.com/).

A trial will be conducted to study the reaction time in young swiss male subjects. The experimental setting aims at studying the fasting condition versus post-prandial condition. The outcome variable of interest is the reaction time in milli seconds [ms]. Some preliminary studies show that reaction time for fasting is about 100 [ms] with a standard deviation of 30 [ms]. The expected change after a meal is an increease of 30 % in reaction time. The study design is a two group superiority trial. The study has a balanced designed. The test will be perform conservativelly with two tails and in an unpair setting. We will use the classical levels of power and alpha (80% and 5% respectivelly.)


# 1. Estimate the require sample size for a parametric approach

power.t.test(delta = 30,sd = 30,sig.level = .05,power = .8,type = "two.sample",alternative = "two.sided")

# 2. Estimate the new required sample size if SD is reduced by 20%

power.t.test(delta = 30,sd = 24,sig.level = .05,power = .8,type = "two.sample",alternative = "two.sided")

# 3. Estimate the new sample size is the SD is 30 [ms] but the expected change is an increase of 36 [ms]

power.t.test(delta = 36,sd = 30,sig.level = .05,power = .8,type = "two.sample",alternative = "two.sided")

# 4. Estimate the new sample size if you decide to use a paire designed

power.t.test(delta = 30,sd = 30,sig.level = .05,power = .8,type = "paired",alternative = "two.sided")

# 5. Estimate the power achieved with 10 subject per group in an unpair design
