## Build, development and test environments as code

**Ryan Larson**

Software Engineer, Tripwire

--new-slide--

## Blurred lines

Horrible song

--page-break--

## Blurred lines

* Development and QA
* Development and Operations

Note:
   * As automated testing has become more ubiquitous, the lines between development and QA have blurred
   * In some cases, the lines are gone
   * Agile, DevOps practices have driven this shift

--page-break--

## Blurred lines

Developers automate

TODO need something about VM

Note:
   * Developers create automated testing frameworks
   * Developers also create automated configuration management and deployment tools

--new-slide--

## Story Time

Tripwire Story

--page-break--

## Story Time

TL;DR Dedicated QA Teams to QA Engineers embedded with Development (or the other way around if you prefer)

   * Move to Agile around 2008 drove the blurring of the lines between dev and QA.
   * Developers and QA now coexist on Scrum teams
   * Scrum teams responsible for their own QA
   * Waterfall bad (QA gets involved too late when bugs are costly to fix)

--page-break--

## Story Time

What happened?

TL;DR Teams owning their own QA drove automation and got QA involved earlier in the process

   * Developers started writing more test code
   * QA started writing more test code [because they had to maintain developer code]
   * More code = more automation

--page-break--

## Story Time

Test Automation is valuable

   * The company as a whole sees test automation as extremely valuable
   * Developer mindset goes from "Testing is hard/not my job" to "Testing is awesome, more codez"
   * QA mindset goes from "Developers code" to "I code too"
   * This is clearly a gross generalization

--page-break--

## Story Time

What happened?

TL;DR Business recognized value of automation. Creates automation and performance testing team!

   * Some teams were better at automation than others
   * Business wants all teams to get value, so they form shared team to act as a support team for the feature teams
   * Ineffective, why? Because it is the same situation as the rest of QA was prior to the agile shift
      * Perf bugs found late in cycle, Perf team doesn't get a hold of the code quick enough (Tie this back into why we started to do Agile)
   * Tried Embed perf team members, didn't really work because the performance **culture** wasn't baked into the team
   * Culture is much harder to change, doesn't happen from the top down
      * Lots of push back from developers (we have to specialize!)
   * Teams are now responsible for their own performance (maybe roll this into because they know how to automate tests and their environments?)

--page-break--

## Story Time

Developers start becoming responsible for creating test environments

   * Both dedicated team and individual developers had automation for provisioning environments. Developers automate!
   * Not invented here syndrome and poor sharable design cause nobody to share anything

 TODO transition into Chef as a framework!
 TODO can be used by dedicated teams and feature teams HANDOFF POINT****
 TODO VM makes this possible

--new-slide--

Ryan Larson

https://github.com/rylarson

@ryrylarson

TODO CALLOUTS
   * Chef provides common framework encourages sharing, we had pile of everybody's shit before

