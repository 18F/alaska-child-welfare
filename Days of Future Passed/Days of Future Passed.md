# Neo-ORCA: Days of Future Passed

## Families Care: The Alaska HSS Quarterly Newsletter, April 1, 2024

This week we are interviewing Simon Taylor, as he moves on from 20 years
of State of Alaska service and prepares to start a second career as a
barrel cooper in Spain. Simon started as one of the IT folks who
participated in the original “ORCA” implementation effort in 2003 –
2004. So, as we celebrated completion of Neo-ORCA and decommission of
the final ORCA subsystems this year, we wanted to get Simon’s
perspective on the significance of this milestone.

*Interviewer:* Looking back, what was the most significant moment for
the Neo-ORCA?

*Simon:* Of course, there were so many, but I would have to point back
to some of the original work the team did in 2018 with mobile
initiatives and adapting to the Tribal Compact. Prior to that year, the
team had been gaining ground with agile approaches, but we were also
trapped in the mindset that we needed a particular support vendor in
order to make significant changes.

I said “mindset”, but it was more than just a mental block. At the time
we had over 10,000 source code artifacts and hundreds of thousands, if
not millions, of lines of code to manage. We also had a very good, but
sort of brittle homegrown build-automation tool that we used to quickly
produce builds. Our State tech team understood the mechanics of this
build tool, but it was cobbled together by staff who had moved on, and
no one could easily maintain or modify it to handle new technologies.
Our support vendor was very committed to helping us move forward, but
the foundations of the code base were about 20 years old at that time,
and “moving forward” was not a simple or reasonably priced proposition.
We had not yet moved into the agile procurement model, and everyone was
understandably trapped in economic and business system maintenance
models that made it too risky to break into new technologies without
putting massive amounts of capital and/or operating funds at risk.

So, we had numerous hurdles to overcome, and the team’s efforts to
further embrace agile scrum methods and actually adapt our traditional
procurement model to an agile and modular procurement approach really
made everything else possible.

*Interviewer:* You mentioned codebase and CI/CD challenges. Tell me a
little more about that.

*Simon:* It’s so amazing to look back now and realize how much we’ve
benefited from a more streamlined codebase and the ability to do CI/CD.
There are really two stories here that are both about whether your
effort goes into business needs or into the business of writing and
maintaining software.

The first story is that the more code you write, the more bugs you
write, test and (ultimately) ship as defects. A bigger codebase means
you are losing that much more business value every step along the way.
And this continues into maintenance, costing more to understand the
code, design and implement new features, etc. So, our smaller Neo-ORCA
saves us money every day in our total cost of ownership.

The second story is about the ability to fail and recover quickly. Since
even well designed, well implemented software features can fail to meet
the needs of their users, failure is unavoidable. This means we want to
*reduce* the cost of failure as much as possible. Scrum, CI/CD and other
processes like prototyping allow us to do just that. We break down the
work into smaller pieces and we fail – or succeed – as fast as possible.
This saves us money both by avoiding wasted effort by the team, and also
avoiding lost business value “living with” problems (barriers to
success) in production.

It’s also worth noting that in transitioning our CI/CD tools, we were
able to save $60K per year in redundant version control and change
management tools. This was a cost that was growing at about 8% per year.
So, over the last six years, that has translated to nearly $450,000.

*Interviewer:* Has everything just been relatively easy then since 2018?

*Simon:* Oh, no. Things were quite hard at first. As I mentioned above,
there were some big transitions in how we were trying to get work done.
We had some assets going into 2018, like our automated build system.
Even so, we decided it would be best to migrate the build system to Team
Services where we were more easily able to maintain it. We also had to
start figuring out what patterns we would actually use to implement the
encasement strategy that ultimately allowed us to let go of ORCA one
business function at a time. Finally, we had to get our teams to
understand how to design in this way. All these work transitions
translated to challenges and learning curves for support team members,
but we also had to adjustment how we worked with department leadership
and our federal partners.

