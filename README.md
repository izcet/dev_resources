# dev_resources
A collection of links that I've personally found useful,
  organized for a fellow developer.
I tried to keep this more as a collection of resources,
  but I did also include some opinion-based tips and comments.
Note that this is largely backend and security-focused,
  though the early fundamentals will be valuable regardless of domain.

## bash and linux essentials
_This section covers some of the bare fundamentals of interacting with a Linux/Unix
shell. While not strictly necesary for programming in itself, you will need to know
how to interact with the computer directly via a terminal interface. The links here
approach the domain from different perspectives, so if one isn't working feel free
to skip around -- they're in no real order, though if you're brand new I would 
recommend starting with the first two._
- [Cisco Linux Essentials](https://www.netacad.com/courses/ndg-linux-essentials/):
  Provides a more classroom style approach with an online course you can complete 
  at your own speed. Effectively explains licensing (_yawn_) and more linux /
  sysadmin relevant commands (`tar`, `gzip`, `bzip2`, `cron`, etc), the different
  shells (`sh`, `bash`, etc) and how to switch them. User management and other system
  utilities, shell expansion and redirection (`*` `>` `|` `&` `;`, etc).
  This will very likely be overkill for what you'll eventually do day-to-day, but
  the sandbox environment it provides and gradual explanation and build-up of terminal
  skills will help immensely.
- [Git]: I have to admit, I learned this entirely from using it in a peer-to-peer
  environment and at work, so I don't have a resource I can just point to. However,
  this is one of the most important things on this list (maybe worth a whole section
  later when I update this again), so definitely take the time to wrap your head around
  it. My 2 cents:
  - Start with the command line. Graphical tools and other programs hide too much
    and you'll have no idea what's really going on under the hood.
  - Create a GitHub/GitLab account, and play around with copying (`git clone`),
    creating (`git init`), revising (`git add` / `git commit`) and updating (`git push`).
    `man git` is useful, but subcommands are more useful (`man git-commit`, for example).
  - All the commands I listed above will be your day-to-day, once you really get into
    the swing, you'll pick up `merge`, `cherrypick`, `rebase`, `log`, etc on your own
    time, when you need to.
- [CommandLine Challenge](https://cmdchallenge.com/): A Set of puzzles that don't
  provide any explanation or instruction, you just have to research the solution yourself.
  (I personally got bored before I finished, but I'll get back to it eventually:tm:)
- [HackerRank Bash](https://www.hackerrank.com/domains/shell/bash): Provides
  incremental, easily digestible challenges that you can complete in a day to
  get up-to-speed with a few of the main commands you'll use in day-to-day
  \*nix system administration, debugging, and shell scripts.
  (`cut`, `tr`, `sort`, `uniq`, `grep`, `sed`, `awk`)
- This [site](http://www.tldp.org/LDP/Bash-Beginners-Guide/html/) has everything
  you'll ever want to look up with bash scripting. I use it more as an occasional
  reference rather than cover to cover reading.
- Stack Overflow, Google, and `man` are all your friends and highly encouraged.
- If you're going to get deeper into shell scripting, some other miscellaneous tools
  are `expect`, `head`, `less`, `cat`, `at`, `diff`, `xargs`,`screen`,
  [escape codes](http://ascii-table.com/ansi-escape-sequences.php), 
  `ps`, `[h]top`, `find`, `kill`.

## Regex 
_This is a domain-specific expression language for pattern-matching and text
  manipulation. It will be useful for complex searches, text substitution, and
  ensuring arbitrary strings follow a given format._
- [HackerRank Regex](https://www.hackerrank.com/domains/regex/re-introduction):
  Really good at providing small, easy to pick up and solve puzzles that progessively
  build off each other.
- [Rexexr](https://regexr.com/): A useful site for live testing your pattern against
  input text to see what's matching and why.
- Learn this! It supplements searching with `grep`, modifying with `sed` (both in the
  shell and also in `vim` replace)

## shell exploits, cryptography and crack-mes
- [Over the Wire](http://overthewire.org/wargames/): Hack this Site! Teaches you
  stuff in a fun, challenging environment. Start with bandit, then play with
  Natas, etc. You'll figure it out.
- [Applied Cryptography](https://www.schneier.com/blog/archives/2014/01/applied_cryptog_1.html)
  is The Book when it comes to learning cryptographic principles, concepts and usage.
  The intro alone is worth reading to get an understanding of how the stuff is used,
  even if you don't get deep into the bits of it.
- There's still [more](https://radare.gitbooks.io/radare2book/content/crackmes/intro.html)
  I [want](https://trailofbits.github.io/ctf/)
  [to](https://microcorruption.com/login)
  [do](http://smashthestack.org/)
  even though I'm not done with Over the Wire.

## GitHub Student Developer Pack
_The contents of this section are subject to change based on what is offered
  by github, and I will not update this every time that changes. I have some
  suggesstions listed, though your mileage may vary._
- Sign up with your college email, if possible.
- Get it [here](https://education.github.com/pack)
  - DigitalOcean for almost a year on their minimum plan.
    Good for putting up a web server, and using it to proxy and learn `ssh`
    (learn why and how to use keys instead of passwords)
  - Free private repositories at github.com
  - Free domain at NameCheap (that you can use with DigitalOcean), plus they've
    got some cheap names.
  - SendGrid free e-mailing api (for sending mass emails from script)

## Programming Languages
_This is a very broad subject with a lot of angles that I'll try to summarize
  neatly into 3 sections. The first will be some background on the concept and
  implementation of languages themselves, the second will have learning materials,
  and the third will be my own experience and notes based on working in those
  languages, in chronological order from when I learned them._
#### Background
- [This video](https://www.youtube.com/watch?v=duhDovqHbEs) is aimed at total
  beginners and explains the concept of programming languages, and the common
  features among them. (Also for beginners, his 
  [hardware](https://www.youtube.com/watch?v=9-KUm9YpPm0) and
  [operating system](https://www.youtube.com/watch?v=9GDX-IyZ_C8) intros
  also helpful for abstract background. The rest of his videos can get very
  technical or political, such as his "OOP is bad" series. Those still have
  value, but I recommend coming back to them once you havehave more
  practical context first)
- There are multiple facets by which languages are grouped, such as wether
  they are _compiled_ or _interpreted_, or if the paradigm is _imperative_,
  _procedural_, _object-oriented_, _functional_, or a blend. Understanding the
  differences between these categories is highly valuable, though debates
  on which style is "best" tend to be highly polarized and largely academic.
  Though any language can be used for any task, each tends to have a domain
  over which it outperforms the rest, for a myriad of reasons.
- The first language anyone learns depends on the domain they aim for first.
  For academics learning in a classroom, it may have been Java, C or Lisp.
  For self-taught web developers, it's more likely to be HTML (some argue
  it's not a programming language, though we won't get into that here),
  JavaScript, or Ruby. For example, I first learned a mix of Imperative and
  OOP in a classroom via Java in the BlueJ IDE, then expanded that knowledge
  with imperative C written in `vim`. In my opinion, learning a more primitive
  (c-like) language helps grasp overall program structure, and modern
  programming styles (functional) build neatly on-top of that foundation.
#### Reference
- [Learn X in Y](https://learnxinyminutes.com/) is the best thing ever made.
  Once you've really mastered one or two languages under your belt, you can
  use this as a supplement to the documentation of any language you want to
  learn in the future.

#### Hot Takes
- **Java**:
  - [++Object Oriented, +Imperative]
    [compiled to jvm bytecode]
  - it was originally invented to steal C programmers so the syntax is similar
  - it's a very good first language because it runs in a garbage-collecting VM,
    which means you don't have to worry about the added complexity of manual
    memory management.
  - in production, it becomes very bloated with enterprise-driven boilerplate
    and arbitrary constructors and interfaces
  - it's pretty ugly and slimey. Though I find it easy to work with because
    of how straightforward it tends to be, this is not my language of choice.
  - bonus: the JVM bytecode can be directly decompiled, so it's great for
    reverse engineering!

- **C**:
  - [+Imperative, +Procedural] 
    [compiled to machine-readable executable]
  - cons: it is very easy to shoot yourself in the foot
  - pros: you get to learn how to shoot yourself in the foot in new,
    exciting and creative ways
  - of the high-level languages, by today's standards it is considered low level.
  - used for systems engineering, linux kernel code, things which require
    extreme efficiency
  - fastest runtime of any language because it's compiled to native code
  - you will need to know how to read this for reverse engineering
  - honestly one of my all-time favorites

- **Python**:
  - [+Imperative, +Procedural]
    [interpreted, but newer versions support an optimized compilation]
  - can support OOP concepts but not its main calling card
  - can be used for simple scripts just as easily as full programs
  - very easy
  - next-to-english in terms of high level readability and syntax
  - great for quick scripting, research, and math/sciencey stuff
  - very slow runtime compared to other languages
  - can have a lot of package dependency confusion and environment variables
    you have to juggle
  - easier to use within a virtual environment (`virtualenv`)
  - used a lot in machine learning
  - also used a lot in security for rapid prototyping of Proof of Concept hacks

- **Assembly**
  - [++Imperative]
  - note: I used an x86 dialect of RedCode for a competition, so while
    I've written ASM code, it wasn't for a fully independent program.
  - the lowest level you could reasonably write by hand
  - useful for academic purposes, or if you're writing absurdly low-level code
  - can be fun and self-modifying

- **C++**:
  - [++Object Oriented, +Procedural]
    [compiled]
  - C with benefits
  - to-the-metal C speed with a lot of OOP abstraction provided
  - very verbose and heavy code (but still something you'd be comfortable with
    if you come from C)

- **Go**:
  - [+Procedural]
    [compiled]
  - has OOP concepts, but doesn't shove them down your throat like Java or C++
  - Very natural and easy, good for networked/distributed/threaded and web
  - Has nil to no graphics support
  - Comes with the GoTour - a built-in tutuorial for the language

- **Scala**:
  - [+Functional, +Procedural, +Object Oriented]
    [compiled to jvm bytecode]
  - significantly more fun to write than Java for JVM code
  - FP forces you to write code in a cleaner, type-safe way. It can be difficult
    to wrap your head around, but it's worth learning on its own merit once
    you've mastered imperative styles.
  - Scala also breaks away from FP and allows you to cheat when OOP or imperative
    code would be more effective.

- **Honorable Mentions**:
  - I don't have enough personal experience to explain pros/cons outside of hearsay.
  - On my own To-Do list to learn
  - JavaScript -- runs literally everywhere on the internet. 
  - Purer Functional Programming languages, like Haskell.
  - Ruby -- I found this enjoyable to program in when I dabbled, but haven't used it
    enough to give a more thorough review.
  - Prolog -- not a conventional programming language, but a more abstract pure
    logic resolver.
  - Erlang

## Random Notes
- Don't use an IDE! Start with `vim` (or `emacs`) and really get comfortable with
  customizing/navigating and using it. Your friends will write code faster than
  you at first, but you'll soon find yourself having a deeper understanding
  and ability to code than those that handicap themselves with conveneince. Use
  an IDE when you start a professional job and surprise yourself with how much
  faster you can code.
- I recommend `vim` because it's preinstalled on all linux machines, useful for
  system recovery. It's great over `ssh` or if you switch machines often.
  (Emacs is useful for someone who wants to take their time to really set up their
  development environment for one machine, and let the investment of the large
  up-front customization pay off later on.)
- use LUKS to encrypt your hard drive on a Linux machine
- Use [Open](https://libreboot.org/faq.html) [Source](https://www.coreboot.org/)
  boot loaders!
- VPNs [are](https://openvpn.net/)
  [cool](https://www.wireguard.com/)
  too
- Become a [Programmer, Motherfucker](http://programming-motherfucker.com/become.html)
- `lldb` `valgrind` `hashcat` `wireshark` `nmap` `htop`, 
  Hopper, radare2, IDA, VMWare Fusion, Docker.

## Offtopic / Aesthetic
- [N-O-D-E](https://n-o-d-e.net/) is cool.
- [Rainy mood](http://www.rainymood.com/): Good background noise, helps me focus.
- [KeyBr](https://www.keybr.com/): Helps provide statistics on typing, and it's
  always good to practice.
- [Tomato Timer](https://tomato-timer.com/): Pomodoro Techniques are useful for
  maximimzing productive time and avoiding burnout.
- [Code Fights](https://codefights.com/): Even though they try to provide
  challenges like HackerRank, I don't consider this a reference for
  problem-solving and learning, rather for speed practice and competetition vs
  friends/strangers.
- [Secure Code Warrior](https://www.securecodewarrior.com/): Right now it seems they
  only offer their "courses" B2B, so you'd have to get your employer to pay for
  your course. All in all I think the platform itself is pretty immature, but
  this has potential and the material is valuable.
