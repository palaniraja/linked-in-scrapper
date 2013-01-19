linked-in-scrapper
==================

All I wanted was their following api to return the values as documented. After so much frustration, I wrote this to scrap the same public info with jquery.

      IN.API.Profile("http://www.linkedin.com/in/aprofileurl")
      .fields("firstName", "lastName", "picture-url", "industry","headline","skills",
      "positions:(company,title,summary,is-current,start-date,end-date)", 
      "group-memberships")
      .result(doMyThing)
      .error(logErrors);
