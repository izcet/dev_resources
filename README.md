# dev_resources
A collection of links that I've personally found useful, organized for a fellow developer.  
I tried to keep this more as a collection of resources, but I did also include some opinion-based tips and comments.

## bash and deep linux essentials
- [HackerRank Bash](https://www.hackerrank.com/domains/shell/bash): Provides incremental, easily digestible challenges that you can complete in a day to get up-to-speed with a few of the main commands you'll use (`cut`, `tr`, `sort`, `uniq`, `grep`, `sed`, `awk`)
- [Cisco Linux Essentials](https://www.netacad.com/courses/ndg-linux-essentials/): Provides a more classroom style approach with an online course you can compete at your own speed. Effectively explains licensing (_yawn_) and more linux / sysadmin relevant commands (_ooh_) (`tar`, `gzip`, `bzip2`, `cron` I think), the different shells (`sh`, `bash`, etc) and how to switch them. User management and other system utilities. Shell expansion and redirection I think (`*` `>` `|` `&` `;`, etc)
- [CommandLine Challenge](https://cmdchallenge.com/): A Set of puzzles that don't provide any explanation or instruction, just puzzles that you have to research the solution to yourself. (I personally got bored before I finished, but I'll get back to it eventually)
- This [site](http://www.tldp.org/LDP/Bash-Beginners-Guide/html/) has everything you'll ever want to look up with bash scripting. I use it more for reference rather than reading it cover to cover.
- Stack Overflow, Google, and `man` are all your friends and highly encouraged.
- Other bash tools worth learning are: `expect`, `head`, `less`, `cat`, `at`, `screen`, [escape codes](http://ascii-table.com/ansi-escape-sequences.php), _really_ understanding all the redirection, suspension, `ps`, `top`, `find`, `kill`. Start with the above and check back with these if any were missed.

## Regex 
- [HackerRank Regex](https://www.hackerrank.com/domains/regex/re-introduction): Really good at providing small, easy to pick up and solve puzzles that progressively build off each other.
- [Rexexr](https://regexr.com/): A useful site for live testing your pattern against input text to see what's matching and why.
- Learn this! It makes searching with `grep`, modifying with `sed` (both in the shell and also in `vim` replace)

## shell exploits, cryptography and crack-mes
- [Over the Wire](http://overthewire.org/wargames/): Hack this Site! Teaches you stuff in a fun, challenging environment. Start with bandit, then play with Natas, etc. You'll figure it out.
- [Applied Cryptography](https://www.schneier.com/blog/archives/2014/01/applied_cryptog_1.html) is The Book when it comes to learning cryptographic principles, concepts and usage. The intro alone is worth reading to get an understanding of how the stuff is used even if you don't get deep into the bits of it.
- There's still [more](https://radare.gitbooks.io/radare2book/content/crackmes/intro.html)
I [want](https://trailofbits.github.io/ctf/)
[to](https://microcorruption.com/login)
[do](http://smashthestack.org/)
even though I'm not done with Over the Wire.

## GitHub Student Developer Pack
- Sign up with yourlogin@student.42.us.org 
(emails sent to that domain will be forwarded to the email you used to sign up at 42)
- Get it [here](https://education.github.com/pack)
  - DigitalOcean for almost a year on their minimum plan. 
  Good for putting up a web server, and using it to proxy and learn `ssh` 
  (learn why and how to use keys instead of passwords)
  - Free private repositories at github.com
  - Free domain at NameCheap (that you can use with DigitalOcean), plus they've got some cheap names.
  - SendGrid free e-mailing api (for sending mass emails from script)

## Languages other than C
- [Learn X in Y](https://learnxinyminutes.com/) is the best thing ever made.
- Coming from C, you'll be able to pick up most of these pretty easy
- My recommendations: stick with C and Bash at first, and get really comfortable with the bare metal environment and execution.

- **Java**:
  - has a very C-like syntax 
  - has high-level OOP functionality
  - can be bloated and slimey
  - bonus: java bytecode can be directly decompiled back to source, great for reverse engineering!

- **C++**: 
  - Pick up at level 7 with the CPP piscine ASAP
  - C with benefits
  - To-the-metal C speed with a lot of OOP abstraction provided
  - Very verbose and heavy code (but still something you'd be comfortable with coming from C)

- **Go**:
  - Has close to C-like syntax
  - has OOP concepts, but doesn't shove them down your throat like Java or C++
  - Very natural and easy, good for networked/distributed/threaded and web
  - Has nil to no graphics support
  - Comes with the GoTour - a built-in tutuorial for the language

- **Python**:
  - Pick up around level 5 (even though you can probably grok it sooner)
  - Can support OOP concepts but not its main calling card
  - Can be used for simple scripts just as easily as full programs
  - Very easy
  - Very easy
  - Next-to-english in terms of high level readability and syntax
  - Great for quick scripting and math/sciencey stuff
  - Code execution is interpreted not compiled (very slow compared to other languages) (like bash)
  - Can have a lot of package dependency confusion and environment variables you have to juggle. Sometimes easier inside its own VM
  - Used a lot in machine learning
  - also used a lot in security for networked penetration testing because it's quick to deploy

- **Honorable Mentions**:
  - I don't have enough personal experience to explain pros/cons outside of hearsay
  - On my own To-Do list to learn
  - JavaScript - runs literally everywhere on the internet. 
  - Functional Programming languages like Haskell and Scala
  - Perl - an elegant language, somewhere between C and bash

## Non Technical Resources
- [Rainy mood](http://www.rainymood.com/): Good background noise, helps me focus.
- [KeyBr](https://www.keybr.com/): Helps provide statistics on typing, and it's always good to practice.
- [Tomato Timer](https://tomato-timer.com/): Pomodoro Techniques are useful for maximimzing productive time and avoiding burnout.
- [Code Fights](https://codefights.com/): Even though they try to provide challenges like HackerRank, I don't consider this a reference for problem-solving and learning, rather for speed practice and competetition vs friends/strangers.

## Random Notes
Someone once said to me that you should host your computers in Amsterdam because they have really good privacy laws,
and proxy your connections through Russia because they won't comply with US disclosure requests. Or something.
- Don't use an IDE! Start with `vim` (or `emacs`) and really get comfortable with customizing/navigating and using it. Your friends will write code faster than you at first, but you'll soon find yourself having a deeper understanding and ability to code than those that handicap themselves with conveneince. Use an IDE when you start a professional job and surprise yourself with how much faster you can code.
- I recommend `vim` because it's preinstalled on all linux machines, useful for system recovery. It's great over `ssh` or if you switch machines often. 
(Emacs is useful for someone who wants to take their time to really set up their development environment for one machine, and let the investment of the large up-front customization pay off later on.)
- use LUKS to encrypt your hard drive on a Linux machine
- Use [DropBear](https://matt.ucc.asn.au/dropbear/dropbear.html) to encrypt a hard drive at boot, and ssh to decrypt it. Or something like that.
- I have [this link](https://www.scaleway.com/) bookmarked for some reason. Dunno, maybe it'll be useful.
- I'm just gonna leave [this](https://cock.li/) here (seriously **NSFW**)
- Use [Open](https://libreboot.org/faq.html) [Source](https://www.coreboot.org/) boot loaders!
- VPNs [are](https://openvpn.net/)
[cool](https://www.expressvpn.com/)
[too](https://www.wireguard.com/)
- Become a [Programmer, Motherfucker](http://programming-motherfucker.com/become.html)
- [N-O-D-E](https://n-o-d-e.net/) is cool.
- `lldb` `valgrind` `hashcat` `wireshark` `nmap` `htop` and the `air`*`-ng`s, Hopper, IDA Pro, VMWare Fusion, Docker.
