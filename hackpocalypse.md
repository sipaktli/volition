# The Age of Artificial Intelligence and Certified Stupidity
*On cybersecurity, professional mediocrity, and the extraordinary sophistication of modern incompetence.*

Artificial intelligence is hacking everything.

Or so the headlines announce, with the sort of breathless astonishment normally reserved for discovering that water is wet.

AI is finding vulnerabilities, exploiting misconfigurations, uncovering exposed credentials, and identifying security weaknesses that have survived years of audits, certifications, and expensive consultancy.

Impressive. Sometimes extraordinarily so.

But there is another, rather less flattering interpretation: **perhaps AI isn't always demonstrating superhuman intelligence. Perhaps it is exposing substandard human diligence.**

Because much of what it discovers isn't some esoteric cryptographic weakness requiring the combined intellect of Alan Turing and a particularly gifted octopus. It is the technological equivalent of finding the bank vault unlocked, the combination scribbled on the door, and the security officer proudly displaying his ISO 27001 certificate.

The problem isn't that we don't know how to secure systems.

It's that we have constructed an entire industry remarkably comfortable with not bothering.

## The Certified Idiot Factory

Modern IT has developed an almost religious fascination with credentials.

Certifications, degrees, vendor badges, prescribed career trajectories, and enough acronyms to give an epileptic seizure to an alphabet.

Not that credentials are worthless. Quite the contrary. A proper education is invaluable, and certifications can demonstrate considerable knowledge.

But a certificate is evidence of having satisfied an assessment, not proof of competence, much less intellectual ability.

Somewhere along the way, we appear to have confused the map with the territory.

The industry increasingly hires by checklist, evaluates by checklist, promotes by checklist, and congratulates itself on the resulting abundance of highly qualified people who cannot distinguish a design principle from a deployment procedure.

Twenty years ago, at least parts of the computing world offered substantial opportunities to self-taught enthusiasts, unconventional thinkers, and obsessive tinkerers. It wasn't an enlightened meritocracy; incompetence and nepotism were hardly invented yesterday. But demonstrable technical ability could sometimes speak more loudly than formal credentials.

Today, a highly capable engineer can be eliminated by an algorithm before reaching an interview, while somebody with an immaculate collection of vendor badges gets to demonstrate their expertise by asking ChatGPT how to restart a Linux service.

We have automated recruitment without solving the small matter of knowing whom to recruit.

And there's a more pernicious consequence.

An organization incapable of recognizing expertise is also incapable of recognizing its absence. Mediocre professionals hire people whose competence they can understand, often reproducing their own limitations.

The genuinely inquisitive engineer becomes an inconvenience. Questions delay delivery. Discovering architectural deficiencies creates work. Exposing an incompetent implementation creates embarrassment.

Better hire somebody who knows the approved procedure, follows it diligently, and never asks why the procedure is idiotic.

**We have not eliminated incompetence. We have given it credentials, standardized its vocabulary, and promoted it into management.**

## First Principles, Last Priorities

The fundamentals of cybersecurity are not exactly classified information.

Least privilege. Defense in depth. Separation of duties. Secure defaults. Minimized attack surfaces. Failure isolation. Explicit verification.

Concepts established decades ago, explained in textbooks, prescribed by standards, and repeated in enough training courses to qualify as medieval liturgy.

Yet organizations routinely violate them.

We deploy elaborate identity-management platforms and then assign excessive privileges because properly defining permissions would be inconvenient.

We embrace Infrastructure as Code and use it to reproduce defective configurations across thousands of machines with unprecedented efficiency.

The security policy is wrong, but at least it's version-controlled.

We surround systems with sophisticated monitoring, endpoint protection, vulnerability scanners, and impressive dashboards, while neglecting basic architectural hygiene.

And when somebody discovers a serious flaw?

A ticket is created. Perhaps a meeting is scheduled. A risk assessment is commissioned. The vulnerability is assigned a color, a probability, an impact score, and an owner who will shortly be reassigned.

Eventually, somebody declares the risk acceptable.

Risk management itself is perfectly legitimate. Absolute security is impossible, resources are finite, and competent engineering requires tradeoffs.

But there is a difference between intelligently accepting a residual risk and turning neglect into an actuarial exercise.

**When calculating the cost of getting hacked becomes a substitute for preventing an avoidable compromise, risk management has become negligence with a spreadsheet.**

Then comes compliance theater.

The organization passes its audits. Its policies are immaculate. Its dashboards radiate reassuring shades of green.

