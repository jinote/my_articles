__Meaning of pos_label in f1_score__

__Summary__

The f1 score is the harmonic mean of precision and recall. 
As such, you need to compute precision and recall to compute the f1-score. 
Both these measures are computed in reference to __"true positives(TP)"__ (positive instances assigned a positive label), 
__"false positives(FP)"__ (negative instances assigned a positive label), etc.

The __pos_label parameter__ lets you __specify which class should be considered "positive"__ for the sake of this computation.

More concretely, imagine you're trying to build a classifier that finds some rare events within a large background of uninteresting events. 
In general all you care about is how well you can identify these rare results; the background labels are not otherwise intrinsically interesting. 
In this case you would set pos_label to be your interesting class. 
If you're in a situation where you care about the results of all classes, f1_score is probably not the appropriate metric.



source:
<https://stackoverflow.com/questions/33831869/what-does-pos-label-in-f1-score-really-mean>
