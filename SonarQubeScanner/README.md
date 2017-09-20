# TeamCity Plugin - SonarQube Scanner for MSBuild

This is a plugin for Teamcity which brings SonarQube Scanner for MSBuild to Teamcity, and provides you two build steps that makes easy setup *begin* and *end* commands.

## How To Install?

1. Download *sonarqube-scanner-msbuild.zip* file located in build folder.
2. Go to the *Administration* page on TeamCity, and then go to *Plugins List* page.
3. Click on *Upload plugin zip* option and upload the zip downloaded in the first step.
4. Set these parameters on *Root Project* level: sonar.server, sonar.user, sonar.password (spec: password display='normal').

> Note: Once you have uploaded the plugin zip into TeamCity, after a few minutes the plugin (in TeamCity) and the scanner (in Agents) should be ready. If they don’t appear after two minutes, you may need to restart the TeamCity Service / Build Agent service.

## How To Use?

1. Go to the build configuration where you want to setup SonarQube Scanner for MSBuild.
2. Add a new build step.
3. Now, you can able to find two new runner types: *SonarQube Begin Analysis* and *SonarQube End Analysis*.
4. From here on you can follow the official documentation: https://docs.sonarqube.org/display/SCAN/Analyzing+with+SonarQube+Scanner+for+MSBuild
5. Enjoy!

> Note: At this point, we are including the latest version of SonarQube Scanner for MSBuild (3.0.2.656) https://github.com/SonarSource/sonar-scanner-msbuild/releases Feel free to do a pull request if a new version is released.