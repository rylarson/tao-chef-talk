## Build, development and test environments as code

**Ryan Larson**

Software Engineer, Tripwire

--new-slide--

## Story time

Tripwire Story

Note:
   * Telling this story to tell you another story
   * I think we are at the same crossroads with environment automation

## Story time - The beginning

Old school software development

Separate development and QA silos

Note:
   * This was bad
   * QA gets involved too late when bugs are costly to fix, especially if they are a product of the basic design
   TODO look up more reasons this was bad

--page-break--

## Story time - Scrum Culture

Developers and QA coexist on Scrum teams that are now
responsible for their own Development and QA.

Note:
   * This is good
   * QA gets involved early, finds bugs.
   * Bugs are cheaper to fix because developers have context when the bugs are found
   * Tripwire always did 'agile'. The culture shift is what took time. Scrum processes helped
      * The culture shift is what was important and what was hard.
   * People problem solved

--page-break--

## Story Time - Blurred lines

   * Move to Scrum drove the blurring of the lines between dev and QA.
   TODO draw this same parallel between DevOps and blurring of the lines between dev and ops
   TODO at least that this created the tools that allows us to get this value
   * Developers naturally pick up some QA work
      * Developers automate, leading to more automated tests

Note:
   * Culture shift leads developers to feel ownership of QA

--page-break--

## Story Time - Test automation

Test automation is valuable

TODO The value add promise of automation is that a developer can make a change, run the tests, and if they pass, they know
they didn't break anything

TODO tie this into value add of codifying environments as code. At any time, test, development, and build environments
 can be reproduced with confidence that the exact same bits are built.

Note:
   * The company as a whole sees the shift towards more automation as extremely valuable
      * At the end of the day, nothing will succeed unless it has value

--page-break--

## Story Time - But wait

Automation is a culture problem too

   * Some teams were naturally better at automation than others
   * Business takes top down approach to make automation skill set available to all teams
      * Forms Performance & Automation team
   * Changing culture is hard :(

Note:
   * 'Step back' feeling
   * Developers and QA both cry "We have to specialize" as jobs move together
   * Ineffective, why? Because it is the same situation as the rest of QA was prior to the agile shift
      * Perf bugs found late in cycle, Perf team doesn't get a hold of the code quick enough
   * Even with embedding perf team members, didn't really work because the performance **culture** wasn't baked into the team
      * Culture is much harder to change, doesn't happen from the top down
         * Lots of push back from developers (we have to specialize!)

--page-break--

TODO this is the transition point to environment automation

## Story Time

Automating your test only gets you so far. You still need resources on which to run the tests.

   * Variances in environments makes automated tests brittle
   * Loss of confidence in automation devalues the automation

TODO Environment automation is even harder than test automation
TODO Test automation frameworks are usually a product of language or technology choice, there are standards
TODO Not invented here syndrome and poor sharable design cause nobody to share anything
TODO transition into Chef as a framework!
TODO can be used by dedicated teams and feature teams HANDOFF POINT****
TODO VM makes this possible
TODO we tried to write our own Configuration Management frameworks. Writing good frameworks is hard, no buyoff, no WIIFM because no free stuff from community site

Note:
   * Environment Problems:
      * Developer machines with the right environment to author tests
      * Continuous integration slaves to run the tests

--page-break--

## Specialization is bad

TODO tie this into blurred lines (maybe this + blurred lines is the closing of Story time)

--new-slide--

## Configuration Management

--page-break--

## Chef

--page-break--

## The power of virtualization

TODO Virtualization is nothing new
TODO Automating virtualization is nothing new
TODO Scripts are not reusable

--page-break-

Vagrant

--new-slide--

Ryan Larson

https://github.com/rylarson

@ryrylarson

TODO CALLOUTS
   * Chef provides common framework encourages sharing, we had pile of everybody's shit before

