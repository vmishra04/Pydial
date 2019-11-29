Pydial
==================================================================

The below is an example chat for recruitment case with the final aim of sending CV in a link

![Image of chat](https://github.com/vmishra04/Pydial/blob/master/Screen%20Shot%202019-11-28%20at%2011.59.01%20PM.png)


This is a single domain example called Recruitment

Some important files to create domain are:

* config/Tut-hdc-recruitment.cfg: Contains config information for chat
* ontology/ontologies/recruitment-rules.json : Contains slots that can be requested along with data to be provided,
in this case the URL for CV
* semi/RegexSemi_recruitment.py: Contains regex information for the slots
* topictracking/TopicTracking : Contains keyword information to switch to recruitment domain from general domain.
Currently it's looking for keyword "opportunity"
* semo/templates/recruitmentMessages.txt: Template file for machine generated sentences
* policy/HDCPolicy: Policy file for selecting next action



Welcome to PyDial: the CUED Python Statistical Dialog System (V1.4)
==================================================================

If you are reading this you have probably already downloaded the PyDial repo but if
you havent, do it now:

> git clone https://bitbucket.org/dialoguesystems/pydial.git
> cd pydial

PyDial uses Python 2.7 and has not been tested with other versions. Ensure 
that you use the requirements.txt file to install the appropriate dependencies
via pip. If you do not have pip installed yet first do

> sudo easy_install pip

otherwise exectued directly

> pip install -r requirements.txt

To check that you have a fully functioning system, run the PyDial functional tests

> sh testPyDial

You should see output similar to the following:

Running PyDial Tests
  1 tests/test_DialogueServer.py   time 0m3.908s
  2 tests/test_Simulate.py         time 0m18.990s
  3 tests/test_Tasks.py            time 0m0.492s
3 tests: 980 warnings,   0 errors
See test logs in _testlogs for details


Finally, install the documentation

> sh createDocs.sh

Then point your browser at documentation/Docs/index.html.  If PyDial is new to you,
read the Tutorial "Introduction to PyDial".


The PyDial Team

August 2018


PyDial is distributed under Apache 2.0 Licensed. See LICENSE