Never mind the credentials exposed through an unauthenticated endpoint or the service architecture held together by obsolete initialization scripts, custom wrappers, and what appears to be industrial-grade optimism.

The auditor checked the box.

Presumably, the attacker will respect that.

Of course, not every ugly configuration is insecure, and not every vulnerability is evidence of incompetence. Complexity produces legitimate defects, including extraordinarily subtle ones.

But when an elementary flaw is demonstrated and those responsible cannot be bothered to investigate, we have crossed from imperfect engineering into professional indifference.

The particularly disturbing failure isn't ignorance.

**It's the complete absence of curiosity after ignorance has been exposed.**

## Modern Solutions to Problems We Didn't Have

The technological industry has another curious habit: treating adoption as progress, irrespective of suitability.

Everything must migrate to the cloud. Everything must be containerized. Everything must be automated. Every application needs another abstraction layer, preferably with a name suggesting revolutionary enlightenment.

Cloud computing is an extraordinary technology. It can improve resilience, elasticity, geographical redundancy, and disaster recovery.

It can also concentrate critical dependencies in a single provider's identity infrastructure, control plane, or operational ecosystem.

Three availability zones do not necessarily eliminate a common dependency.

Nor does moving an application to AWS magically transform a defective architecture into a resilient one. Sometimes you've simply relocated the disaster and arranged to pay for it monthly.

Multicloud isn't automatically salvation either. Complexity is quite capable of introducing more failure modes than it eliminates.

The serious question is not whether something runs in the cloud, but **which failures the architecture can withstand, and whether those are the failures that matter**.

Containerization offers another splendid opportunity for conceptual confusion.

Linux containers provide valuable mechanisms for process isolation and resource control. But a conventional container shares its host kernel. Its security depends on configuration, privileges, capabilities, namespaces, mandatory access controls, and additional protections.

A container is not a miniature virtual machine with an impenetrable moat.

FreeBSD jails offer a different, mature confinement model; neither technology possesses supernatural immunity to vulnerabilities.

Similarly, application packaging systems such as Flatpak can improve isolation, but their effectiveness depends upon sandbox permissions and the actual trust boundary. A sandbox with excessively broad access is an exceptionally well-packaged disappointment.

The problem isn't the technology.

It's using technology without understanding the properties it actually provides.

We have become extremely proficient at asking *how do we deploy this?* while becoming rather less interested in asking *why should we?*

## Your Face Is Now Somebody Else's Database

Biometrics deserves special recognition in the pantheon of contemporary technological absurdities.

Your fingerprint opens your phone. Your face grants access to financial services. Your government uses biological identifiers to verify identity. Your apartment building wants facial recognition because apparently metal keys were an insurmountable engineering challenge.

And somewhere, a company of questionable competence may be storing biometric templates under a privacy policy written by lawyers who have never encountered a database they didn't want to monetize.

Unlike passwords, biological characteristics cannot meaningfully be replaced.

To be precise, not every biometric authentication system exposes biometric data. Properly implemented device-local authentication can keep templates inside secure hardware and authenticate to services using cryptographic credentials. A compromised building-access template does not automatically grant access to a bank account.

These distinctions matter.

But centralized biometric repositories, opaque data-sharing arrangements, questionable retention practices, and ubiquitous identity collection introduce risks that extend far beyond authentication.

An authentication mechanism may be technically effective while creating an entirely different class of privacy and security problems.

And that suggests two independent questions that every technology deserves:

**Is it implemented correctly? And is its use desirable in the first place?**

A technically impeccable surveillance system can still be socially pernicious. An ethically worthwhile technology can still be incompetently deployed.

Unfortunately, the industry seems particularly fond of answering neither question before submitting the purchase order.

## Enter the Artificial Intelligence

Now introduce AI into this magnificent technological ecosystem.

For decades, attackers have exploited elementary vulnerabilities using techniques and tools they scarcely understood.

The script kiddie was already a formidable argument against the reassuring notion that attacking a system requires understanding it.

AI pushes this asymmetry further.

It can assist with reconnaissance, vulnerability analysis, code comprehension, exploit adaptation, and the examination of complex systems. It can make certain capabilities accessible to people who would otherwise lack the expertise to develop them independently.

Not every aspiring criminal becomes an elite hacker by typing an ambitious prompt. AI makes mistakes, invents vulnerabilities, and can misunderstand complex systems.

Nevertheless, reducing the cost of technical investigation and exploitation changes the economics of attack.

