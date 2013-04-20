linked-in-scrapper
==================

###Demo

[Click here](http://htmlpreview.github.io/?https://github.com/palaniraja/linked-in-scrapper/blob/master/index.html) to see the demo. 

_**Note:** You need to be signed out of LinkedIn._

###Why?

All I wanted was their following api to return the values as documented. After so much of frustration, I wrote this to scrap the same public info with jquery.

      IN.API.Profile("http://www.linkedin.com/in/aprofileurl")
      .fields("firstName", "lastName", "picture-url", "industry","headline","skills",
      "positions:(company,title,summary,is-current,start-date,end-date)", 
      "group-memberships")
      .result(doMyThing)
      .error(logErrors);


###Credits

Thanks to [learningjquery](http://www.learningjquery.com/2009/04/better-stronger-safer-jquerify-bookmarklet)for _Step 1: jQuerify_ bookmarklet