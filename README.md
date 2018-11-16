# The Open Source Lab

This is where I will keep notes about my vision for an opensource lab.

## Background

The rationale for such an effort is based on my experience as a graduate student
and open source software engineer. You can read about this in [background.md](background.md).

## Research

There are a set of interesting projects that I'd want to do to better understand open source and generally how individuals interact with software
and one another during software development. Read about them in [research](research.md)

## Problems

### 1. Training in Reproducible Science

The problem is that scientists aren't adequately trained in reproducible practices
and general software engineering.

**What resources are currently available?**

Currenly, they have the following options:

 1. learn on their own (or do nothing) **default
 2. take additional courses (online or on campus)
 3. hire additional staff to supplement the missing knowledge
 4. find another mentor or student for guidance / support

**1** is the default, and obviously not ideal because we get a messy landscape of
bad practices, or just sad and overworked researchers. **2** (taking additional 
courses) is essentially devoting time and resources (in a large way)
to additional learning. While this is a great option, courses are expensive from
a monetary and time standpoint. Signing up for a (very social) workshop or traveling
to a conference is not a good fit for every kind of learner. 
It's also notable that the courses available
don't necessariy provide a holistic overview of the skills that the student
actually needs. **3** is a good solution but really only feasible for larger,
more established labs. It also places the challenge on needing the software 
engineering staff to learn some of the domain, and the succes of the effort is
dependent on how well the staff can communicate with the researchers. **4** also
works very well given a supportive PI or lab staff otherwise. This is also usually
hard to find.

**What about data science?**

There are a myriad of "data science" coures popping up at universities that will
teach basic data wrangling, machine learning, etc., and this has resulted from
a huge increase in the demand for "data scientists" and thus the demand for degrees
to do it. The track of "data science" does **not** address the core of this issue
because at base value, it's another cirriculum to get through with a focus on
the applied science. You can easily learn to use Python, R, without learning about
how to run jobs at scale, create reproducible builds, or set up continuous integration.

**What about computer science?**

Computer science is commonly confused with programming. The culture around computer science
departments sometimes focused on the idea of needing to understand the complexity of systems,
programming languages, and algorithms. Why this is of course invaluable, there is an important
distinction here. Scientists need applied training in scaled computing, reproducibility, version control, and continuous integration. They need training in programming. 

> Computer science is not the same as programming.

What I see happening is that, while it's the case that practices from computer science **do**
translate into good practices for scientists, the set of things you need to practice good
science is a subset (smaller) of the domain of computer science. We have courses for 
computer science, and for data science, but we currently don't have enough base support 
for the gray area between - the programming practices that both of them share. It is not
"lofty enough" of an achievement or certificate to learn to open pull requests, write
documentation, or run jobs on an HPC cluster. 


### 2. Support for Reproducible Science

The culmination of the above is that the biologists, chemists,
and psychologists that are already enrolled in their separate departments run into issues
focused around these topics. They don't have the bandwidth to watch entire lecture videos in
person or online, and the result is either a poorly executed analysis, or an email 
as a cry for help to research computing support.

**What about teaching staff?**

I've seen first hand, both in college, graduate school, and after, how well an army of Teaching
Assistant's paired with a great professor can be. It can help with the training of 400+ students
at once, albeit the assessment practices are catered to servethis volume. Firstly, the students 
enrolled in these courses do not reflect the complete set that need the training. Arguably, every
graduate student or staff that needs to interact with data and "do good science" needs the
trianing, but courses that teach basic programming are (mostly) undergraduates going for a 
Computer Science major. Second, the reality that the courses are exploding in numbers, and it's hard
for the teaching staff to keep up, is simple evidence that it's time for change. This isn't new
or surprising, because we have platforms like the Khan Academy, EdX, and coursera to scale the
courses. However, it's still problematic that as the number of students grows, the teaching
staff needs to as well, and this can only go so far.


**What about computing support?**

An email to research computing support is by far the quicket way to get help with a tiny
thing like submitting a job to SLURM. In fact, this level of support is the one factor (in my mind)
that places a local HPC cluster one head above whatever cloud options are available. I don't
see Google Cloud or Amazon being able to sit down after hours with a graduate student and help
them debug their code. The limitations of this team are the same as with teaching staff - it 
works up to a certain number of users, and then you hit a ceiling.

For both of the above, problem is that the **support for reproducible science** does not scale.


### 3. A Culture of Serious Science

A soft problem in this domain is with respect to culture. It is respectable to get a degree
in a field, especially a STEM field, and especially something that is less applied. 
As stated earlier, learning tiny programming skills, or putting a focus on the human
element of having fun instead of rigorous testing, is often overlooked. It's a bit of a catch-22
because people will be motivated and learn a lot when they are having fun, but the ways
that we expect students to learn are (sometimes) fun, but (most of the time) stresful.
In order to help with this problem, we need to have more fun.

### Summary of Problems

I think that traditional academic training is dated. It doesn't easily scale, 
is not suited for learners that want (and need) to learn by doing, and
doesn't focus on the applied skills that are actually needed. 
We have now summarized the main problems:

 1. Training and support for reproducible science is not scaling well
 2. Reproducible Practices and programming are wrapped into Computer Science and Data Science, but they are different.
 3. The culture is very academic and series.

I think we need
to do it differently, and while we cannot (and should not) totally restructure
a university, we can start to develop initiatives that can grow in the same
was as open source software. This is the open source lab.

## Goals

We can now define the goals of the open source lab. The open source lab:

 1. should not be a traditional course, or offer courses. There are no assignments or testing or similar that would confuse the work with a more stressful and serious academic environment.
 2. should be a base of work (tools) that are needed for the same scientists
 3. should be able to exist in a university environment, and across departments. Each department can have multiple entrypoints for their students to participate. For example, an independnet student might coincide with a project with the lab, or training for HPC a required module of sorts that the lab provides.
 4. must be self-sustaining. This means the projects are open source across universities. This also means that tools to provide support, help, etc., are also shared.

## Tools Needed

This is a brief list of tools that I think are necessary to get started.

 1. An open source "helpme" command line tool to submit questions to a shared discussion and question area. The best idea so far is integration with the [Cyber Infrastructure discourse board](https://ask.cyberinfrastructure.org/). Using a tool like [helpme](https://www.github.com/vsoch/helpme) I should be able to quickly ask, or answer questions.
 2. An interface akin to CodeStepByStep.com that asks (and quizzes) simple command line or job manager questions. There are no courses to sign up for, and it's just a fun way to spend time.
