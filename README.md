This is a demo project to illustrate a bug introduced with the latest changes to Docusaurs with [PR#1281](https://github.com/facebook/Docusaurus/pull/1281). 
Steps to reproduce the bug
1. Install Node and Yarn
2. Clone this repository
3. Go to DocusaurusBrokenLinks/website
4. Execute yarn run start
5. Go to this url on browser http://localhost:3000/docs/api/api-deploy.html
6. Click on consumption link, it is broken. Ideally, it should lead to http://localhost:3000/docs/api/api-consume.html. But it is broken at the moment.

Basically Consumption.md is present in version 1.0.0 but removed from version next. This causes broken links in version 1.0.0.
Basically, with the changes in PR#1281](https://github.com/facebook/Docusaurus/pull/1281) ,a document that is in version 1.0.0 but removed from next version, will have broken links for that document in version 1.0.0.
