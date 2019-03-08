This is a demo project to illustrate a bug in [Docusaurus 1.7.2](). 
Steps to reproduce the bug
1. Install Node and Yarn
2. Clone this repository
3. Go to DocusaurusBrokenLinks/website
4. Execute yarn run start
5. Go to this url on browser http://localhost:3000/docs/api/api-deploy.html
6. Click on consumption link, it is broken. Ideally, it should lead to http://localhost:3000/docs/api/api-consume.html.
7. Click on overview link, it should lead to overview page within API i.e at http://localhost:3000/docs/api/api-overview.html instead it leads to http://localhost:3000/docs/index.html