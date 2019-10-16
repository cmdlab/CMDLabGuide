
**Update**: 08/23/2019

**Maintained By**: Arunima K. Singh

**Email**: arunimasingh@asu.edu  

# Table of contents
1. [About Our Group](#section1)
2. [After You Join the Group](#section2)
3. [Our Computing Resources](#section3)
    1. [ASU Supercomputing](#section3.1)
    2. [XSEDE Supercomputing](#section3.2)
4. [Setting Up a New Computer](#section4) 
    1. [Windows](#section4.1)
    2. [Mac](#section4.2)
    3. [Sharing/Duplicating Anaconda Environments](#section4.3)
    4. [Using MongoDB](#section4.4)
5. [Our Software Infrastructure](#section5)
6. [Resources for Learning New Topics](#section6)
    1. [Slack](#section6.1)
    2. [Books](#section6.2)
    3. [Materials Science](#section6.3)
    4. [Computer Programming](#section6.4)
    5. [Professional Skills](#section6.5)

## 1. About Our Group <a name="section1"></a>
Computational Materials Design (CMD) lab's research focuses on atomistic simulations of complex surfaces and interfaces. We develop and use quantum mechanical simulations as well as molecular dynamics simulations to push the boundaries of knowledge in nanomaterials, 2D materials, and surface dominant-phenomena. Contributing to the Materials Genome Initiative, our lab develops scientific-software infrastructure to enable high-throughput computational studies, facilitating an accelerated discovery and design of novel materials. 

Active topics of interest are highly motivated by practical applications with an overarching goal of developing a computational Surface Genome database of materials. Towards this goal, we actively collaborate with experimentalists and theorists within ASU and several other universities and national laboratories, including Caltech, NIST-Gaithersburg and the Lawrence Berkeley National Lab. 

Our group maintains a [web-site](http://cmd.lab.asu.edu/) where you can find our latest research achievements along with other group related information.

## 2. After You Join the Group <a name="section2"></a>
A very warm welcome to the group. The following sections are written to guide you during your initial phases in the group. You are always welcome to seek in-person help from the CMD lab group members on any aspect of your research and your day-to-day life at ASU or Arizona. 

After joining the group, 

* Join Slack Group

Request access to the cmdlabworkspace.slack.com using your ASURITE e-mail id. Our group uses slack as an alternative for e-mail communications. If you haven't used slack before, the link to its help center can be found [here](http://get.slack.help/hc/en-us). Slack is a messaging app for teams which is searchable and shareable. The slack workspace will allow you to communicate quickly with Arunima as well as other group members. 

* Get Access to Group's Google Drive 

Our group maintains a Team Google Drive folder which provides access to group-specific resources. Request an access to the Team Drive by sending an e-mail to arunimasingh@asu.edu. In this drive you will find books, journal articles, presentations etc. related our research. Most of the shared data in the drive is either protected under some copy-right law or unpublished research. Do not share anything from this drive to someone who does not belong to the CMD lab. 

* Install ASU's VPN to Work from Home

Virtual Private Network (VPN) provides you an off-campus connectivity to ASU's network thereby providing access to research articles and library resources even when you are off-campus. Follow the instructions [here](http://getprotected.asu.edu/content/two-factor-authentication-services-vpn-connections) to setup VPN on your PC. 

While on campus you can access ASU's [free Wi-Fi](http://uto.asu.edu/services/campus-it-resources/wifi) using your ASURITE id.

* Get User Accounts on Supercomputing Resources

We have supercomputing resources both on-campus and off-campus. See [section 3](#section3) for more information about the individual supercomputers. 

-Get Access to ASU Supercomputing: 

Register for an account on the ASU supercomputing platform through this [link]( http://rcstatus.asu.edu/agave/howto/getting_an_account.php). Make sure to use your ASURITE id for the request. You can expect the ASU supercomputing staff to get back to you with the cluster login information within 24 hours. A guide to get started on using the cluster can be found [here](https://asurc.atlassian.net/wiki/spaces/RC/overview). To reach the Agave help-desk send a service request [here](https://rcstatus.asu.edu/agave/index.php).

-Get Access to XSEDE Supercomputing: 

Send an e-mail to Arunima and she will add your e-mail id to the XSEDE supercomputing. It typically takes the XSEDE staff 2-3 days to activate new users but they can take up to 5 days during busy times of the year. More information on how to use XSEDE supercomputers can be found in [section 3](#section3).

* Share Your Bio and Photo for Group's Website

Share your headshot and a brief bio which will be added on the group [website](https://cmd.lab.asu.edu/). 

* Setup Your Computer

See [section 4](#section4) to find out how to do this and a recommended list of software to install. 

## 3. Our Computing Resources <a name="section3"></a>

We perform ab-initio quantum mechanical simulations on supercomputers. The basic methodology for these simulations is density functional theory (DFT) but we also develop and use post-DFT methods such as hybrid functionals, many-body perturbation theory and dynamical correlations within the random phase approximation. Supercomputer provide the much needed memory and processing power which is orders of magnitude larger than what can be accessed through typical PC's. Our group has access to two major supercomputing clusters: 

### ASU Supercomputing <a name="section3.1"></a>

[Website link.](http://cores.research.asu.edu/research-computing/about-rc)
Note that agave has two partitions: (1) a home directory with a 100GB limit (/home/ASURITE) and (2) a scratch directory with no quota but purged every 30 days (/scratch/ASURITE).

### XSEDE Supercomputing <a name="section3.2"></a>

[Website link.](http://portal.xsede.org/#/guest)

Both the supercomputers are maintained by dedicated high-performance computing (HPC) staff. HPC staff maintains up-to-date free user-guides and also conducts web-seminars to guide you through the most effective use of the supercomputing resources. 

To get access to our XSEDE supercomputer Comet, create an account on the [XSEDE portal](https://portal.xsede.org/my-xsede?p_p_id=58&p_p_lifecycle=0&p_p_state=maximized&p_p_mode=view&_58_struts_action=%2Flogin%2Fcreate_account). After you have created your account, e-mail your XSEDE id to Arunima and she will add you to the group's Comet research allocation. 

Every user has an access to the HPC online [help-desk](https://portal.xsede.org/group/xup/help-desk) that can be used to get help on any aspect which is not covered in the existing documentation. For instance, if you are interested in installing a software which is not compatible with the supercomputer, you can seek the help of HPC staff to see if they can point you in the direction of right resources which will make your supercomputer account compatible for a successful installation of the software. 

## 4. Setting up a new computer <a name="section4"></a>

Depending on your project, you may need to install some of the following software on your computer: 

This guide walks you through the steps for setting up pymatgen, fireworks and atomate on ASU’s supercomputer, Agave. Installation steps for a local machine or another super computer will differ, but follow similar steps.
Setup an environment:

* Download anaconda installer from https://conda.io/docs/user-guide/install/linux.html and install anaconda using the command below. 

```
bash Anaconda-latest-Linux-x86_64.sh
```

* Create a python environment

``` conda create -n cms python=3.6 ```

* Activate the environment and install the base libraries (cms=computational materials science)

```source activate cms ```

```conda install numpy scipy matplotlib pandas ```

Install python libraries for open-source computational materials science software packages:
To install atomate (and hence pymatgen, pymatgen-db, fireworks and custodian) on the environment, use the following:

``` source activate cms ```

``` cd ~/anaconda3/envs/cms ```

``` mkdir code ```

``` cd code ```

``` git clone https://github.com/materialsproject/pymatgen.git --branch v2018.11.30```

``` git clone https://github.com/materialsproject/pymatgen-db.git --branch v2018.2.21```

``` git clone https://github.com/materialsproject/fireworks.git --branch v1.8.1```

``` git clone https://github.com/materialsproject/custodian.git --branch v2019.2.10```

``` git clone https://github.com/hackingmaterials/atomate.git --branch v0.8.4```

``` cd pymatgen ```

``` pip install –e . ```

``` cd .. ```

``` cd pymatgen-db ```

``` pip install –e . ```

``` cd .. ```

``` cd fireworks ```

``` pip install –e . ```

``` cd .. ```

``` cd custodian ```

``` pip install –e . ```

``` cd .. ```

``` cd atomate ```

``` pip install –e . ```

``` cd .. ```

* To install [matminer](https://github.com/hackingmaterials/matminer) use the following commands: 

 ```source activate cms ```
 
 ```cd ~/anaconda3/envs/cms/code/ ```
 
 ```git clone https://github.com/hackingmaterials/matminer.git ```

then enter the cloned repository or folder to install in the development mode: 

 ```cd matminer ```
 
 ```pip install –e . ```
 
 * To install [gasp](https://github.com/henniggroup/gasp) use the following commands:
 
 ```source activate cms ```
 
 ```cd ~/anaconda3/envs/cms/code/ ```
 
 ```git clone https://github.com/henniggroup/GASP-python.git ```
 
 then enter the cloned repository or folder to install in the developmen mode: 
 
 ```cd GASP-python```
 
 ```pip install -e .```
 
* Contact Arunima for VASP, GULP and [LAMMPS](https://lammps.sandia.gov/) executables



Other OS specific software: 

### Windows <a name="section4.1"></a>
* To acess ASU supercomputing or XSEDE supercomputing: install [putty](http://www.putty.org/), [WinSCP](http://winscp.net/eng/download.php), [Xming](https://sourceforge.net/projects/xming/)

### Mac <a name="section4.2"></a>
* [Jupyter](http://jupyter.org/) notebook

### Sharing/Duplicating Anaconda Environments <a name="section4.3"></a>
Anaconda enables users to share pre-built virtual environments through exporting a yaml file using the anaconda command-line tool. For cross-platform sharing version numbers are often different and may need slight modification to be compatible. To create your own yaml file use the following commands:

```conda activate my_sharing_env```

```conda env export > linux_atomate_stable.yml```

To install identical stable cms environments on remote cluster a stable linux cms environment can be found in the CMD lab google drive in SettingUpYourComputer. You can install this anaconda environment using the following commands:

``` conda env create -f linux_atomate_stable.yml ```

### Using MongoDB <a name="section4.4"></a>
[STARTUP COMMAND : ```mongod --auth --bind_ip_all --logpath log/mongod.log --fork```]

MongoDB is a document-oriented database program that allows users to store data in a json-like structure.

The steps required to install and setup your own MongoDB server are given below:

* Installing MongoDB:

To host a mongoDB server you need the server core installed

```
sudo apt install mongodb-server-core
```

To connect to a different mongoDB client you need the clients libraries installed

```
sudo apt install mongodb-clients
```

* Launching the Server
You can try to launch the mongoDB server with
```
mongod
```

If it throws an error saying "/data/db" doesnt exist, try the command

```
mkdir -p /data/db
```

You should now be able to launch the server, you can also launch the mongo shell to try out some commands and make sure everything works well:

```
mongo
```

This mongo server will only accept connections from the local system and needs to be explicitly told to accept all incoming connections using ```--bind_ip_all```
For security reasons we enable authentication using ```--auth```.

The final command should be:

```
mongod --auth --bind_ip_all --logpath log/mongod.log --fork
```

The ```--logpath``` option is used to save logs from the mongo server for debugging purposes and ```--fork``` creates a background process that will keep running after the admin signs out.

* Setting up users

MongoDB allows us to create users at a database level, but we can use an authentication server where we can specify users and roles for all databases.
By default the "admin" database is used for authentication purposes.

First you need to create your mongoDB root user:

You will have to run the mongo server without the ```--auth``` to create the first few users.

First create the root admin user:

```
use admin

db.createUser(
{
    user: "adminUser",
    pwd: "******",
    roles: [ { role: "root", db: "admin" } ]
}
)
```

Now the admin user can create different users similar to this:

```
use admin

db.createUser({
user: "Uranium",
pwd: "***",
roles: [
{ role: "readWrite", db: "database_orange" },
{ role: "read", db: "database_blue" }
]})
```
A new user Uranium is created who has readWrite access to database_orange and read access to database_blue.

More information about builtin roles can be [found here.](https://docs.mongodb.com/manual/core/security-built-in-roles/)

You can also create custom roles, by choosing the specific actions you want to allow:

```
db.runCommand({
createRole: "listDatabases",
privileges: [{ resource: { cluster : true }, actions: ["listDatabases"]}],
roles: [] 
})
```
This creates a new role called "listDatabases", which is allowed to view a list of all the databases on the server.
More information about privilege actions can be [found here.](https://docs.mongodb.com/manual/reference/privilege-actions/)

You can also grant new roles to existing users:

```
db.grantRolesToUser( "labrat", [{ role: "listDatabases", db: "admin" }])
```

More information about databases and collection commands will be added soon

## 5. Our software infrastructure <a name="section5"></a>

Any software-infrastructure developed by our group is shared via [github](https://github.com/as2362). Some of the software are open-access while others are only accessible by the members of the group and our collaborators. 

We use [VASP](https://www.vasp.at/) for density-functional theory simulations. This licensed software is accessible to all group members. The source code, the psuedopotential library and the makefiles and executables for our supercomputing platform can be found on the CMDLab google drive.  

## 6. Resources for learning new topics <a name="section6"></a>

### Slack <a name="section6.1"></a>
If you have a specific question, sometimes the easiest solution is to post it to the Slack group and crowdsource the answer from the CMD lab group members. 

### Books <a name="section6.2"></a>
As an ASU student or affiliate, you can get access to almost any book you’d like through the [ASU library](http://lib.asu.edu/). Our group has several technical books shared on the CMD lab google drive. If you need a book which is not available through the library we can purchase it through research funds. 

### Materials Science <a name="section6.3"></a>

It can be difficult to find resources that explain concepts in materials science clearly. Often, struggling through multiple attempts to understand a topic using several different resources in a patchwork and non-linear fashion is the only way forward. That said, the resources listed below are particularly helpful.

For beginners to density functional theory, I would recommend the book “Density Functional Theory: A Practical Introduction”, which truly achieves what it states by providing physical insights and relevant information rather than just listing equations. A copy is available within the group through the CMD lab google drive. If you are interested in the physics of the DFT, the book "Atomic and Electronic Structure of Solids" dives into the relevant physics at a level suited for graduate students. Again, this book is available on the CMD lab google drive. 


### Computer Programming <a name="section6.4"></a>
Note that there are usually many excellent resources to choose from when learning computer science topics. You usually have the flexibility of choosing to learn from a book, a video series, or even interactive tutorials like www.learnpython.org. Use the list below as potential starting points, but there exist many other high-quality alternatives you can find on your own and may be even better-suited to your needs.

* Terminal and Command Line

The command line is a text interface for your computer. It's a program that takes in commands, which it passes on to the computer's operating system to run. From the command line, you can navigate through files and folders on your computer, just as you would with Windows Explorer on Windows or Finder on Mac OS. The difference is that the command line is fully text-based.

If you are using a MAC, the "Macintosh Terminal Pocket Guide" is an easy to read and a beginner friendly introduction to the command lines which can be entered via the terminal. If you are using a Windows machine, you will need a SSH client like [putty](http://www.putty.org/) to access the Linux OS of your supercomputing resource. You can learn how to enter text-based commands on the Linux supercomputer through the SSH client. A good introductory book for learning how to use the Linux terminal is the "Linux Pocket Guide". Both the books are shared on the CMD lab google drive. 

* Python

For pure beginners to Python, you might try the book “Learn Python the Hard Way”. It is a fun and easy introduction to Python. Beginners that know a little but not a lot of Python can also look at “How to Make Mistakes in Python” (ebook). For intermediate programmers, you might try “20 Python Libraries You Aren’t Using (But Should)”  (ebook). For advanced programmers, you might try “Expert Python Programming”. These books are also on CMD lab's google drive.

* MongoDb

A (now somewhat old, but still clear) resource for beginning to use MongoDb is the “The Little MongoDB Book”:
https://github.com/karlseguin/the-little-mongodb-book
.There is also an extensive library of webinars on MongoDb on their official web site.

* Group Tutorials

To bring everyone up to speed with the software our group use we have created tutorials and introductory documentation for our software. You can find this documentation on the CMDLab Google Drive under the Code_Softwares folder.


### Professional Skills <a name="section6.5"></a>
To learn professional skills like writing papers and presenting talks and posters you can try this e-book http://go.nature.com/2opiiQh. You can also refer to the book "Trees, Maps, and Theorems" which is available on the CMD lab google drive. 
 