And this matters enormously when the targets are constructed upon decades of inherited technical debt, excessive privileges, misconfigurations, obsolete assumptions, and architectural decisions nobody has revisited since the original engineers departed.

Some AI discoveries will be genuinely brilliant. Others will amount to noticing that an application has unrestricted access to a production database for reasons nobody can explain.

The remarkable thing is not that AI notices.

It's that the humans responsible often didn't. Or worse, did and carried on regardless.

We already have examples of attacks reaching supposedly isolated critical infrastructure. Stuxnet demonstrated that an air gap, while a valuable defensive measure, is not an enchanted force field. Maintenance processes, removable media, trusted suppliers, and human behavior remain rather inconvenient features of physical reality.

Power plants, hospitals, banks, cryptocurrency exchanges, industrial systems, and ordinary consumer services are not automatically defenseless. Their security differs enormously, and capable defenders exist.

But the threat is increasingly asymmetric.

Defenders must maintain large, evolving systems, often under difficult operational constraints. Attackers can concentrate on particular weaknesses. AI may make parts of that search cheaper, faster, and accessible to more adversaries.

It does not follow that everything will inevitably be hacked.

It does follow that **the traditional strategy of surviving through obscurity, attacker incompetence, and sheer good fortune becomes progressively less sustainable**.

Particularly when the supposed defenders have institutionalized their own incompetence.

## The Real Vulnerability

The uncomfortable truth is that cybersecurity has never been merely a technological problem.

It is also an intellectual one.

We possess extraordinary tools, mature security principles, extensive technical literature, powerful automation, and decades of accumulated experience.

Yet elementary deficiencies continue to survive behind layers of certification, managerial hierarchy, procedural compliance, and professional self-congratulation.

A CTO need not personally understand every kernel mechanism. But technical leadership must preserve the capacity to recognize expertise, question assumptions, and ensure that credible warnings are evaluated.

An engineer need not know everything. But engineering demands the curiosity to investigate what one does not understand.

A security professional need not eliminate every vulnerability. But security cannot be reduced to producing evidence that a mandatory process was followed.

None of this requires genius.

It requires intellectual honesty, professional responsibility, and the increasingly unfashionable inclination to give a damn.

Artificial intelligence may radically transform offensive cybersecurity. It may discover vulnerabilities of astonishing complexity, devise unconventional attack paths, and expose failures that would otherwise remain hidden for decades.

But perhaps its most humiliating achievement will be much simpler.

It will demonstrate how many supposedly sophisticated systems were vulnerable to mistakes that never required sophisticated intelligence to recognize.

**We have spent decades teaching machines to automate our work, while teaching professionals to substitute procedure for understanding.**

Now we are building machines capable of examining the results.

And the results may not be flattering.

The coming cybersecurity crisis, if it materializes at the scale some fear, will not be attributable solely to the extraordinary abilities of artificial intelligence.

It will also reflect the accumulated consequences of things we already knew, already understood, already documented—and repeatedly chose not to address.

The machines may become frighteningly intelligent.

**The more immediate embarrassment is how little intelligence they may need.**

---

### References

- **Saltzer & Schroeder (1975),** *The Protection of Information in Computer Systems.* Foundational exposition of least privilege and secure-design principles. [IEEE](https://doi.org/10.1109/PROC.1975.9939)
- **MITRE,** *CWE Top 25 Most Dangerous Software Weaknesses.* Recurring, well-documented vulnerability classes. [CWE](https://cwe.mitre.org/top25/)
- **NIST SP 800-207,** *Zero Trust Architecture.* Architecture, identity, and implicit-trust failures. [NIST](https://csrc.nist.gov/pubs/sp/800/207/final)
- **NIST SP 800-63B,** *Digital Identity Guidelines.* Authentication, biometrics, and their limitations. [NIST](https://pages.nist.gov/800-63-3/sp800-63b.html)
- **NIST SP 800-30 Rev. 1,** *Guide for Conducting Risk Assessments.* The legitimate foundations of security risk assessment. [NIST](https://csrc.nist.gov/pubs/sp/800/30/r1/final)
- **CISA,** *Secure by Design.* The need to address security deficiencies at the engineering and organizational levels. [CISA](https://www.cisa.gov/securebydesign)
- **Langner (2011),** *Stuxnet: Dissecting a Cyberwarfare Weapon.* On the compromise of industrial control systems. [IEEE](https://doi.org/10.1109/MSP.2011.67)
