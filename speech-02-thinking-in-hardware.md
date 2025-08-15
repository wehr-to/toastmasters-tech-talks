## Intro bullet points 

- A lot of things in life can be attributed to cause and effect
- You flip a light switch, and the room lights up. But what really happened?
- The switch closed a circuit, allowed current to flow, which excited atoms in a filament or triggered LEDs to emit photons.
You didn’t see all that. You just saw the effect.
- We treat software the same way, we click, it responds, not many question the cause and beneath below these actions, and especially what would happen if someone were to break the cause and effect chain.
- I will explain that to truly build, defend, or understand technology, you need to think in layers down to hardware, firmware, and physical memory itself

The goal of this section was to really get the audience picturing how to envision the rest of the talking points 

## Mid section / Abstractions are the illusion

- Many live in the effect only while never seeing the true cause, think someone only operating within a GUI and never thinking to see the syscall or write code while never wondering what exactly the CPU does with it
- While operating systems, libraries, and drivers exist to hide complexity and make things easier, they can make a defender blind to vulnerabilities beneath, and this can allow an attacker to not only control the cause but the effect as well
- A prime example of this is spectre, they didnt break into the OS, but rather exploited the way CPU's guess the future and leaked data from processes
- Tying back to my point, these high level attacks do not care about what you wrote, they care about what your actual machine guesses, stores, and moves information at the lowest level

## Wrapup 

- We patch web apps, we scan ports, but asking yourself how does the memory actually behave is equally if not more important
- The book OSTEP teaches that the OS exists to manage complexity and isolation, things like memory management, scheduling, and syscalls, but if the OS is built on assumptions on how the hardware behaves, and the hardware gets manipulated, then even your OS becomes exploitable.
- To tie everything back to the beginning point, as a security professional has to think beyond "how does this python function work" but rather "how does this syscall behave?", in laymans terms understanding the underlying causes has more secure outcomes.

## Resources
- https://meltdownattack.com/

## Presentation mastery pathway alignment: 

| Toastmasters Goal         |      Speech Contribution                              |
| ------------------------- | ----------------------------------------------------- |
| Build audience connection | Light switch metaphor, cause/effect framing           |
| Use compelling structure  | Clear intro > thesis > examples > conclusion          |
| Demonstrate presence      | Analogies & pacing invite vocal/body variation        |
| Persuade with logic       | Spectre, syscalls, memory behavior = layered evidence |
| Express your voice        | Deeply technical but explained with clarity           |

####
- Many things in life can be explained through cause and effect.
- Flip a light switch > the room lights up. But what really happened?
- The switch closed a circuit.
- Current flowed.
- Atoms in a filament or LED emitted photons.
- You saw the effect, not the underlying cause.
- Software works the same way: we click, it responds.
- Few think about the layers beneath—or what happens if someone breaks the cause-and-effect chain.
- To truly build, defend, or understand technology, you must think down to hardware, firmware, and even physical memory.

#### Mid Section, Abstractions as Illusions
- Many live entirely in the “effect,” never questioning the “cause.”
- Example: Someone who only works in a GUI may never consider:
- The syscalls behind a button click.
- The CPU instructions behind those syscalls.
- Abstractions (OS, libraries, drivers) hide complexity and make life easier.
- But abstractions can blind defenders to deeper vulnerabilities.
- Example — Spectre vulnerability:
- Attackers didn’t exploit an OS bug.
- They exploited speculative execution, where CPUs predict future instructions to improve performance.
- Predictions left subtle traces in cache, which attackers measured to leak sensitive data from other processes.
- High-level defenses can fail if the attack targets the machine’s actual low-level behavior.

#### Closer
- We patch web apps and scan ports, but how often do we ask: “How does memory actually behave?”
- Operating Systems: Three Easy Pieces teaches that the OS manages complexity—memory, scheduling, syscalls.
- If the OS is built on hardware assumptions—and those assumptions are wrong, the OS’s guarantees can fail.
- This mindset prevents you from being a walking vendor demo and instead makes you someone who truly understands what’s under the hood.
- Security professionals must think beyond:
- “How does this Python function work?”
- To: “How does this syscall behave? What does the hardware actually do?”
- When you understand the true cause, you can protect the effect.
