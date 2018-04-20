## Regular Expressions

Find regexes that match the following. (e.g. find a single regex that matches
both `antelope` and `antelopes`.)

* Single regex that matches either of these:

    #### antelope rocks out 
    #### antelopes rock out
    `/antelopes?\srocks?\sout/g`

* Regex that matches either of:
    
   #### goat || moat

  ### but not:

   #### boat
   `/[gm]oat/g`

* Regex that matches dates in YYYY-MM-DD format. (Year can be 1-4 digits, and
  month and day can each be 1-2 digits). This does not need to verify the date
  is correct (e.g 3333-33-33 can match).

  #### 2000-10-12
  #### 1999-1-20
  #### 1999-01-20
  #### 812-2-10

  `/\d{1,4}-\d{1,2}-\d{1,2}/g`

  ## VT-100 Terminal

  * Come up with regexes for the two above sequences. The one to set the
    cursor position should accept any digits for the row and column. The
    bold sequence need only accept `1` (and is a trivial regex). (ESC is
    a single character which can be represented with `\e` in the regex.)

    `/\e\[(1m)?(\d{1,2};\d{1,2}f)?/gi ` 