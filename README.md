# ShodanCLI

Shodan is a search engine for internet-connected devices. It allows users to search for specific types of devices and view detailed information about them. The Shodan command-line interface (CLI) is a tool that allows users to access Shodan's features from the command line. Some common Shodan CLI commands include the following:

##### Shodan CLI - Installation
| Command     |
| :-------------- 
|  $ pip install shodan|
| $ shodan init YOUR_API_KEY|

#### Shodan CLI - Test
| Command     |
| :-------------- 
| $ shodan -h |
|$ shodan info|
|$ shodan myip|
|$ shodan version|

#### Shodan CLI - Use It
| Command     |
| :-------------- 
|$ shodan stats --facets org country:GB ssl.version:sslv2 HTTP|
|$ shodan count port:22 country:gb|
|$ shodan host 8.8.8.8|
|$ shodan stats --facets country|org apache|

#### Shodan CLI - Get to know the network
| Command     |
| :-------------- 
|$ shodan count net:192.168.1.0/24|
|$ shodan stats --facets port net:192.168.1.0/14|
|$ shodan stats --facets vuln net:192.168.1.0/14|
|$ shodan search --fields ip_str,port,org,hostnames net:192.168.1.0/24|

#### Shodan CLI - Get to know the domain
| Command     |
| :-------------- 
|$ shodan domain google.com|

#### Shodan CLI - Get to know the history
| Command     |
| :-------------- 
|$ shodan host --history 8.8.8.8|
