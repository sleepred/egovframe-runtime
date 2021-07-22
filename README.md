[![Englsh][language-en-shield]](README.md) 
[![Korean][language-kr-shield]](README.kr.md)


![image](https://user-images.githubusercontent.com/1613812/125195363-365a7d00-e290-11eb-92b5-6cfd5266962e.png)


[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]


<!-- ABOUT THE PROJECT -->
# eGovFrame Runtime

eGovernment Standard Framework - Runtime Environment

## Description

Common modules necessary for the execution of business logic programs in eGovernment project. Application programming environment to facilitate the standardized development of screens, server programs and data.

<!-- GETTING STARTED -->
## Getting Started

eGovFrame Runtime uses the Maven framework. 

### Prerequisites

* Maven, version 3+
* Java JDK 1.7+

### How to build

#### Building it

This is a Maven project, and to build it use the following command:

```
$ mvn clean install
```
Optionally you can specify -Drelease to trigger obfuscation and/or uglification (as needed)

Optionally you can specify -Dmaven.test.skip=true to skip the tests (even though
you shouldn't as you know)

The build result will be a eGovFrame Runtime package located in ```target```.

#### Packaging / Distributing it

Packages can be built by using the following command:
```
$ mvn clean package
```

The packaged results will be in the `target/` sub-folders of `assemblies/*`.

#### Running the tests

__Unit tests__

This will run all unit tests in the project (and sub-modules). To run integration tests as well, see Integration Tests below.

```
$ mvn test
```

<!-- USAGE EXAMPLES -->
### Usage

eGovFrame Runtime can be downloaded using maven through the following settings in pom.xml file.

#### Using dependency definitions. 

Define parent project in pom file

After adding above, add the following dependency definitions. 
(Only the required ones.)

``` xml

<properties>
    <spring.maven.artifact.version>5.2.5.RELEASE</spring.maven.artifact.version>
    <org.egovframe.rte.version>4.0.0</org.egovframe.rte.version>
</properties>

...

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.cmmn</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.ptl.mvc</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.psl.dataaccess</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.logging</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<!-- OPTIONAL -->
<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.idgnr</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

<!-- OPTIONAL -->
<dependency>
    <groupId>egovframework.rte</groupId>
    <artifactId>egovframework.rte.fdl.property</artifactId>
    <version>${egovframework.rte.version}</version>
</dependency>

...

```

## Version History

* 4.0.0 beta
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 4.0.0 alpha
    * Initial Release

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b eGovFramework/egovframe-runtime`)
3. Commit your Changes (`git commit -m 'Add some egovframe-runtime'`)
4. Push to the Branch (`git push origin eGovFramework/egovframe-runtime`)
5. Open a Pull Request

## Asking for help

Please go to https://www.egovframe.go.kr/home/sub.do?menuNo=69 to ask questions and get help.

```
command to run if program contains helper info
```

<!-- LICENSE -->
## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
The eGovFrame Framework is released under version 2.0 of the [Apache License](https://www.apache.org/licenses/LICENSE-2.0).

## Contact

Contributors names and contact info

ex. Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com
ex. Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[language-kr-shield]: https://img.shields.io/badge/language-Korean-blue.svg?style=for-the-badge
[language-en-shield]: https://img.shields.io/badge/language-English-red.svg?style=for-the-badge

[contributors-shield]: https://img.shields.io/github/contributors/sleepred/Good-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/sleepred/Good-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/sleepred/Good-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/sleepred/Good-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/sleepred/Good-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/sleepred/Good-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/sleepred/Good-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/sleepred/Good-README-Template/issues
[license-shield]: https://img.shields.io/github/license/sleepred/Good-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/sleepred/Good-README-Template/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png



