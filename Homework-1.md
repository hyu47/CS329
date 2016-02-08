## Information Mapping

The goal of this task is to map information between multiple webpages. Your python program must do the followings:

* Read the [course webpage](http://www.mathcs.emory.edu/classes-semester.php?subject=CS&year=2015&term=2&graduate=0), and save the course information (e.g., [`parse_html.py`](../tree/master/src/regular_expressions/parse_html.py)).
* Read the [exam calendar webpage](http://registrar.emory.edu/Students/Calendars/examcalendar/emorycollege_examcalendar.html) and save the exam information for the current semester.
* When the program is run, it should print the following information:

   ```
   COURSE  SECION   LOCATION             CLASS HOURS  FINAL DATE           FINAL HOURS
   CS130R     000  MSC: W303       M 4:00pm - 4:50pm      28-Apr  11:30 A.M - 2:00 P.M
   ...
   CS329      001  MSC: W201      MW 2:30pm - 3:45pm       3-May   3:00 P.M - 5:30 P.M
   ...
   CS455      000  MSC: W306  TuTh 10:00am - 11:15am       2-May  8:00 A.M - 10:30 A.M
   ```

## Submission

* Write a python program `hw1.py` that satisfies the above condition.
* Put `hw1.py` under the directory `cs329/hw1`.

## Notes

* The information needs to be in a _pretty_ format.
* Some courses have their schedules spread out between lectures and labs (e.g., CS130R). Your program should handle this as well. 