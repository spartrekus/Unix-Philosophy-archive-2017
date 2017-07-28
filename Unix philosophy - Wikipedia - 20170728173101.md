Unix philosophy {#firstHeading .firstHeading lang="en"}
===============

From Wikipedia, the free encyclopedia

Jump to:
[navigation](https://en.wikipedia.org/wiki/Unix_philosophy#mw-head),
[search](https://en.wikipedia.org/wiki/Unix_philosophy#p-search)

[![](./Unix%20philosophy%20-%20Wikipedia_files/220px-Ken_n_dennis.jpg)](https://en.wikipedia.org/wiki/File:Ken_n_dennis.jpg)

[](https://en.wikipedia.org/wiki/File:Ken_n_dennis.jpg "Enlarge")

[Ken
Thompson](https://en.wikipedia.org/wiki/Ken_Thompson "Ken Thompson") and
[Dennis
Ritchie](https://en.wikipedia.org/wiki/Dennis_Ritchie "Dennis Ritchie"),
key proponents of the Unix philosophy

The **Unix philosophy**, originated by [Ken
Thompson](https://en.wikipedia.org/wiki/Ken_Thompson "Ken Thompson"), is
a set of cultural norms and philosophical approaches to
[minimalist](https://en.wikipedia.org/wiki/Minimalism_(computing) "Minimalism (computing)"),
[modular](https://en.wikipedia.org/wiki/Modularity_(programming) "Modularity (programming)")
[software
development](https://en.wikipedia.org/wiki/Software_development "Software development").
It is based on the experience of leading developers of the
[Unix](https://en.wikipedia.org/wiki/Unix "Unix") [operating
system](https://en.wikipedia.org/wiki/Operating_system "Operating system").
Early Unix developers were important in bringing the concepts of
modularity and reusability into software engineering practice, spawning
a "[software
tools](https://en.wikipedia.org/wiki/Software_tools "Software tools")"
movement. Over time, the leading developers of Unix (and programs that
ran on it) established a set of cultural norms for developing software,
norms which became as important and influential as the technology of
Unix itself; this has been termed the "Unix philosophy."

The Unix philosophy emphasizes building simple, short, clear, modular,
and extensible code that can be easily maintained and repurposed by
developers other than its creators. The Unix philosophy favors
[composability](https://en.wikipedia.org/wiki/Composability "Composability")
as opposed to [monolithic
design](https://en.wikipedia.org/wiki/Monolithic_application "Monolithic application").

Contents
--------

 [hide] 

-   [1 Origin](https://en.wikipedia.org/wiki/Unix_philosophy#Origin)
-   [2 *The UNIX Programming
    Environment*](https://en.wikipedia.org/wiki/Unix_philosophy#The_UNIX_Programming_Environment)
-   [3 *Program Design in the UNIX
    Environment*](https://en.wikipedia.org/wiki/Unix_philosophy#Program_Design_in_the_UNIX_Environment)
-   [4 Doug McIlroy on Unix
    programming](https://en.wikipedia.org/wiki/Unix_philosophy#Doug_McIlroy_on_Unix_programming)
-   [5 Do One Thing and Do It
    Well](https://en.wikipedia.org/wiki/Unix_philosophy#Do_One_Thing_and_Do_It_Well)
-   [6 Eric Raymond’s 17 Unix
    Rules](https://en.wikipedia.org/wiki/Unix_philosophy#Eric_Raymond.E2.80.99s_17_Unix_Rules)
-   [7 Mike Gancarz: The UNIX
    Philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#Mike_Gancarz:_The_UNIX_Philosophy)
-   [8 "Worse is
    better"](https://en.wikipedia.org/wiki/Unix_philosophy#.22Worse_is_better.22)
-   [9 See also](https://en.wikipedia.org/wiki/Unix_philosophy#See_also)
-   [10 Notes](https://en.wikipedia.org/wiki/Unix_philosophy#Notes)
-   [11
    References](https://en.wikipedia.org/wiki/Unix_philosophy#References)
-   [12 External
    links](https://en.wikipedia.org/wiki/Unix_philosophy#External_links)

Origin[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=1 "Edit section: Origin")]
-----------------------------------------------------------------------------------------------------------------------

The UNIX philosophy is documented by [Doug
McIlroy](https://en.wikipedia.org/wiki/Doug_McIlroy "Doug McIlroy")^[[1]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-taoup-ch1s6-1)^
in the Bell System Technical Journal from
1978:^[[2]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-2)^

1.  Make each program do one thing well. To do a new job, build afresh
    rather than complicate old programs by adding new "features".
2.  Expect the output of every program to become the input to another,
    as yet unknown, program. Don't clutter output with extraneous
    information. Avoid stringently columnar or binary input formats.
    Don't insist on interactive input.
3.  Design and build software, even operating systems, to be tried
    early, ideally within weeks. Don't hesitate to throw away the clumsy
    parts and rebuild them.
4.  Use tools in preference to unskilled help to lighten a programming
    task, even if you have to detour to build the tools and expect to
    throw some of them out after you've finished using them.

Later summarized by [Peter H.
Salus](https://en.wikipedia.org/wiki/Peter_H._Salus "Peter H. Salus") in
A Quarter-Century of Unix
(1994):^[[1]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-taoup-ch1s6-1)^
This is the Unix philosophy:

-   Write programs that do one thing and do it well.
-   Write programs to work together.
-   Write programs to handle text streams, because that is a universal
    interface.

In the book *[The Pragmatic Programmer: From Journeyman to
Master](https://en.wikipedia.org/wiki/The_Pragmatic_Programmer "The Pragmatic Programmer")*
the authors mention the philosophy of combining "small, sharp tools" and
the use of "common underlying format—the line-oriented, plain text
file"^[[3]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-3)^
to accomplish larger tasks.

> The whole philosophy of UNIX seems to stay out of
> [assembler](https://en.wikipedia.org/wiki/Assembly_language "Assembly language").
>
> — [Joseph Henry
> Condon](https://en.wikipedia.org/wiki/Joseph_Henry_Condon "Joseph Henry Condon")^[[4]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-interview-4)^

The development of
[pipes](https://en.wikipedia.org/wiki/Unix_pipes "Unix pipes") in 1973
formalized the existing principle of
[stdin](https://en.wikipedia.org/wiki/Stdin "Stdin")-[stdout](https://en.wikipedia.org/wiki/Stdout "Stdout")
into a philosophy in [Version 3
Unix](https://en.wikipedia.org/wiki/Version_3_Unix "Version 3 Unix"),
with older software rewritten to comply. Previously visible in early
utilities such as
[wc](https://en.wikipedia.org/wiki/Wc_(Unix) "Wc (Unix)"),
[cat](https://en.wikipedia.org/wiki/Cat_(Unix) "Cat (Unix)"), and
[uniq](https://en.wikipedia.org/wiki/Uniq "Uniq"), McIlroy cites
Thompson's [grep](https://en.wikipedia.org/wiki/Grep "Grep") as what
"ingrained the tools outlook irrevocably" in the operating system, with
later tools like
[tr](https://en.wikipedia.org/wiki/Tr_(Unix) "Tr (Unix)"),
[m4](https://en.wikipedia.org/wiki/M4_(computer_language) "M4 (computer language)"),
and [sed](https://en.wikipedia.org/wiki/Sed "Sed") imitating how grep
transforms the [input
stream](https://en.wikipedia.org/wiki/Input_stream "Input stream").^[[5]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-reader-5)^

"The truth about Unix: *The user interface is
horrid*"^[[6]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-6)^
was a 1981 criticism of the design philosophy published in
*[Datamation](https://en.wikipedia.org/wiki/Datamation "Datamation")*.
It was written by [Don
Norman](https://en.wikipedia.org/wiki/Don_Norman "Don Norman"), who had
a background in cognitive science and was the key proponent of the
then-current philosophy of [cognitive
engineering](https://en.wikipedia.org/wiki/Cognitive_engineering "Cognitive engineering"),^[[4]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-interview-4)^
apparently focused on how engineers comprehend and form a personal
[cognitive
model](https://en.wikipedia.org/wiki/Cognitive_model "Cognitive model")
of a system.

*The UNIX Programming Environment*[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=2 "Edit section: The UNIX Programming Environment")]
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[![](./Unix%20philosophy%20-%20Wikipedia_files/220px-Rob-pike-oscon.jpg)](https://en.wikipedia.org/wiki/File:Rob-pike-oscon.jpg)

[](https://en.wikipedia.org/wiki/File:Rob-pike-oscon.jpg "Enlarge")

[Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike "Rob Pike"), co-author
of *[The UNIX Programming
Environment](https://en.wikipedia.org/wiki/The_UNIX_Programming_Environment "The UNIX Programming Environment")*

In their preface to the 1984 book, *[The UNIX Programming
Environment](https://en.wikipedia.org/wiki/The_UNIX_Programming_Environment "The UNIX Programming Environment")*,
[Brian
Kernighan](https://en.wikipedia.org/wiki/Brian_Kernighan "Brian Kernighan")
and [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike "Rob Pike"), both
from [Bell Labs](https://en.wikipedia.org/wiki/Bell_Labs "Bell Labs"),
give a brief description of the Unix design and the Unix
philosophy:^[[7]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-unix1984-7)^

> Even though the UNIX system introduces a number of innovative programs
> and techniques, no single program or idea makes it work well. Instead,
> what makes it effective is the approach to programming, a philosophy
> of using the computer. Although that philosophy can't be written down
> in a single sentence, at its heart is the idea that the power of a
> system comes more from the relationships among programs than from the
> programs themselves. Many UNIX programs do quite trivial things in
> isolation, but, combined with other programs, become general and
> useful tools.

The authors further write that their goal for this book is "to
communicate the UNIX programming
philosophy."^[[7]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-unix1984-7)^

*Program Design in the UNIX Environment*[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=3 "Edit section: Program Design in the UNIX Environment")]
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[![](./Unix%20philosophy%20-%20Wikipedia_files/220px-Brian_Kernighan_in_2012_at_Bell_Labs_2.jpg)](https://en.wikipedia.org/wiki/File:Brian_Kernighan_in_2012_at_Bell_Labs_2.jpg)

[](https://en.wikipedia.org/wiki/File:Brian_Kernighan_in_2012_at_Bell_Labs_2.jpg "Enlarge")

[Brian
Kernighan](https://en.wikipedia.org/wiki/Brian_Kernighan "Brian Kernighan")
has written at length about the Unix philosophy

In October 1984, Brian Kernighan and Rob Pike published a paper called
*Program Design in the UNIX Environment*. In this paper, they criticize
the accretion of program options and features found in some newer Unix
systems such as [4.2BSD](https://en.wikipedia.org/wiki/4.2BSD "4.2BSD")
and [System V](https://en.wikipedia.org/wiki/System_V "System V"), and
explain the Unix philosophy of software tools, each performing one
general
function:^[[8]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-design1984-8)^

> Much of the power of the UNIX operating system comes from a style of
> program design that makes programs easy to use and, more important,
> easy to combine with other programs. This style has been called the
> use of *software tools*, and depends more on how the programs fit into
> the programming environment and how they can be used with other
> programs than on how they are designed internally. [...] This style
> was based on the use of *tools*: using programs separately or in
> combination to get a job done, rather than doing it by hand, by
> monolithic self-sufficient subsystems, or by special-purpose, one-time
> programs.

The authors contrast Unix tools such as `cat`, with larger program
suites used by other
systems.^[[8]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-design1984-8)^

> The design of `cat` is typical of most UNIX programs: it implements
> one simple but general function that can be used in many different
> applications (including many not envisioned by the original author).
> Other commands are used for other functions. For example, there are
> separate commands for file system tasks like renaming files, deleting
> them, or telling how big they are. Other systems instead lump these
> into a single "file system" command with an internal structure and
> command language of its own. (The PIP file copy program found on
> operating systems like
> [CP/M](https://en.wikipedia.org/wiki/CP/M "CP/M") or
> [RSX-11](https://en.wikipedia.org/wiki/RSX-11 "RSX-11") is an
> example.) That approach is not necessarily worse or better, but it is
> certainly against the UNIX philosophy.

Doug McIlroy on Unix programming[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=4 "Edit section: Doug McIlroy on Unix programming")]
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[![](./Unix%20philosophy%20-%20Wikipedia_files/220px-Dennis_Ritchie_(right)_Receiving_Japan_Prize.jpeg)](https://en.wikipedia.org/wiki/File:Dennis_Ritchie_(right)_Receiving_Japan_Prize.jpeg)

[](https://en.wikipedia.org/wiki/File:Dennis_Ritchie_(right)_Receiving_Japan_Prize.jpeg "Enlarge")

[Doug
McIlroy](https://en.wikipedia.org/wiki/Doug_McIlroy "Doug McIlroy")
(left) with [Dennis
Ritchie](https://en.wikipedia.org/wiki/Dennis_Ritchie "Dennis Ritchie")

McIlroy, then head of the Bell Labs Computing Sciences Research Center,
and inventor of the [Unix
pipe](https://en.wikipedia.org/wiki/Pipeline_(Unix) "Pipeline (Unix)"),^[[9]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-9)^
summarized the Unix philosophy as
follows:^[[1]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-taoup-ch1s6-1)^

> This is the Unix philosophy: Write programs that do one thing and do
> it well. Write programs to work together. Write programs to handle
> [text
> streams](https://en.wikipedia.org/wiki/Standard_streams "Standard streams"),
> because that is a universal interface.

Beyond these statements, he has also emphasized simplicity and
[minimalism](https://en.wikipedia.org/wiki/Minimalism "Minimalism") in
Unix
programming:^[[1]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-taoup-ch1s6-1)^

> The notion of "intricate and beautiful complexities" is almost an
> oxymoron. Unix programmers vie with each other for "simple and
> beautiful" honors — a point that's implicit in these rules, but is
> well worth making overt.

Conversely, McIlroy has criticized modern
[Linux](https://en.wikipedia.org/wiki/Linux "Linux") as having [software
bloat](https://en.wikipedia.org/wiki/Software_bloat "Software bloat"),
remarking that, "adoring admirers have fed Linux goodies into a
disheartening state of
[obesity](https://en.wikipedia.org/wiki/Obesity "Obesity")."^[[10]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-10)^
He contrasts this with earlier approach taken at Bell Labs when
developing and revising [Research
Unix](https://en.wikipedia.org/wiki/Research_Unix "Research Unix"):^[[11]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-11)^

> Everything was small... and my heart sinks for Linux when I see the
> size of it. [...] The [manual
> page](https://en.wikipedia.org/wiki/Man_page "Man page"), which really
> used to be a manual *page*, is now a small volume, with a thousand
> options... We used to sit around in the Unix Room saying, 'What can we
> throw out? Why is there this option?' It's often because there is some
> deficiency in the basic design — you didn't really hit the right
> design point. Instead of adding an option, think about what was
> forcing you to add that option.

Do One Thing and Do It Well[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=5 "Edit section: Do One Thing and Do It Well")]
-----------------------------------------------------------------------------------------------------------------------------------------------------------------

As stated by McIlroy, and generally accepted throughout the Unix
community, Unix programs have always been expected to follow the concept
of DOTADIW, or "Do One Thing and Do It Well." Sources for the acronym
DOTADIW are limited throughout the internet, but is discussed at length
during the development and packaging of new operating systems,
especially in the Linux community. There has been a point of great
contention during the Linux
[systemd](https://en.wikipedia.org/wiki/Systemd "Systemd") debates of
2014–2015, and especially in the
[Debian](https://en.wikipedia.org/wiki/Debian "Debian")
community.^[[12]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-12)^

[Patrick
Volkerding](https://en.wikipedia.org/wiki/Patrick_Volkerding "Patrick Volkerding"),
the project lead of [Slackware
Linux](https://en.wikipedia.org/wiki/Slackware_Linux "Slackware Linux"),
invoked this design principle in a criticism of the systemd
architecture, stating that, "attempting to control services, sockets,
devices, mounts, etc., all within one
[daemon](https://en.wikipedia.org/wiki/Daemon_(computing) "Daemon (computing)")
flies in the face of the UNIX concept of doing one thing and doing it
well."^[[13]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-volkerding-2012-13)^

Eric Raymond’s 17 Unix Rules[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=6 "Edit section: Eric Raymond’s 17 Unix Rules")]
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

In his book *[The Art of Unix
Programming](https://en.wikipedia.org/wiki/The_Art_of_Unix_Programming "The Art of Unix Programming")*
that was first published in
2003,^[[14]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-14)^
[Eric S.
Raymond](https://en.wikipedia.org/wiki/Eric_S._Raymond "Eric S. Raymond"),
an American programmer and open source advocate, summarizes the Unix
philosophy as [KISS
Principle](https://en.wikipedia.org/wiki/KISS_Principle "KISS Principle")
of "Keep it Simple,
Stupid."^[[15]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-15)^
He provides a series of design
rules:^[[1]](https://en.wikipedia.org/wiki/Unix_philosophy#cite_note-taoup-ch1s6-1)^

Rule of [Modularity](https://en.wikipedia.org/wiki/Modularity_(programming) "Modularity (programming)")
:   Developers should build a program out of simple parts connected by
    well defined interfaces, so problems are local, and parts of the
    program can be replaced in future versions to support new features.
    This rule aims to save time on debugging code that is complex, long,
    and unreadable.

Rule of Clarity
:   Developers should write programs as if the most important
    communication is to the developer who will read and maintain the
    program, rather than the computer. This rule aims to make code as
    readable and comprehensible as possible for whoever works on the
    code in the future.

Rule of Composition
:   Developers should write programs that can communicate easily with
    other programs. This rule aims to allow developers to break down
    projects into small, simple programs rather than overly complex
    monolithic programs.

Rule of [Separation](https://en.wikipedia.org/wiki/Separation_of_mechanism_and_policy "Separation of mechanism and policy")
:   Developers should separate the mechanisms of the programs from the
    policies of the programs; one method is to divide a program into a
    front-end interface and a back-end engine with which that interface
    communicates. This rule aims to prevent bug introduction by allowing
    policies to be changed with minimum likelihood of destabilizing
    operational mechanisms.

Rule of Simplicity
:   Developers should design for simplicity by looking for ways to break
    up program systems into small, straightforward cooperating pieces.
    This rule aims to discourage developers’ affection for writing
    “intricate and beautiful complexities” that are in reality bug prone
    programs.

Rule of Parsimony
:   Developers should avoid writing big programs. This rule aims to
    prevent overinvestment of development time in failed or suboptimal
    approaches caused by the owners of the program’s reluctance to throw
    away visibly large pieces of work. Smaller programs are not only
    easier to write, optimize, and maintain; they are easier to delete
    when deprecated.

Rule of Transparency
:   Developers should design for visibility and discoverability by
    writing in a way that their thought process can lucidly be seen by
    future developers working on the project and using input and output
    formats that make it easy to identify valid input and correct
    output. This rule aims to reduce debugging time and extend the
    lifespan of programs.

Rule of Robustness
:   Developers should design robust programs by designing for
    transparency and discoverability, because code that is easy to
    understand is easier to stress test for unexpected conditions that
    may not be foreseeable in complex programs. This rule aims to help
    developers build robust, reliable products.

Rule of Representation
:   Developers should choose to make data more complicated rather than
    the procedural logic of the program when faced with the choice,
    because it is easier for humans to understand complex data compared
    with complex logic. This rule aims to make programs more readable
    for any developer working on the project, which allows the program
    to be maintained.

Rule of Least Surprise
:   Developers should design programs that build on top of the potential
    users' expected knowledge; for example, ‘+’ in a calculator program
    should always mean 'addition'. This rule aims to encourage
    developers to build intuitive products that are easy to use.

Rule of Silence
:   Developers should design programs so that they do not print
    unnecessary output. This rule aims to allow other programs and
    developers to pick out the information they need from a program's
    output without having to parse verbosity.

Rule of Repair
:   Developers should design programs that fail in a manner that is easy
    to localize and diagnose or in other words “fail noisily”. This rule
    aims to prevent incorrect output from a program from becoming an
    input and corrupting the output of other code undetected.

Rule of Economy
:   Developers should value developer time over machine time, because
    machine cycles today are relatively inexpensive compared to prices
    in the 1970s. This rule aims to reduce development costs of
    projects.

Rule of [Generation](https://en.wikipedia.org/wiki/Generative_programming "Generative programming")
:   Developers should avoid writing code by hand and instead write
    abstract high-level programs that generate code. This rule aims to
    reduce human errors and save time.

Rule of [Optimization](https://en.wikipedia.org/wiki/Optimization_(computer_science) "Optimization (computer science)")
:   Developers should
    [prototype](https://en.wikipedia.org/wiki/Software_prototyping "Software prototyping")
    software before polishing it. This rule aims to prevent developers
    from spending too much time for marginal gains.

Rule of Diversity
:   Developers should design their programs to be flexible and open.
    This rule aims to make programs flexible, allowing them to be used
    in ways other than those their developers intended.

Rule of Extensibility
:   Developers should design for the future by making their protocols
    extensible, allowing for easy plugins without modification to the
    program's architecture by other developers, noting the version of
    the program, and more. This rule aims to extend the lifespan and
    enhance the utility of the code the developer writes.

Mike Gancarz: The UNIX Philosophy[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=7 "Edit section: Mike Gancarz: The UNIX Philosophy")]
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

In 1994, [Mike
Gancarz](https://en.wikipedia.org/w/index.php?title=Mike_Gancarz&action=edit&redlink=1 "Mike Gancarz (page does not exist)")
(a member of the team that designed the [X Window
System](https://en.wikipedia.org/wiki/X_Window_System "X Window System")),
drew on his own experience with Unix, as well as discussions with fellow
programmers and people in other fields who depended on Unix, to produce
*The UNIX Philosophy* which sums it up in 9 paramount precepts:

1.  *Small is beautiful.*
2.  *Make each program do one thing well.*
3.  *Build a prototype as soon as possible.*
4.  *Choose portability over efficiency.*
5.  *Store data in flat [text
    files](https://en.wikipedia.org/wiki/Text_file "Text file").*
6.  *Use software leverage to your advantage.*
7.  *Use [shell
    scripts](https://en.wikipedia.org/wiki/Shell_script "Shell script")
    to increase leverage and portability.*
8.  *Avoid captive user interfaces.*
9.  *Make every program a
    [filter](https://en.wikipedia.org/wiki/Filter_(software)#Unix "Filter (software)").*

"Worse is better"[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=8 "Edit section: "Worse is better"")]
---------------------------------------------------------------------------------------------------------------------------------------------

Main article: [Worse is
better](https://en.wikipedia.org/wiki/Worse_is_better "Worse is better")

[Richard P.
Gabriel](https://en.wikipedia.org/wiki/Richard_P._Gabriel "Richard P. Gabriel")
suggests that a key advantage of Unix was that it embodied a design
philosophy he termed "worse is better", in which simplicity of both the
interface *and* the implementation are more important than any other
attributes of the system—including correctness, consistency, and
completeness. Gabriel argues that this design style has key evolutionary
advantages, though he questions the quality of some results.

For example, in the early days Unix used a [monolithic
kernel](https://en.wikipedia.org/wiki/Monolithic_kernel "Monolithic kernel")
(which means that user processes carried out kernel system calls all on
the user stack). If a signal was delivered to a process while it was
blocked on a long-term
[I/O](https://en.wikipedia.org/wiki/Input/output "Input/output") in the
kernel, then what should be done? Should the signal be delayed, possibly
for a long time (maybe indefinitely) while the I/O completed? The signal
handler could not be executed when the process was in kernel mode, with
sensitive kernel data on the stack. Should the kernel back-out the
system call, and store it, for replay and restart later, assuming that
the signal handler completes successfully?

In these cases [Ken
Thompson](https://en.wikipedia.org/wiki/Ken_Thompson_(computer_programmer) "Ken Thompson (computer programmer)")
and [Dennis
Ritchie](https://en.wikipedia.org/wiki/Dennis_Ritchie "Dennis Ritchie")
favored simplicity over perfection. The Unix system would occasionally
return early from a system call with an error stating that it had done
nothing—the "Interrupted System Call", or an error number 4 (`EINTR`) in
today's systems. Of course the call had been aborted in order to call
the signal handler. This could only happen for a handful of long-running
system calls such as `read()`, `write()`, `open()`, and `select()`. On
the plus side, this made the I/O system many times simpler to design and
understand. The vast majority of user programs were never affected
because they didn't handle or experience signals other than `SIGINT` and
would die right away if one was raised. For the few other
programs—things like shells or text editors that respond to job control
key presses—small wrappers could be added to system calls so as to retry
the call right away if this `EINTR` error was raised. Thus, the problem
was solved in a simple manner.

See also[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=9 "Edit section: See also")]
---------------------------------------------------------------------------------------------------------------------------

-   [Cognitive
    engineering](https://en.wikipedia.org/wiki/Cognitive_engineering "Cognitive engineering")
-   [Unix
    architecture](https://en.wikipedia.org/wiki/Unix_architecture "Unix architecture")
-   [Minimalism
    (computing)](https://en.wikipedia.org/wiki/Minimalism_(computing) "Minimalism (computing)")
-   [Software
    engineering](https://en.wikipedia.org/wiki/Software_engineering "Software engineering")
-   [Hacker
    ethic](https://en.wikipedia.org/wiki/Hacker_ethic "Hacker ethic")
-   [List of software development
    philosophies](https://en.wikipedia.org/wiki/List_of_software_development_philosophies "List of software development philosophies")

Notes[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=10 "Edit section: Notes")]
----------------------------------------------------------------------------------------------------------------------

1.  \^ [Jump up to:
    ^***a***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-taoup-ch1s6_1-0)
    [^***b***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-taoup-ch1s6_1-1)
    [^***c***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-taoup-ch1s6_1-2)
    [^***d***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-taoup-ch1s6_1-3)
    [^***e***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-taoup-ch1s6_1-4)
    [Raymond, Eric
    S.](https://en.wikipedia.org/wiki/Eric_S._Raymond "Eric S. Raymond")
    (2003-09-23). ["Basics of the Unix
    Philosophy"](http://www.catb.org/~esr/writings/taoup/html/ch01s06.html).
    [*The Art of Unix
    Programming*](http://www.catb.org/~esr/writings/taoup/html/).
    Addison-Wesley Professional.
    [ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number") [0-13-142901-9](https://en.wikipedia.org/wiki/Special:BookSources/0-13-142901-9 "Special:BookSources/0-13-142901-9").
    Retrieved 2016-11-01. 
2.  **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-2)**
    [Doug
    McIlroy](https://en.wikipedia.org/wiki/Doug_McIlroy "Doug McIlroy"),
    E. N. Pinson, B. A. Tague (8 July 1978). ["Unix Time-Sharing System:
    Foreword"](http://emulator.pdp-11.org.ru/misc/1978.07_-_Bell_System_Technical_Journal.pdf)
    (PDF). *The Bell System Technical Journal*. Bell Laboratories.
    pp. 1902–1903. CS1 maint: Multiple names: authors list
    ([link](https://en.wikipedia.org/wiki/Category:CS1_maint:_Multiple_names:_authors_list "Category:CS1 maint: Multiple names: authors list"))
3.  **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-3)**
    Andrew Hunt; David Thomas (1999). ["The Pragmatic Programmer: From
    Journeyman to
    Master"](https://books.google.com/books?id=5wBQEp6ruIAC&pg=PA76). 
4.  \^ [Jump up to:
    ^***a***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-interview_4-0)
    [^***b***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-interview_4-1)
    ["Joseph H.
    Condon"](https://www.princeton.edu/~hos/mike/transcripts/condon.htm).
    [Princeton
    University](https://en.wikipedia.org/wiki/Princeton_University "Princeton University")
    History of Science. 
5.  **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-reader_5-0)**
    [McIlroy, M.
    D.](https://en.wikipedia.org/wiki/Doug_McIlroy "Doug McIlroy")
    (1987). [*A Research Unix reader: annotated excerpts from the
    Programmer's Manual,
    1971–1986*](http://www.cs.dartmouth.edu/~doug/reader.pdf) (PDF)
    (Technical report). CSTR. Bell Labs. 139. 
6.  **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-6)**
    Norman, Don (1981). ["The truth about Unix: The user interface is
    horrid"](http://www.bradleymonk.com/File:The_truth_about_Unix_Don_Norman.pdf)
    (PDF). *Datamation* (27(12)). 
7.  \^ [Jump up to:
    ^***a***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-unix1984_7-0)
    [^***b***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-unix1984_7-1)
    Kernighan, Brian W. Pike, Rob. *The UNIX Programming Environment.*
    1984. viii
8.  \^ [Jump up to:
    ^***a***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-design1984_8-0)
    [^***b***^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-design1984_8-1)
    Rob Pike; Brian W. Kernighan (October 1984). ["Program Design in the
    UNIX
    Environment"](http://harmful.cat-v.org/cat-v/unix_prog_design.pdf)
    (PDF). 
9.  **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-9)**
    [http://cm.bell-labs.com/cm/cs/who/dmr/mdmpipe.html](http://cm.bell-labs.com/cm/cs/who/dmr/mdmpipe.html)
10. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-10)**
    Douglas McIlroy. ["Remarks for Japan Prize award ceremony for Dennis
    Ritchie, May 19, 2011, Murray Hill,
    NJ"](http://www.cs.dartmouth.edu/~doug/dmr.pdf) (PDF). Retrieved
    2014-06-19. 
11. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-11)**
    Bill McGonigle. ["Ancestry of Linux — How the Fun Began
    (2005)"](https://archive.org/details/DougMcIlroy_AncestryOfLinux_DLSLUG).
    Retrieved 2014-06-19. 
12. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-12)**
    Varghese, Sam. ["Systemd fallout: Two Debian technical panel members
    resign"](http://www.itwire.com/business-it-news/open-source/66153-systemd-fallout-two-debian-technical-panel-members-resign/).
    ITWire. Retrieved 2015-03-31. 
13. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-volkerding-2012_13-0)**
    ["Interview with Patrick Volkerding of
    Slackware"](http://www.linuxquestions.org/questions/interviews-28/interview-with-patrick-volkerding-of-slackware-949029/).
    *linuxquestions.org*. 2012-06-07. Retrieved 2015-10-24. 
14. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-14)**
    [Raymond,
    Eric](https://en.wikipedia.org/wiki/Eric_S._Raymond "Eric S. Raymond")
    (2003-09-19). [*The Art of Unix
    Programming*](http://www.catb.org/~esr/writings/taoup/html/).
    Addison-Wesley.
    [ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number") [0-13-142901-9](https://en.wikipedia.org/wiki/Special:BookSources/0-13-142901-9 "Special:BookSources/0-13-142901-9").
    Retrieved 2009-02-09. 
15. **[Jump up
    \^](https://en.wikipedia.org/wiki/Unix_philosophy#cite_ref-15)**
    [Raymond,
    Eric](https://en.wikipedia.org/wiki/Eric_S._Raymond "Eric S. Raymond")
    (2003-09-19). ["The Unix Philosophy in One
    Lesson"](http://www.catb.org/~esr/writings/taoup/html/ch01s07.html).
    [*The Art of Unix
    Programming*](http://www.catb.org/~esr/writings/taoup/html/).
    Addison-Wesley.
    [ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number") [0-13-142901-9](https://en.wikipedia.org/wiki/Special:BookSources/0-13-142901-9 "Special:BookSources/0-13-142901-9").
    Retrieved 2009-02-09. 

References[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=11 "Edit section: References")]
--------------------------------------------------------------------------------------------------------------------------------

-   *[The Unix Programming
    Environment](http://cm.bell-labs.com/cm/cs/upe/)* by [Brian
    Kernighan](https://en.wikipedia.org/wiki/Brian_Kernighan "Brian Kernighan")
    and [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike "Rob Pike"),
    1984
-   *[Program Design in the UNIX
    Environment](http://harmful.cat-v.org/cat-v/)* – The paper by Pike
    and Kernighan that preceded the book.
-   [*Notes on Programming in
    C*](http://doc.cat-v.org/bell_labs/pikestyle), Rob Pike, September
    21, 1989
-   *A Quarter Century of Unix*, Peter H. Salus, Addison-Wesley, May 31,
    1994
    ([ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number")
    [0-201-54777-5](https://en.wikipedia.org/wiki/Special:BookSources/0-201-54777-5 "Special:BookSources/0-201-54777-5"))
-   [*Philosophy*](http://www.faqs.org/docs/artu/philosophychapter.html) —
    from [*The Art of Unix
    Programming*](http://www.catb.org/~esr/writings/taoup), Eric S.
    Raymond, Addison-Wesley, September 17, 2003
    ([ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number")
    [0-13-142901-9](https://en.wikipedia.org/wiki/Special:BookSources/0-13-142901-9 "Special:BookSources/0-13-142901-9"))
-   [Final Report of the Multics Kernel Design
    Project](http://citeseer.ist.psu.edu/schroeder77final.html) by M. D.
    Schroeder, D. D. Clark, J. H. Saltzer, and D. H. Wells, 1977.
-   *The UNIX Philosophy*, Mike Gancarz,
    [ISBN](https://en.wikipedia.org/wiki/International_Standard_Book_Number "International Standard Book Number")
    [1-55558-123-4](https://en.wikipedia.org/wiki/Special:BookSources/1-55558-123-4 "Special:BookSources/1-55558-123-4")

External links[[edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit&section=12 "Edit section: External links")]
----------------------------------------------------------------------------------------------------------------------------------------

-   [Basics of the Unix
    Philosophy](http://www.catb.org/esr/writings/taoup/html/ch01s06.html)
    – by Catb.org
-   [The Unix Philosophy: A Brief
    Introduction](http://www.linfo.org/unix_philosophy.html) – by The
    Linux Information Project (LINFO)
-   [The Unix
    Philosophy](http://hebb.cis.uoguelph.ca/~dave/27320/new/unixphil.html)
-   [Why the Unix Philosophy still
    matters](http://marmaro.de/docs/studium/unix-phil/unix-phil.pdf)

\<img
src="//en.wikipedia.org/wiki/Special:CentralAutoLogin/start?type=1x1"
alt="" title="" width="1" height="1" style="border: none; position:
absolute;" /\>

Retrieved from
"[https://en.wikipedia.org/w/index.php?title=Unix\_philosophy&oldid=791861823](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&oldid=791861823)"

[Categories](https://en.wikipedia.org/wiki/Help:Category "Help:Category"):

-   [Software development
    philosophies](https://en.wikipedia.org/wiki/Category:Software_development_philosophies "Category:Software development philosophies")
-   [Unix](https://en.wikipedia.org/wiki/Category:Unix "Category:Unix")

Hidden categories:

-   [CS1 maint: Multiple names: authors
    list](https://en.wikipedia.org/wiki/Category:CS1_maint:_Multiple_names:_authors_list "Category:CS1 maint: Multiple names: authors list")

Navigation menu
---------------

### Personal tools {#p-personal-label}

-   Not logged in
-   [Talk](https://en.wikipedia.org/wiki/Special:MyTalk "Discussion about edits from this IP address [alt-shift-n]")
-   [Contributions](https://en.wikipedia.org/wiki/Special:MyContributions "A list of edits made from this IP address [alt-shift-y]")
-   [Create
    account](https://en.wikipedia.org/w/index.php?title=Special:CreateAccount&returnto=Unix+philosophy "You are encouraged to create an account and log in; however, it is not mandatory")
-   [Log
    in](https://en.wikipedia.org/w/index.php?title=Special:UserLogin&returnto=Unix+philosophy "You're encouraged to log in; however, it's not mandatory. [alt-shift-o]")

### Namespaces {#p-namespaces-label}

-   [Article](https://en.wikipedia.org/wiki/Unix_philosophy "View the content page [alt-shift-c]")
-   [Talk](https://en.wikipedia.org/wiki/Talk:Unix_philosophy "Discussion about the content page [alt-shift-t]")

### Variants {#p-variants-label tabindex="0"}

### Views {#p-views-label}

-   [Read](https://en.wikipedia.org/wiki/Unix_philosophy)
-   [Edit](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=edit "Edit this page [alt-shift-e]")
-   [View
    history](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=history "Past revisions of this page [alt-shift-h]")

### More {#p-cactions-label tabindex="0"}

### Search

[](https://en.wikipedia.org/wiki/Main_Page "Visit the main page")

### Navigation {#p-navigation-label}

-   [Main
    page](https://en.wikipedia.org/wiki/Main_Page "Visit the main page [alt-shift-z]")
-   [Contents](https://en.wikipedia.org/wiki/Portal:Contents "Guides to browsing Wikipedia")
-   [Featured
    content](https://en.wikipedia.org/wiki/Portal:Featured_content "Featured content – the best of Wikipedia")
-   [Current
    events](https://en.wikipedia.org/wiki/Portal:Current_events "Find background information on current events")
-   [Random
    article](https://en.wikipedia.org/wiki/Special:Random "Load a random article [alt-shift-x]")
-   [Donate to
    Wikipedia](https://donate.wikimedia.org/wiki/Special:FundraiserRedirector?utm_source=donate&utm_medium=sidebar&utm_campaign=C13_en.wikipedia.org&uselang=en "Support us")
-   [Wikipedia
    store](https://shop.wikimedia.org/ "Visit the Wikipedia store")

### Interaction {#p-interaction-label}

-   [Help](https://en.wikipedia.org/wiki/Help:Contents "Guidance on how to use and edit Wikipedia")
-   [About
    Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:About "Find out about Wikipedia")
-   [Community
    portal](https://en.wikipedia.org/wiki/Wikipedia:Community_portal "About the project, what you can do, where to find things")
-   [Recent
    changes](https://en.wikipedia.org/wiki/Special:RecentChanges "A list of recent changes in the wiki [alt-shift-r]")
-   [Contact
    page](https://en.wikipedia.org/wiki/Wikipedia:Contact_us "How to contact Wikipedia")

### Tools {#p-tb-label}

-   [What links
    here](https://en.wikipedia.org/wiki/Special:WhatLinksHere/Unix_philosophy "List of all English Wikipedia pages containing links to this page [alt-shift-j]")
-   [Related
    changes](https://en.wikipedia.org/wiki/Special:RecentChangesLinked/Unix_philosophy "Recent changes in pages linked from this page [alt-shift-k]")
-   [Upload
    file](https://en.wikipedia.org/wiki/Wikipedia:File_Upload_Wizard "Upload files [alt-shift-u]")
-   [Special
    pages](https://en.wikipedia.org/wiki/Special:SpecialPages "A list of all special pages [alt-shift-q]")
-   [Permanent
    link](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&oldid=791861823 "Permanent link to this revision of the page")
-   [Page
    information](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&action=info "More information about this page")
-   [Wikidata
    item](https://www.wikidata.org/wiki/Special:EntityPage/Q14652 "Link to connected data repository item [alt-shift-g]")
-   [Cite this
    page](https://en.wikipedia.org/w/index.php?title=Special:CiteThisPage&page=Unix_philosophy&id=791861823 "Information on how to cite this page")

### Print/export {#p-coll-print_export-label}

-   [Create a
    book](https://en.wikipedia.org/w/index.php?title=Special:Book&bookcmd=book_creator&referer=Unix+philosophy)
-   [Download as
    PDF](https://en.wikipedia.org/w/index.php?title=Special:ElectronPdf&page=Unix+philosophy&action=show-selection-screen&coll-download-url=%2Fw%2Findex.php%3Ftitle%3DSpecial%3ABook%26bookcmd%3Drender_article%26arttitle%3DUnix%2Bphilosophy%26returnto%3DUnix%2Bphilosophy%26oldid%3D791861823%26writer%3Drdf2latex)
-   [Printable
    version](https://en.wikipedia.org/w/index.php?title=Unix_philosophy&printable=yes "Printable version of this page [alt-shift-p]")

### Languages {#p-lang-label}

-   [العربية](https://ar.wikipedia.org/wiki/%D9%81%D9%84%D8%B3%D9%81%D8%A9_%D9%8A%D9%88%D9%86%D9%83%D8%B3 "فلسفة يونكس – Arabic")
-   [Čeština](https://cs.wikipedia.org/wiki/Filosofie_Unixu "Filosofie Unixu – Czech")
-   [Deutsch](https://de.wikipedia.org/wiki/Unix-Philosophie "Unix-Philosophie – German")
-   [فارسی](https://fa.wikipedia.org/wiki/%D9%81%D9%84%D8%B3%D9%81%D9%87_%DB%8C%D9%88%D9%86%DB%8C%DA%A9%D8%B3 "فلسفه یونیکس – Persian")
-   [Français](https://fr.wikipedia.org/wiki/Philosophie_d%27Unix "Philosophie d'Unix – French")
-   [한국어](https://ko.wikipedia.org/wiki/%EC%9C%A0%EB%8B%89%EC%8A%A4_%EC%B2%A0%ED%95%99 "유닉스 철학 – Korean")
-   [Italiano](https://it.wikipedia.org/wiki/Filosofia_Unix "Filosofia Unix – Italian")
-   [日本語](https://ja.wikipedia.org/wiki/UNIX%E5%93%B2%E5%AD%A6 "UNIX哲学 – Japanese")
-   [Norsk
    bokmål](https://no.wikipedia.org/wiki/Unix-filosofien "Unix-filosofien – Norwegian")
-   [Português](https://pt.wikipedia.org/wiki/Filosofia_Unix "Filosofia Unix – Portuguese")
-   [Русский](https://ru.wikipedia.org/wiki/%D0%A4%D0%B8%D0%BB%D0%BE%D1%81%D0%BE%D1%84%D0%B8%D1%8F_UNIX "Философия UNIX – Russian")
-   [中文](https://zh.wikipedia.org/wiki/Unix%E5%93%B2%E5%AD%A6 "Unix哲学 – Chinese")

[Edit
links](https://www.wikidata.org/wiki/Special:EntityPage/Q14652#sitelinks-wikipedia "Edit interlanguage links")

-   This page was last edited on 22 July 2017, at 23:15.
-   Text is available under the [Creative Commons Attribution-ShareAlike
    License](https://en.wikipedia.org/wiki/Wikipedia:Text_of_Creative_Commons_Attribution-ShareAlike_3.0_Unported_License)[](https://creativecommons.org/licenses/by-sa/3.0/);
    additional terms may apply. By using this site, you agree to the
    [Terms of Use](https://wikimediafoundation.org/wiki/Terms_of_Use)
    and [Privacy
    Policy](https://wikimediafoundation.org/wiki/Privacy_policy).
    Wikipedia® is a registered trademark of the [Wikimedia Foundation,
    Inc.](https://www.wikimediafoundation.org/), a non-profit
    organization.

-   [Privacy
    policy](https://wikimediafoundation.org/wiki/Privacy_policy "wmf:Privacy policy")
-   [About
    Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:About "Wikipedia:About")
-   [Disclaimers](https://en.wikipedia.org/wiki/Wikipedia:General_disclaimer "Wikipedia:General disclaimer")
-   [Contact
    Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Contact_us)
-   [Developers](https://www.mediawiki.org/wiki/Special:MyLanguage/How_to_contribute)
-   [Cookie
    statement](https://wikimediafoundation.org/wiki/Cookie_statement)
-   [Mobile
    view](https://en.m.wikipedia.org/w/index.php?title=Unix_philosophy&mobileaction=toggle_view_mobile)

-   [![Wikimedia
    Foundation](./Unix%20philosophy%20-%20Wikipedia_files/wikimedia-button.png)](https://wikimediafoundation.org/)
-   [![Powered by
    MediaWiki](./Unix%20philosophy%20-%20Wikipedia_files/poweredby_mediawiki_88x31.png)](https://www.mediawiki.org/)

[](https://en.wikipedia.org/wiki/Unix_philosophy?action=edit)
