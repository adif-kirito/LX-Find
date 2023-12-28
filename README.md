# Finding your way aroud linux

One Paragraph of project description goes here

<!-- ----------------------------------------------- -->
## Find files based on filename

```
find [directory path] -type f -name [filename]
```

Example: find /home/Andy -type f -name sales.txt <br><br>

<!-- ----------------------------------------------- -->
## Find Directory based on directory name

```
find [directory path] -type d -name [filename]
```

Example: find /home/Andy -type d -name pictures <br><br>

<!-- ----------------------------------------------- -->
## Find files based on size

```
find [directory path] -type f -size [size]
```

Example: find /home/Andy -type f -size 10c <br>
*(c for bytes, k for kilobytes, M megabytes, G for gigabytes)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on username

```
find [directory path] -type f -user [username]
```

Example: find /etc/server -type f -user john <br><br>

<!-- ----------------------------------------------- -->
## Find files based on group name

```
find [directory path] -type f -group [group name]
```

Example: find /etc/server -type f -group teamstar <br><br>

<!-- ----------------------------------------------- -->
## Find files modified after a specific date

```
find [directory path] -type f -newermt '[date and time]'
```

Example: find / -type f -newermt '6/30/2020 0:00:00' <br>
*(all dates/times after 6/30/2020 0:00:00 will be considered a condition to look for)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on date modified

```
find [directory path] -type f -newermt [start date range] ! -newermt [end date range]
```

Example: find / -type f -newermt 2013-09-12 ! -newermt 2013-09-14 <br>
*(all dates before 2013-09-12 will be excluded; all dates after 2013-09-14 will be excluded, therefore this only leaves 2013-09-13 as the date to look for.)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on date accessed

```
find [directory path] -type f -newerat [start date range] ! -newerat [end date range]
```

Example: find / -type f -newerat 2017-09-12 ! -newerat 2017-09-14 <br>
*(all dates before 2017-09-12 will be excluded; all dates after 2017-09-14 will be excluded, therefore this only leaves 2017-09-13 as the date to look for.)* <br><br>

<!-- ----------------------------------------------- -->
## Find files with a specific keyword

```
grep -iRl [directory path/keyword]
```

Example: grep -iRl '/folderA/flag' <br><br>

<!-- ----------------------------------------------- -->
## Filter your results to exclude files/directories that you do not have permission to

```
2>/dev/null
```

<br><br>

<!-- ----------------------------------------------- -->
## Find Manual

```
man find
```

<br><br>


delete when done
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
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

* TryHackMe - Linux Strength Training(https://tryhackme.com/room/linuxstrengthtraining)
* Inspiration
* etc
