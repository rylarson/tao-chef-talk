## Build, development and test environments as code

**Ryan Larson**

Software Engineer, Tripwire

--new-slide--

## Story time

Tripwire Story

Note:
   * Telling this story to tell you another story
   * Evolution of relationship between QA and Development is similar to evolution of relationship
   between Development and Operations
   * Evolution of test automation is similar to evolution of environment automation
   * I think we are at the same crossroads with environment automation

--page-break--

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
   * Teams feel shared ownership of both development and QA

--page-break--

## Story Time - Test automation

Scrum blurred the lines between development and QA. At the same time, the industry as a whole was making a shift towards
automating lots of tests.

Note:
   * Automation further blurred the lines between dev and QA.
      * Developers were picking up QA 'development' tasks and QA was developing software to test software.

--page-break--

## Story Time - Test automation

Test automation is valuable

TODO tie this into value add of codifying environments as code. At any time, test, development, and build environments
 can be reproduced with confidence that the exact same bits are built.

Note:
   * The company as a whole sees the shift towards more automation as extremely valuable
      * At the end of the day, nothing will succeed unless it has value
   * The value add promise of automation is that a developer can make a change, run the tests, and if they pass, they know
     they didn't break anything
   * This change empowered developers to find many of the bugs before things got to QA.
   * Allowed developers to have greater confidence in their code and be more autonomous

   TODO empowering developers with automated tests is the same as empowering them with automated environments

--page-break--

## Story Time - It wasn't easy...

Automation is a culture problem too

Note:
   * Some teams were naturally better at automation than others
   * Business takes top down approach to make automation skill set available to all teams
        * Forms Performance & Automation team
   * Ineffective, why? Because it is the same situation as the rest of QA was prior to the agile shift
        * Perf bugs found late in cycle, Perf team doesn't get a hold of the code quick enough
   * Changing culture is hard :(
      * Even with embedding perf team members, didn't really work because the automation **culture** wasn't baked into the team
         * Culture is much harder to change, doesn't happen from the top down
            * Lots of push back from developers (we have to specialize!)
   * Developers and QA both cry "We have to specialize" as the job roles start to have more overlap.

--page-break--

## Story Time - But we did it

Driven by industry shifts, better tools, and better processes, we eventually got it.

Note:
   * It took time, but the culture shifted
   * Common tool sets allowed teams to share best practices, even share code
   * Industry as a whole highlighted the value
      * Test automation as a practice matured across the industry
   * Not specializing didn't hurt anybody!

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

