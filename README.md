# Agent_Based_Modelling

## WHAT IS IT?

An environmental scenario example where factories contaminate the environment, resulting in exposure to a randomly moving population. This contamination spreads (diffuse) at each patch 10% of its contamination.

Because of exposure to contamination, people eventually get sick and finally die.
Also one install a certain number of cleaners that decontiminates the neighboring envirnment of factories. The degree of decontamination depends on clean-rate : stronger clean-rate => greater decontamination

## HOW IT WORKS

At initialization people's number is set to 100 with max health of 50.
They move around being exposed to contamination. At each step their health will decline with 0.01 systematically + a certain degree of exposure to contamination. (depending of the magnitude of contamination: greater contamination leads to greater exposure). A global indicator is set to be the % of high contamination patches vs total patches
More people are exposed, less health they get and finally die if health goes under zero. 

Also people reproduce wich will depend on their health and birth-rate.
As to patches that contain contamination, they can regenerate. Regeneration consists in reducing by itself the  contamination but under some conditions : contamination level not too high (less then 10) , plus it will depend on birth-rate (biger birth-rate, slower will be the regeneration, as more people will consume more ressources)

## HOW TO USE IT

Manually set variables:

NUM-CLEANERS : nb of cleaners 
RANDOM-CLEANER- LOCALIZATION : switch ON/OFF to locate cleaners next to most contaminated factories / or randomly
NUM-FACTORIES: nb of factories
CLEAN-RATE: power of cleaners
BIRTH-RATE: will determine how fast population grow
RESOURCE-REGENERATION: chances to regenerate


## THINGS TO NOTICE

Localization of cleaners : if cleaners are not installed around factories, pollution ends up by reaching high level wich respectively will negatively impact people reproduction.
Also, the proportion of cleaners/ factories impacts a global health and a smoother decline.

Changing the birth-rate will not repercute on overall quality of life (health, pollution), but will maintain an eco-system more sustainable.

Whithout surprise, the decontamination power of cleaner have a positive influence on quality of life but also contributes to keep the eco-system more enduring.

As to regenration rate of ressource, it won't change much in the equilibrum of eco-system, except that health decline is smoother.

## THINGS TO TRY

Try adjusting the parameters under various settings. How sensitive is the stability of the model to the particular parameters? How to find a right balance between nb of people, their level of pollution and level of health. 
