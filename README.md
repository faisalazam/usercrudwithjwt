[![Parent CI/CD][parent-cicd-badge-url]][parent-cicd-link-url]
[![pages-build-deployment][pages-build-deployment-badge-url]][pages-build-deployment-link-url]
[![Instructions Coverage][instructions-coverage-badge-url]][instructions-coverage-link-url]
[![Branches Coverage][branches-coverage-badge-url]][branches-coverage-link-url]
[![checkstyle][checkstyle-badge-url]][checkstyle-link-url]
![Known Vulnerabilities][known-vulnerabilities-badge-url]
[![Apache License, Version 2.0, January 2004][apache-license-badge-url]][apache-license-link-url]


<h1 style="text-align:center">
  Maven, Plugins, GitHub Pages, and GitHub Workflows/Actions ![Awesome](https://github.com/faisalazam/MavenInActionWithGitHubActions/raw/master/.github/assets/awesome-badge.svg)
</h1>

<p>
    <a href="https://faisalazam.github.io/MavenInActionWithGitHubActions">This project</a> 
    will automatically be deployed to <a href="https://pages.github.com/">GitHub Pages</a> 
    with <a href="https://github.com/features/actions">GitHub Actions</a> by going through the following steps:
</p>
<p>
    <a href="https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/putting-all-together.yml">
        <img src="https://github.com/faisalazam/MavenInActionWithGitHubActions/raw/master/.github/assets/putting-all-together.png" alt="" />
    </a>
</p>

## Inspiration
<p>
    While working on a personal project, felt a need to develop and share a template maven project solving 
    the basic problems. Some of them are included below which led to a series of small projects in this repo:
</p>
<ul>
    <li>Running all tests</li>
    <li>Running single test, class, package etc.</li>
    <li>Running unit and integration tests separately</li>
    <li>Code coverage for unit and integration tests separately</li>
    <li>Combined code coverage for unit and integration tests</li>
    <li>Other checks like checkstyle, PMD, etc.</li>
    <li>Project Site generation for single module setup</li>
    <li>Project Site generation for multi module setup</li>
    <li>Automated deployment to GitHub Pages using GitHub Workflows and Actions</li>
</ul>

## Modules
Following are the submodules of this [parent project][parent-project-url]:

| Module                                         | Status                                                                                                                                                                                      |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [SiteGeneration][site-generation-url]          | [![Site CI/CD][site-cicd-badge-url]][site-cicd-link-url] [![pages-build-deployment][pages-build-deployment-badge-url]][pages-build-deployment-link-url]                                     |
| [TestsExecution][tests-execution-url]          |                                                                                                                                                                                             |
| [JacocoExecution][jacoco-execution-url]        |                                                                                                                                                                                             |
| [PuttingAllTogether][putting-all-together-url] | [![PuttingAllTogether CI/CD][putting-all-together-badge-url]][putting-all-together-link-url] [![pages-build-deployment][pages-build-deployment-badge-url]][pages-build-deployment-link-url] |

Every next submodule is built on top of the previous submodule. For exampple, [TestsExecution][tests-execution-url] is 
built on top of [SiteGeneration][site-generation-url].

Contributing
------------

We accept Pull Requests via GitHub. Comments on the PRs is the main channel of communication for contributors.
There are some guidelines which will make applying PRs easier for us:
+ No tabs! Please use spaces for indentation.
+ Respect the code style.
+ Create minimal diffs - disable on save actions like reformat source code or organize imports. If you feel the source code should be reformatted create a separate PR for this change.
+ Provide [JUnit tests][junit-url] for your changes and ensure that your changes don't break any existing tests by running:
    + ```mvn clean test verify```
+ You can check whether there are currently broken tests at the [Continuous Integration][parent-cicd-link-url] page.

If you plan to contribute on a regular basis, please consider filing a [contributor license agreement][contributor-license-agreement-url].
You can learn more about contributing via GitHub in our [contribution guidelines](CONTRIBUTING.md).

License
-------
This code is under the [Apache Licence v2][apache-license-link-url].

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[parent-cicd-badge-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/parent-build.yml/badge.svg
[parent-cicd-link-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/parent-build.yml
[pages-build-deployment-badge-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/pages/pages-build-deployment/badge.svg
[pages-build-deployment-link-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/pages/pages-build-deployment
[instructions-coverage-badge-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/jacoco-merged/jacoco-resources/badges/jacoco.svg
[instructions-coverage-link-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/jacoco-merged/index.html
[branches-coverage-badge-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/jacoco-merged/jacoco-resources/badges/branches.svg
[branches-coverage-link-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/jacoco-merged/index.html
[checkstyle-badge-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/badges/checkstyle-result.svg
[checkstyle-link-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/INDIVIDUAL_MODULES/PuttingAllTogether/checkstyle.html
[known-vulnerabilities-badge-url]:https://snyk.io/test/github/faisalazam/maveninactionwithgithubactions/badge.svg
[apache-license-badge-url]:https://img.shields.io/github/license/apache/maven.svg?label=License
[apache-license-link-url]:https://www.apache.org/licenses/LICENSE-2.0
[site-cicd-badge-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/site-generation.yml/badge.svg
[site-cicd-link-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/site-generation.yml
[putting-all-together-badge-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/putting-all-together.yml/badge.svg
[putting-all-together-link-url]:https://github.com/faisalazam/MavenInActionWithGitHubActions/actions/workflows/putting-all-together.yml
[parent-project-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/staging/index.html
[site-generation-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/staging/SiteGeneration/sitegeneration/index.html
[tests-execution-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/staging/TestsExecution/testsexecution/index.html
[jacoco-execution-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/staging/JacocoExecution/jacocoexecution/index.html
[putting-all-together-url]:https://faisalazam.github.io/MavenInActionWithGitHubActions/staging/PuttingAllTogether/puttingalltogether/index.html
[junit-url]:https://junit.org/junit5/docs/current/user-guide
[contributor-license-agreement-url]:https://www.apache.org/licenses/#clas