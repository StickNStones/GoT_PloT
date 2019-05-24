This project was inspired by both https://www.reddit.com/r/dataisbeautiful/comments/94kafp/reddit_is_changing_its_mind_about_elon_musk_oc/e3llqsk/
and https://www.reddit.com/r/dataisbeautiful/comments/bmgkfu/oc_the_downfall_of_game_of_thrones_ratings/

Paper on VADER
http://comp.social.gatech.edu/papers/icwsm14.vader.hutto.pdf

The Pushshift API was used to get comments out of each of the 73 discussion threads.

Matplotlib was used to create the visualization.

VADER is used to analyze the text. It uses a lexical feature list as quantitative analysis, and uses rules to analysis the qualitative
sentiment. The authors state that values above 0.05 are positive, and under -0.05 are negative, with inbetween being neutral.

Interestingly the sentiment of Season 5 Episode 6, "Unbowed, Unbent, Unbroken" was the lowest rated episode on IMBD
before season 8, and is also the episode with the lowest sentiment, approaching -0.10. The IMBD score drop is represented in the sentiment.

In contrast, Season 3, episode 9, "The Rains of Castamere" has a 9.9/10 rating on IMBD, while the sentiment score drops. (But not under -0.05)
This is likely due to the episode's content being negative and VADER picking it up. 

The first episode under -.05 is Season 5 Episode 8, "The Mountain and the Viper". This result is most likely due to similar nature of
the last, as the episode has a 9.7 IMBD rating. 