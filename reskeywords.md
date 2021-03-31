---
layout: page
title: Keywords in Context
#subtitle: 
---

### Method Overview

Keywords in Context is a very straightforward form of text analysis. I used Python to locate each instance of a word in the texts, and then pull out that word with approximately 30 characters on either side. This process provides a glimpse of how the word is being used within the text.

### Review of Data

This was the most instantly successful analysis method of the three I used.  While it doesn't produce any "data" exactly, what it did was give me an overview of the context surrounding my search term. This in turn let me identify articles in the journal worth reading closely. While it's possible to do this with a key search in the PDFs on Hathitrust (which is how I then proceeded to find the journal articles once I identified ones I wanted to see via this process), it is much more efficient to do it with Python, which can search every issue within just a few minutes. It turns out 30 characters on either side of a word really is enough to get the gist of how the word is being used.
 
#### Safety
The word "safety" is used in a few different contexts within *Stone*. One common context is in reference to the safety of the stone material itself: how to blast it into large chunks, transport it, and store it without damage. Safety factors and safety margins are also used quite frequently in some of the articles related to engineering. As discussed above, safety often appears in the 1910s in reference to concrete, a material that was competing with stone for use both paving and building work. Many articles in this period, such as this quote from an article titled "Deaths and Injuries in Concrete Collapses" from the December 1912 issue demand tighter regulations on concrete in the interest of public safety:
 
>The record of concrete disasters during the past month is no less imposing and shocking than usual. If this country were not more careless about human life than any other civilized government, the terrible accidents that constantly follow the use of this treacherous material would lead to such stringent regulations that public safety would be conserved. Here we express great indignation, promise a searching investigation, and then forget all about the matter until a new disaster occurs.[1]
 
As can be seen in the example above, hazard-related words such as "injuries," accidents," and "disaster" also frequently appear during this time period in reference to concrete.
 
Articles pulled up through keyword in context analysis show that discussions of workplace safety do appear throughout the journal, particularly around the use of explosives in quarry work. There is also a great deal of discussion around safety issues in steam-powered equipment in the 1890s and early 1900s. After 1910 safety frequently appears as part of the phrase "Safety First," a slogan frequently used by safety advocates in the Progressive Era who focused on safety improvements to mechanical equipment and worker safety education that became a generic slogan for safety initiatives nationwide.[2]
 
Through close reading of articles flagged during my review of the keyword in context data I was indeed able to see that there are changes in the language used over time in articles about workplace safety. For instance, in an article titled "Risks in Quarrying" from the November 1897 issues blames workplace accidents on careless employees. For example, when the article discusses explosives:
 
>If there is anything to be feared in quarrying operations it might be supposed to be blasting; but there is a class of men – and we imagine, hardly a quarry is without representatives of them – who are so foolhardy in dealing with powder as to appear irrational. They cannot be convinced that the force in powder may be latent. If it will not "go off" they imagine it can be tamped with impunity, and it does not always happen that they are made cautious by an accident.[3]
 
The article ends by stating that safety regulations are unnecessary and potentially dangerous to business with an interestingly gendered comparison:
 
>If operations in quarries were carried out by little girls, it would be prudent to watch over them; but as with men there are few risks, we can only consider the recommendations as exemplifying Lord Melbourne's apprehensions about the danger of a policy which insisted on "something being done" at any cost.[4]
 
Other articles call for more safety at the quarry, including this editorial titled "Criminal Accidents" from the March 1889 issue which bemoans the lack of safety measures for workers overall, and particularly in quarries, in the United States:
 
>We say that it is the apathy with which a thing of this kind is received that is the most discouraging feature of the whole business. Slap a man in the face and you are fined for it in the police court; slap a man's head off with a carelessly contrived piece of machinery, or kill him in a building and you get the sympathy of the people for having had such an accident occur on the premises. This is a large world and the more we look at it the more it swells.[5]
 
For comparison the article "Precautions Against Quarry Accidents" from the August 1914 issue of *Stone* ends with the following statement:
 
>Every quarry has its own individual problems that must be studied with the greatest care and attention if accidents are to be reduced to the lowest possible minimum. Even the straight hoisting of a heavy block from the quarry pit may entail disaster. The slipping of a chain or sling may bring a sudden strain on a derrick which it is unable to withstand. Even the most rigid scrutiny of apparatus cannot forestall all disaster. In such cases dependence must be placed upon wise and careful management. Stringent regulations that will keep workmen out of the danger zones as much as possible, may seem costly precautions for the moment, but they will pay in the long run.[6]
 
The majority of articles in the later half of the digitized issues focus more on how to provide safety than in trying to assign blame as seen in the earlier issues. Many of the articles directly relate this greater awareness of safety to workmen's compensation laws, for instance "Causes of Quarry Accidents" from October 1915 states:
 
