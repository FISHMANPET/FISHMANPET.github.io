---
title: "What is automation, to me"
categories:
  - automation
future: true
---

I'm the team lead of our new Infrastructure Automation team, a team that exists basically because I asked for it. I've been given an incredible amount of freedom to  to set my own vision and direction for the team. Importantly, it means "Automation" gets to mean whatever I say it means.

But, what do _I_ think Automation is?

I've been an ops my entire career, and as an elder millennial I think I'm just old enough to be able to say "back in my day."
And back in my day, we didn't have virtualization, or most of the configuration management tools as we know them now.
Building and configuring new systems and applications was comparatively rare, and was often done by hand. And we liked it that way!

We did things by hand, that's manual.
Lot's of IT people all over are in a state like this even today.
A new employee is hired, and they have to create an AD account,
add the user to some mailing lists, enable access to some cloud services,
and maybe a few other things.
Some of them will get frustrated by all this manual effort, which also happens to be error prone, and they'll start writing a script to do the work for them.

In my world of Windows and PowerShell and operations, we seem happy to call this "Automation".
To me, this is the first step towards automation, but it's really not quite automation.

As cliched as dictionary definitions are, the word automation is derived from the word automatic.
But a tech having a script that can be used when a new employee is hired isn't automatic. it still requires the tech to take an action.
IT seems rife with farming analogies these days, so I think back to farming 150 years ago, before tractors.
It was lots of hard manual labor, and the tractor revolutionized that.
But the tractor didn't automate farming, it _mechanized_ it.

Likewise, the person working the help desk and writing a script to make their job easier hasn't fully automated that task, but they have mechanized it.
I don't make this distinction because I think mechanization is less important than automation. In fact it's vitally important, if for no other reason it's the first step to automation.

As someone with a background in ops, rather than dev, I think my perspective on automation is a little different from the conventional devops wisdom.
Ironically, whereas the dev-focused devops definition seems concerned with automating infrastructure (in service of the apps),
my ops perspective is that I'm interested in automating the business process, which usually means consuming those apps.

That business case, that's where things start getting exciting to me.
I work at a sprawling public university with over 60,000 students,
nearly 5,000 faculty, and nearly 15,000 staff.
We're also highly decentralized.
If you can name an application or service, somebody somewhere here is probably running it.
And eventually those applications will need to work together in some way.
Even something as simple as logging in can become a huge undertaking,
when SSO auto-provisioning doesn't have all the hooks you need,
like how all our Slack users have their timezone set to the default of PST.
Or maybe it's more complicated than that. How you get data out of system 1,
transform it, put it into system 2, then pull the changes out,
put them through system 3, and put the result back into system 1?
In other words, how do you _glue_ it all together?

_Glue_. Now there's a word

As a brief aside, I'm aware of Tanya Reilly and her description of [Glue Work](https://noidea.dog/glue)
and fully agree with her analysis and assessment of it.
And I see some of that glue work in the tasks I choose to take on in my role.
Though as a cis white guy and especially as one with a woman manager,
I'm able to sidestep a lot of the career pitfalls that come from doing glue work.
Maybe some day I'll have more to say on that topic but for now,
I just want to acknowledge Tanya but also point out that for purposes of
this discussion, the _glue_ I'm talking about here is separate from Tanya's _glue work_.

Back to _my_ glue. How do I glue all these systems together?
I get excited by a well documented REST API.
I get excited when I find a "hook" into a process (business or technical)
that lets me interact with it and inject what I need into it.
