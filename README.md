# Project-Sneaky-Peanut-Butter
This is a placeholder for a project I recently did called "Project Sneaky Peanut Butter" wherein I gathered 7 kinds of Peanut Butter, A RedBoard (Arduino), and a Spectral Triad Sensor https://learn.sparkfun.com/tutorials/spectral-triad-as7265x-hookup-guide?_ga=2.230455772.1578243289.1643145700-1853259630.1615791300

to gather spectral signatures across 18-channels from peanut butter samples, in an attempt to classify/detect them with a Keras Model


Here is the data https://docs.google.com/spreadsheets/d/e/2PACX-1vQPPhKcY856BgIwGFwJ-4j1riuS4i0fvTWm031K-1UjbLj1BtlFK10A6_sDFYfviR3sma9aR_mONT0_/pubhtml

Not a strictly useful project, but I can run the ML model in real-time with an unknown sample and tell you which style of PB it is :-D 
(If you spend some time exploring the data, a few things stand out...Simply JIF has the highest R channel peak avaerage,  the "shape" of the A, F, R, and W peaks help delineate many out-right)

If I were to put the same model in speech, I'd say:
Is there 3000+ R-channel?


-> YES? It's either Simply JIF, JIF Honey, or Kroger Honey

*     Multiple R values > 3250? = Simply JIF

*     A > F = Kroger Honey

*     A < F = JIF Honey


-> NO?

*      A > F = JIF Omega-3

....the last 2 are the hardest to distinguish, but Reduced Fat JIF has a larger W channel compared to its A and F channels, when compared to Kroger Creamy


NOTES: 1, the organic option, was disqualified on account of oil/foodstuff separation....so, 6 datasets