>The enactment of compensation laws in this country makes the study of industrial accidents of great importance. Apart from all questions of humanity, it is essential, on the mere basis of dollars and cents, that every precaution be taken to guard the safety of the working men.[7]
 
This change around the language of safety can be seen in the journal beyond articles that discuss safety directly, particularly in accident reporting and advertisements. "Notes from Quarry and Shop," the section in early issues of *Stone* devoted to miscellaneous news items, are filled with small reports of unusual accidents and reports on the outcomes of litigation of cases where widows and injured men sued employers for negligence. These "unusual" accident reports for the most part disappear by 1912 and are replaced by tables of statistics on all accidents within the industry as compiled in reports by the U.S. Bureau of Mines and the Bureau of Labor Statistics. Articles discussing specific accidents in the late 1910s and 1920s primarily focus on analyzing what went wrong and how to prevent similar accidents from occurring in the future. Advertisements also increasingly tout the safety features of their products from the 1910s-1920s. For example, this 1917 advertisement for DuPont Blasting Machines uses the "Safety-First" slogan and notes its product can "safeguard life and property." This advertisement for DuPont Blasting Machines that uses the "Safety-First" slogan[8] is only one of many that uses safety vocabulary in later issues.

![image](/assets/img/dupontblastingmachine.png)

#### Health and Environment

 I had fewer results overall for words related to health and environment keywords in the journal issues than I did for safety keywords. The fact that the digitized issues of the journal only go up to 1922 means that the major period of silicosis discussion (the early 1930s) is not represented. In fact the word "silicosis" never appears in the pages of the journal. However, dust inhalation appears to have always been recognized as a significant stone industry hazard in the quarry industry. Articles from the 1880s and 1890s reference "stone consumption," "miner's consumption" and "phthisis," varying terms used to refer to silicosis before silicosis itself entered general use around 1917.[9] An article in "Notes on Quarrying," from the March 1890 issue states:
 
>Hand channeling in sandstone should be prohibited by law for the sake of humanity. It is sure death to the operator, owing to the inhaling of the dust-grit which settles in the lungs, producing what is called "stone consumption," a disease which kills its victim in about seven years from its inception.[10]

"Risks in Quarrying" from the November 1897 issue also notes the health hazard of dust inhalation, but finds it an inevitable byproduct of modernization:

>It will be said that the death rate among quarriers is about 12 per cent. higher than the mortality of "all males'' in this country, and that circumstance is proof of the existence of evils which are probably remediable. Again, quarriers are much above average in mortality from phthisis and diseases of the respiratory organs, being nearly three times in excess of fishermen. … according to Dr. Ogle, the late superintendent of statistics, "the mortality figures tend to show that the quarriers are a set of strong men, who live a healthy life, with the exception of the inhalation of dust and the liability to accident."  If the conclusion be correct it is much to be regretted; but it is hard to see how government officers could prevent the inhalation of minute particles of stone or compel them from operating injuriously on the respiratory organs. The use of respirators or the practice of breathing through the nose might diminish the evil, and quarriers could make the experiment without compulsion. Science may some day discover other means of preserving men against the consequences of following dangerous trades, but unless we go back to the savage or golden age we must put up with them. Every application of material in manufactures brings misery with it.[11]
 
Conflicts around health between employers and employees appear frequently in the pages of *Stone* between 1909-1922, particularly around the use of pneumatic (air-driven) tools which increased dust levels, particularly in stone finishing sheds. These tools in the form of drills, chisels, planers, and jackhammers began to appear in quarry work in the mid-1890s, and became increasingly common throughout the early 1900s.[12] In 1909 there was a major strike by granite workers in Barre, Vermont around using dust-producing pneumatic tools in enclosed sheds. *Stone* covered this conflict in several articles, including "Cost of the Barre Strike'' in the March 1910 issue. Other journal issues cover additional conflicts around pneumatic tools between labor and employers through the 1920s. For instance "The Air Hammer and Health" in the May 1918 issue presents findings from a U.S. Public Health Service report that investigated whether jackhammers cause numbness and paralysis in workers. *Stone* was anxious to report that the Public Health Service stated that there was no negative effect for air hammer use, but the conflict kept appearing in the pages of the magazine throughout the 1920s. 
 
My environmental keywords did not provide many results. However, results for "smoke" and "dust" were illuminating. *Stone* devoted a lot of space to discussion of air pollution within its pages, not primarily as a health hazard (although its health effects were noted), but because of its effect as a major threat to the beauty of stone as a cladding for buildings. The sheer numbers of articles about stone cleaning procedures that reference the dirty air and soot-encrusted buildings of twentieth-century America are a fascinating way of conceptualizing urban air quality in an era that saw an enormous increase in air pollution due to increased use of coal in industry.[13] For instance, this article from the October 1899 issue titled "Color and Decay of Stone" describes the following:
 
