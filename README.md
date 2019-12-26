# migrate-ngjs-ng8-in-iis
A migration pattern for angular ngjs to ng8 deployed in iis.
The existing application is AngularJS + .NET api deployed in IIS.
One way to slowly migrate to a newer (2+) version of angular is to have them both exist side-by-side and migrate features from AngJS to Ang2+.

# This repo has 3 applications
- Angular 8
- AngularJS
- .NET API

# Deployment
1. Deploy .NET API using vs publish to IIS.
2. Copy AngularJS files to IIS root inside a folder named "AngJS".
3. Copy Angular 8 dist files to the root iis folder.

# Browse
http://localhost:port/Index.html - Loads the angular 8 project
http://localhost:port/AngJS/Index2.html - Loads the angularjs project (fetches data from api endpoint api/values)
http://localhost:port/api/values - Gets data from API.