Security was a significant hurdle, and there were a few other perfect
storms along the way, like the OIT transition occurring at the same time
we were working through business adjustments to accommodate the Tribal
Compact. We had to make some of our early decisions to transition from
the heavy Java platform we were on to the lighter .NET platform we moved
to. That was a big win because of our longstanding investments in .NET,
but it was also a new commitment to bifurcate the code and start down
the encasement path. So, it was really risky for us.

Really, we were lucky that the core ORCA team had been practicing agile
delivery and seen a lot of value out of it compared to the traditional
maintenance models. I actually think we might have thrown in the towel
if it hadn’t been for folks like Dana Penner and Joe Butler who had led
those early agile efforts prior to 2018.

*Interviewer:* Was there a specific technical feature that was a big win
for Neo-ORCA?

*Simon:* Well, again, there were many, but I would call out our document
solution. It allowed us to get rid of a clunky and unsupported ActiveX
control, move off of an unsupported Microsoft Office product, and
continue to use a standardized and versionable set of templates to merge
data into court and other required documents. We also improved the user
experience by eliminating a thick client viewer/editor for the
documents. So, it was a win all the way around.

I suppose, thinking about it a bit more, I should really point to the
mobile solution, though the win there wasn’t completely about the
technical “mobile” feature. Workers needed to be able to easily gather
case notes and photographic evidence in the field. So, mobile was a
great technical solution. However, in that case, I think the win was
solving certain security problems and breaking through with a
supportable, secure mobile solution. That was something the department
had previously only done with maybe one SaaS application. Also, it had
become a real pain point for Office of Children’s Services to be able to
collect information and evidence in the field in an efficient way. So,
that was also a big win to put those capabilities in workers’ hands and
to eliminate some serious information security risks at the same time.

*Interviewer:* The federal CCWIS standards have been a big deal for OCS
for a long time. What was that journey like, and what was the hardest
part of becoming CCWIS compliant?

*Simon:* CCWIS was hard. Even after the CCWIS rules were adopted for a
couple years, there was still a lot to learn about what the feds really
wanted. But I think the hard part about CCWIS was maturing our data
strategy in Alaska. CCWIS is *heavily* data centered with a focus on
data analytics, but our data analytics concepts in the department were
pretty immature when we started. This was true on the IT, the program
side and the research side.

So, we really had to up our game and invest in training our staff in the
breadth of the data-science and analytics field. This kind of investment
can be quite challenging because, in an environment where every dollar
budgeted has to be justified with some sort of concrete outcome, people
get very focused on tools instead of the more theoretical, conceptual
skills. That’s fine for producing specific reports, but when people are
heavily invested in tools, then they’re always getting steered by tool
vendors to re-invest in the tools. Again, that’s fine, but often times
the tool vendor is just selling them a glossy of a feature that is
actually quite common across the tool space. So staff get sold on a cool
looking but common feature, and then aren’t really focusing in that sale
on operationalizing the feature and how to really get the return on
investment. This typically leads to unrealistic expectations about the
work involved, which leads to investment failure.

The necessary alternative, in my opinion, is to educate staff in the
concepts behind the tool features, and in how to operationalize new
features. That way, when a tools vendor comes to the table with a glossy
pitch about all the cool things you can do with their tool, your staff
recognize the core concepts and can focus on the operational
opportunities and challenges really necessary to leverage the tool.

All of this held very true in the data analytics space that CCWIS
directed us to focus on. So, we had to mature our staff; we had to
invest in helping our people *really understand* the concepts that cut
across the tools. We also had to train people in thinking through and
implementing effective operational use of the capabilities involved.

Finally, as always, security was a big theme with CCWIS because you
can’t achieve data quality unless you are effective in revealing that
data to specific stakeholder groups in a way that invests them in
quality. So for CCWIS, this involved us rethinking how we design the
user experience – working toward a certain democratization of data to
achieve the right ownership and visibility of the data, while we worked
carefully to ensure we got the maintained the integrity of our
information security.
