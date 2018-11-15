# SecurityWeek9

# Project 9 - Honeypot
In this project, we had to create a honeypot server, which according to [Tech Target](http://searchsecurity.techtarget.com/definition/honey-pot) is a computer system that is set up to act as a decoy to lure cyberattackers, and to detect, deflect or study attempts to gain unauthorized access to information systems.


## Honeypot 1: Dionaea with HTTP
### Summary
Dionaea is a honeypot whose intention is to trap malwares that are exploiting vulnerabilities exposed by services offered to the network with the ultimate goal of gaining a copy of the attacking malware.

![](/honeypot.gif?raw=true)

At the moment of the writing of this document, the MHN server has recorded **2023** attacks for the day to the `dionaea` honeypot. The following tables show the breakdowns based on the origin of the attack and port attacked.

Table 1: Rank of Attacks based on the Origin IP

| Rank |    IP Address   | Origin         | # of Attacks |
|:----:|:---------------:|:--------------:|:------------:|
| 1    |72.226.28.47     | USA            | 516          |
| 2    |107.155.185.36   | USA            | 93           |
| 3    |158.69.241.18    | Canada         | 59           |
| 4    |195.154.181.191  | France         | 55           |
| 5    |51.15.190.16     | United Kingdom | 40           |


Table 2: Rank of Attacks based on the Attacked Port 

| Rank | Port # | # of Attacks |
|:----:|:------:|:------------:|
|   1  |  5060  |      337     |
|   2  |   23   |      287     |
|   3  |   445  |      115     |
|   4  |   443  |      102     |
|   5  |  1433  |      57      |


Unfortunately, the MHN Admin Server was not able to discern _**any**_ attack signature. 

**JSON Export** of this honeypot can be found [over here](/dionaea.json) at the `assets` directory of this repository.

### Issues
It was a confusing and exasperating experience to set up Google Cloud Platform (GCP) project and VMs for this project.

### Unresolved Questions
The following nagging questions popped up to the top my head during this project:
- How do these developers developed these different honeypots? What are the _minimum_ requirements to create one or at least to understand more of its mode of actions?


## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

