# Elegant-simple-array-input-from-a-flatfile-by-Novinosrin
Elegant simple array input from a flatfile by Novinosrin

    Elegant simple array input from a flatfile by Novinosrin

    I did not know that

    github
    https://tinyurl.com/y94wfhtn
    https://github.com/rogerjdeangelis/Elegant-simple-array-input-from-a-flatfile-by-Novinosrin

    SAS Forum
    https://tinyurl.com/ycf6l29w
    https://communities.sas.com/t5/SAS-Procedures/Counting-gt-0-in-observation-across-variables/m-p/528142

    Novinosrin profile
    https://communities.sas.com/t5/user/viewprofilepage/user-id/138205

    data have;

    array months(6);
    input months(*);

    cards4;
    0 4 3 7 6 8
    3 7 5 0 5 0
    6 8 6 2 8 0
    4 7 0 7 9 4
    5 8 6 0 5 7
    ;;;;
    run;quit;


     WORK.HAVE total obs=5

      MONTHS1    MONTHS2    MONTHS3    MONTHS4    MONTHS5    MONTHS6

         0          4          3          7          6          8
         3          7          5          0          5          0
         6          8          6          2          8          0
         4          7          0          7          9          4
         5          8          6          0          5          7

    * this does not work;
    data have;

    array months(6);
    input months:;

    cards4;
    0 4 3 7 6 8
    3 7 5 0 5 0
    6 8 6 2 8 0
    4 7 0 7 9 4
    5 8 6 0 5 7
    ;;;;
    run;quit;