>A white limestone or marble structure erected in the midst of the business portion of a large city, soon loses its original color, becoming gray and dingy from the smoke and dirt that fills the air. If the limestone is bituminous and contains a small amount of oil, it will be certain to collect all the dust and smoke which chances to fall upon it. In the suburban and residence parts of the city and in the rural districts, where both smoke and dust have little effect, the original color will not suffer so much from external causes alone. In the business section of our large cities, the walls of all the buildings become so begrimed with smoke and dust that it is barely possible to tell which were originally constructed out of light and which out of dark colored stone. One has to familiarize himself with the different shades of brown and gray, characteristic of different colored stones, after they have been steeped in a smoke and dust laden atmosphere, in order to be able to determine their original color.[14]
 
Another example is this miscellaneous news item from the August 1916 issue:
 
>Workmen are now engaged in cleaning the magnificent new postoffice at Denver, built of Colorado marble and completed only a year ago. It is said that the air of Denver is so impregnated with smoke that the stone becomes begrimed almost as soon as the cleaning is completed.[15]
 
*Stone* also discusses environmental issues in the context of scenic beauty vs. industrialization. For instance, an article from the September 1903 issue titled "The Warfare Against Quarries" summarizes the conflict:
 
>But when the stone man started his business, he may have avoided the cities and settlements and gone far into the wilds. Perhaps he establishes himself at the foot of some bold cliff or on a solitary hill. Presently along will come some poetic soul and bewail the fact that mercenary men are defacing a beautiful landscape.[16]
 
Articles about the battle over quarrying of the Palisades in New York/New Jersey follow this pattern, with *Stone* typically on the side of the quarryman.

### Conclusions and Areas for Further Research

I found the Keywords in Context method particularly successful in how it located articles for close reading so efficiently. After reading the articles pulled up by the analysis, I have several additional avenues of research I'd like to pursue. Interestingly some of the early language around safety (when safety is considered the responsibility of the individual workman rather than management) is gendered – for example the 1897 article quoted above where safety is something necessary only for "little girls." In addition, many early articles calling for greater safety measures draw attention to the desperate widows and children the injured workers can no longer support as a reason greater safety is required. I'd be interested in locating gender-related keywords in the text to see if there is a pattern in how they are being used and if this changes over time. I also have a few stone companies and products I want to do some additional research on and this method will make finding relevant articles very straightforward.

### Footnotes

[1]“Deaths and Injuries in Concrete Collapses,” *Stone* 33, No. 12 (December 1912), 644.

[2] Dianne Bennett and William Graebner, "Safety First: Slogan and Symbol of the Industrial Safety Movement," *Journal of the Illinois State Historical Society* 68, no. 3 ( June 1975), 254.

[3] “Risks in Quarrying,” *Stone* 15, No. 4 (November 1897), 573.

[4] Ibid, 577.

[5] “Criminal Accidents,” *Stone* 1, No. 11 (March 1889), 274.

[6] “Precautions Against Quarry Accidents,” *Stone* 35, No. 8 (August 1914), 414.

[7] “Causes of Quarry Accidents,” *Stone* 36, No. 10 (October 1915), 538.

[8] Image Source: [*Stone* 38 (April 1917)](https://babel.hathitrust.org/cgi/pt?id=nyp.33433069065880&view=1up&seq=5), 219.

[9] David Rosner and Gerald E. Markowitz, *Deadly Dust: Silicosis and the Politics of Occupational Disease in Twentieth-Century America* (Princeton, NJ: Princeton University Press, 1991), 31.

[10] Notes on Quarrying,” *Stone* 2, No. 11 (March 1890), 214-215.

[11] “Risks in Quarrying,” *Stone* 15, No. 4 (November 1897), 576.

[12] David Seager, "Barre, Vermont Granite Workers and the Struggle Against Silicosis, 1890-1960." *Labor History* 42, no. 1 (2001), 66. 

[13]  Stephen Mosely, "Environmental History of Air Pollution and Protection," in *The Basic Environmental History: Environmental History, vol 4* ed. Mauro Agnoletti and Simone Neri Serneri (Springer, 2014), 148.

[14] “Color and Decay of Stone,” *Stone* 19, No. 5 (October 1899), 429. 

[15] "Notes from the Stone Field," "*Stone* 37, No. 8 (August 1916), 431.

[16] “The Warfare Against Quarries,” *Stone* 26, No. 5 (September 1903), 457.



