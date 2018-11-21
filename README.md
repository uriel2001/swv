# Tool-chain for Software Visualization

One Paragraph of project description goes here

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
CentOS 7 이상
```

### Installing

1. SWV 환경 구축을 위한 기본 디렉터리 생성
   - 여섯 개의 디렉터리를 생성
```
# mkdir /usr/local/SWV
# mkdir /usr/local/SWV/dev
# mkdir /usr/local/SWV/tools
# mkdir /usr/local/SWV/server
# mkdir /usr/local/SWV/src
# mkdir /usr/local/SWV/toolchain
```
2. Apache HTTP 서버 설치
   - yum을 이용해 관련된 유틸리티 설치
```
# yum -y install gcc make gcc-c++ pcre-devel httpd-devel apr-devel apr-util-devel
# yum -y install expat-devel
```
   - wget을 이용해 관련된 유틸리티 다운로드 및 설치
```
# cd /usr/local/SWV/server
# wget http://archive.apache.org/dist/httpd/httpd-2.4.29.tar.gz
# wget http://mirror.apache-kr.org/apr/apr-1.6.5.tar.gz
# wget http://mirror.apache-kr.org/apr/apr-util-1.6.1.tar.gz
# wget http://downloads.sourceforge.net/project/pcre/pcre/8.41/pcre-8.41.tar.gz
# tar -xvzf httpd-2.4.29.tar.gz
# tar -xzvf apr-1.6.5.tar.gz
# tar -xzvf apr-util-1.6.1.tar.gz
# tar -xzvf pcre-8.41.tar.gz
# mv apr-1.6.5 ./httpd-2.4.29/srclib/apr
# mv apr-util-1.6.1 ./httpd-2.4.29/srclib/apr-util
# cd pcre-8.41
# ./configure
# make
# make install
```




And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

