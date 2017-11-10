## Deploy instructions

#### Staging

- We use [Surge](surge.sh) to host our staging version of the site.

```
(imho) $ yarn # Install surge
(imho) $ surge _site/ imho.surge.sh

    Surge - surge.sh

              email: your-email@gmail.com
              token: *****************
       project path: /Users/you/code/imho/_site/
               size: 37 files, 2.0 MB
             domain: imho.surge.sh
             upload: [====================] 100%, eta: 0.0s
   propagate on CDN: [====================] 100%
               plan: Free
              users: your-email@gmail.com
         IP Address: 45.55.110.124

    Success! Project is published and running at imho.surge.sh
```

#### Production

- Change or add domain CNAME records according to [Surge instructions](http://surge.sh/help/adding-a-custom-domain):

```
Host Name    IP/URL               Record Type
@            na-west1.surge.sh    CNAME
www          na-west1.surge.sh    CNAME
*            na-west1.surge.sh    CNAME
```

If the DNS provider doesn't support CNAME records, alternatively set an A record to the IP `45.55.110.124`.

Deploy to custom domain with surge:

```
(imho) $ surge _site/ imho.press

    Surge - surge.sh

              email: your-email@gmail.com
              token: *****************
       project path: /Users/you/code/imho/_site/
               size: 37 files, 2.0 MB
             domain: imho.surge.sh
             upload: [====================] 100%, eta: 0.0s
   propagate on CDN: [====================] 100%
               plan: Free
              users: your-email@gmail.com
         IP Address: 45.55.110.124

    Success! Project is published and running at imho.surge.sh
```
