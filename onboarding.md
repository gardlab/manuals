# You've joined the GARD Lab! What's next?

Starting a new position can be overwhelming. Adapting to new systems, adhereing to protocols, adjusting to the lab culture - all challenging tasks (both hopefully exciting)! This onboarding manual in intended to give you a jump start. It will walk you through the tools that the lab uses, identify mandatory trainings that you will need to take, and guide you through the onboarding process. 

## Tools (for everyone)
The following are tools that the lab uses to run smoothly. All lab members are expected to engage with these tools to various degrees.

* **Github** (https://github.com/gardlab/). The lab has its own github account. This account should be used to store manuals and protocols, data analysis scripts, and open-source data and stimuli. The data manager is in charge of managing the account. 
    * Since we are a new lab, we don't yet have a file organization system for our github account. One way to organize files is through data modality (e.g., all scripts related to processing fMRI data; all scripts related to processing genetic data). There may be other systems. We will develop a protocol together. 
    * Know that anything uploaded to the lab github account must be paired with a readme file
    * When you post code, make sure it is flawless because we don't want to distribute buggy code to the world. Have the data manager check it and get approval before posting. 
* **Slack** (https://slack.com/). Slack is a great tool to faciliate communication among lab members. Sometimes emails get lost and we all get too many emails anyways. Slack each other for quick questions. Use emails for more formal communication (e.g., to send Dr. Gard a proposal draft)
    * Install slack on your computer(s). The lab manager or Dr. Gard will add you to the gardlab slack account (gardlab.slack.com) - remind them if they don't! All senior staff (grad students, staff, postdocs) should be given administrator privledges
    * Create channels for different projects. Use the #random channel for non-work-related chats or make a private chat with another lab mate. 
    * Turn on your notifications during work hours or check Slack 1x/day on work days. 
    * Do not worry if someone slacks you after hours - you are not expected to respond, but some of us may work at odd times. 
    * Keep if professional. Add memes, make jokes, have fun - but keep the banter respectful
    * Try to keep each channel on topic, so that people can suscribe only to the channels that concern them. For messages to one person or a small group, use direct messages.
* **Email**. We have several lab listserves for sending emails to several lab members at once. The lab manager or Dr. Gard will add you to the appropriate listserves - remind them if they don't!
    * gardlabseniorstaff@umd.edu = PI, graduate students, staff, postdocs
    * gardlabundergrad@umd.edu = undergraduate research assistants  
    * Staff: To add someone to a lab listserve email, click on the menu in the top right of your gmail inbox frontpage. Click "groups". Click "add members".
    * Staff: If you need to create a new listserve email, you need to request this through UMD IT. Go [here](https://umd.service-now.com/itsupport?id=service&service=fd7603b637911e406574c97a43990ebb)
*  **Google Drive**. Google drive is great for working in shared documents that can't be shared with the world (otherwise, Github). The lab manager or Dr. Gard will add you to the GARD Lab google folder - remind them if they don't! What is in the GARD Lab google drive? 
    * Lab Meetings: lab agendas, goals document - other stuff as it comes up (Staff should amend this manual as needed)
    * Resources/Presentations: Whenever there is a presentation in lab meeting or a training session that constitutes "general knowledge", it should be added to this folder. We spend a lot of time making presentations - let's store this knowledge and re-use it!
    * Undergraduate Projects: each semester, undergraduate research assistants undertake a small project - this may be creating a public science scholarship blog, presenting a data processing stream or an empirical paper, etc. These projects should be stored in this folder to include guidelines and examples
    * Undergraduate Tasks
    * Website: How-to document for making changes to the website. Content that needs to be (or is already) uploaded to the website.
    * Note that Google Drive works well when you download the desktop version so it syncs between the cloud and your local computer. 
    * Note Note - Google Drive through UMD is NOT HIPAA-compliant. That means that data of any kind (with or withour personal protected information) should not be stored here! 
 * **UMD Box** UMD Box is HIPAA-compliant and can be used to store data with and without personal protected information. Box should also be used to store scripts, stimuli, and code that hasn't been "vetted" before it is posted to github. UMD has also made Box storage unlimited. So go wild. 
    * Box works best when you download the desktop version so it syncs between the cloud and your local computer. 
    * Log-in using your UMD email account [here](https://umd.account.box.com/login)
    * The lab manager or Dr. Gard will add you to the GARD Lab box folder - remind them if they don't!
    * Since we are a new lab, we don't yet have a file organization system for our Box account. We will develop a protocol together.
    * You should never store data on your personal computer. This is what the desktop version of Box is for. Map your scripts to the datafiles located on box or the shared server drive (more soon on that)
 * **Gard Lab Server** In collaboration with Dr. Lea Dougherty, Dr. Gard has purchased a remote linux server. All senior staff and UGs working on relevant projects need access. The server is named "basil" because herbs are the best. Future servers will be also be named in the herb family - Dr. Gard is partial to rosemary and chives, but TBD.
   * The broadest file structure for the server is as follows:
```
/software/basil ## This space is meant as a shared software directory where you can install software packages away from the data.
/data/basil/gard ## This space is meant to store GARD Lab data only
/data/basil/shared ## This space is meant to store ABCD imaging data
/data/basil/dougherty ## This space is meant to store Dougherty lab data only
```
   * To obtain server access:
      1. Create a Glue/TerpConnect account [here](https://cgi.oit.umd.edu/cgi-bin/account/activation.cgi). Select the TerpConnect service (may already be selected) and click the 'Submit' button.  The account should be created in a day or so. 
      2. The data manager or Dr. Gard will grant access to the machine (basil.umd.edu) by emailing Prasad Dharmasena (pkd@umd.edu)
      3. You will also need several programs to access the server
            1. The UMD VPN Client. When you are off-campus, you will need to use a "virtual private network" or VPN to access the server. This does not apply if you are working in the lab or on campus. You should NEVER connect to ther server using public wifi (e.g., Starbucks). Go [here](https://it.umd.edu/spotlight/connections/what-vpn) to download the UMD VPN Client and learn more: 
            2. A Secure Shell (SSH) Client. Be sure to allow ‘X11 forwarding’ in the settings if you need to display graphics from the server on your local screen. For PCs, download PuTTY [here](https://www.putty.org/). MACs have a built-in SSH Client, which you can access through terminal (Finder --> Utilities --> Terminal). The hostname is basil.umd.edu and the login credentials are your UMD Directory ID/password.
            4. Mounting the server drive onto a local computer (either your own or in the lab) via SMB/Samba access: This allows you to mount the same filesystems as network drives on your Windows/Mac machines. You need to use your operating system’s “map a network drive” (or similar wording) methods to access. The hostname is basil.umd.edu and the login credentials are your Directory ID and the samba password I’ve saved in a text file in your Glue account (in ~/basil/samba-pw file). Please use the above SSH method to login and retrieve that password.
        
## Trainings (for everyone)
All of the following at trainings that must be completed before you start working in the lab. In some cases, you will attend a lab-wide training during your first semester in the GARD Lab.
*  **UMD History** The African American History and Landmarks at UMD Tour. In-person where possible. https://bsos.umd.edu/diversity/african-american-history-and
*  **Diversity, Equity, and Inclusion Training** Lab staff should request an annual training for the lab through the UMD Office of Diversity and Inclusion [here](https://diversity.umd.edu/training-education/diversity-training/)
*  **Human Subjects Research** All lab members working on a research project must complete [IRB training](https://research.umd.edu/irbtraining). This includes (a) CITI (Collaborative Institutional Training Initiative) Training, and (b) HIPAA (Health Insurance Portability and Accountability Act of 1996) Training. There may be additional IRB trainings required for specific projects. That information will be listed here once it becomes available.

## Trainings/Resources (for some)
There are several major research areas that the lab tackles. Each method/approach requires heavy investment - this is why we specialize! You can't know everything - we collaborate with other experts while you become an expert in 1-2 well-defined methods/approaches. 
* **Program Policies** All new graduate students (Clinical, Developmental, NACS) are required to review their area's graduate student handbook and promptly set up a meeting with Dr. Gard for discussion. This should occur before the Fall semester of your first year or shortly after your first semester begins. 
   *  [Clinical Psych](https://psyc.umd.edu/graduate/clinical-psychology)
   *  [Developmental Psych](https://psyc.umd.edu/graduate/developmental-program)
   *  [Neuroscience and Cognitive Neuroscience](https://nacs.umd.edu/landingtopic/current-nacs-students)
* **Linux bash command line** - most folks in the lab need to learn how to navigate in the command line environment. Our server, basil, is best accessed from a SSH client. Below are a few resources that will give you a basic introduction to linux command line. If you find a resource that you like, please add it here with some notes about how it is different/better/more fun than those listed below! 
   * https://linuxcommand.org/
   * https://ubuntu.com/tutorials/command-line-for-beginners#1-overview
   * http://www.ee.surrey.ac.uk/Teaching/Unix/
   * https://hrs.isr.umich.edu/genomics-workshop/online-video-modules (a couple introductory videos from my collaborator at Michigan)
* **fMRI** - functional MRI is a major focus on the lab. There are several parallels in working with task-based and resting-state fMRI data, but also several differences. Graduate students with a focus on fMRI research should intend to take Dr. Luis Pessoa's NACS course "Introduction to Functional Magnetic Resonance Imaging". In addition, there are several online courses that can be incredibly helpful, some geared towards different packages. Check in with Dr. Gard to see which courses/trainings you should take:
   * Andy Jahn's Brain Book (has tutorials for several programs): https://andysbrainbook.readthedocs.io/en/latest/
   * NIH fMRI course - slides and videos: https://fmrif.nimh.nih.gov/public/fmri-course/index_html
   * FSL course: https://fsl.fmrib.ox.ac.uk/fslcourse/
   * SPM12 Manual: https://www.fil.ion.ucl.ac.uk/spm/doc/manual.pdf
   * fMRI basics, talk by Rebecca Saxe: https://www.youtube.com/watch?v=yA65FuSpOMs
   * Books: (1) Huettel, S. A., Song, A.W., & McCarthy, G. (2008). Functional Magnetic Resonance Imaging (2nd edition). Sinauer Associates, Inc: Sunderland, Massachusetts, USA. (2) Poldrack, Russell A. Mumford, Jeanette A. Nichols, Thomas E. Handbook of functional MRI data analysis. 2011
   * BIDS: https://bids.neuroimaging.io/
   * fMRIprep: https://github.com/nipreps/fmriprep
   * Mumford Brain Stats (fMRI help): https://mumfordbrainstats.tumblr.com/
   * fMRI power calculation options: (1) https://jeanettemumford.org/fmripower/ (2) http://neuropowertools.org/
   * list of summer schools in neuroscience and related fields: https://github.com/PhABC/neuroSummerSchools
* **R Statistical Software** - one of the most flexible (and free!) statistical software packages available is R. There is an incredible online support system and resources for statistical analysis and data visualization within R. Using R further allows the lab to engage in reproducible open science practices. But absolutely the learning curve can be steep. In addition to learning what statistical tools are at your disposal, the assumptions of each tool, and the theory behind it, you have to figure out *how* to implement said tool/approach in R. All trainees working on a project that involves data analysis needs to learn the basics of R. For graduate students, you will get some of this training in your first year stats courses and in subsequent stats courses that are germaine to your research program. But here are some helpful resources for R newbies and experts alike:
   * Introduction to R (a free book): https://moderndive.com/
   * R for Data Science (another free book): https://r4ds.had.co.nz/
   * Introductory R course through DataCamp: https://www.datacamp.com/courses/free-introduction-to-r
   * Quick-R (includes tutorial, data management tips, basic stats approaches): https://www.statmethods.net/
   * Hierarchical Linear Modeling and other advanced methods: http://www.r-tutor.com/
   * Linear Mixed Models: https://gkhajduk.github.io/2017-03-09-mixed-models/
* **Epigenetics and Genetics**
   * Genomics for Social Scientists at University of Michigan, Ann Arbor (https://hrs.isr.umich.edu/genomics-workshop). There are two 1-week workshops offerred by my collaborators (and former mentors) at the Institute for Social Research at UMICH. There is a 1-week course on genomic data in June, and another 1-week workshop in using epigenetic data in January. There is an application. Talk to Dr. Gard for more information!

