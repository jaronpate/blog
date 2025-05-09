<!-- [TLDR](#tldr) -->

We recently started hiring again, and with that came the scramble to pull together interview materials. Among them was a two JavaScript questions—simple, practical, nothing fancy. But as I was reviewing candidate submissions, something stood out.

Everyone’s answers were different—not just in implementation style, but in interpretation. Some misunderstood the constraints. Others made assumptions we had not intended. A few skipped over edge cases entirely, not because they missed them, but because the prompt never made them clear.

This was not a problem that was blocking hiring. It was not a fire that needed to be put out. But it was noise. Every submission needed extra context to review. Feedback we gave felt inconsistent. Candidates were being evaluated as much on their mind-reading ability as their technical skill and problem-solving abilities.

So I pulled the original prompt and rewrote it—clearly, explicitly, and directly. I packaged it into a single `.js` file that we could send to candidates, with instructions, scaffolding, and a test case included. Now we get consistent, comparable results. And now reviewers can evaluate problem-solving, not guesswork.

It is a small change. But it removed ambiguity from the process, saved review time, and made the experience better for both sides of the table.

This is glue work.

---

As far as I can tell this term was popularized by **Tanya Reilly**, who used it to describe the invisible work that keeps teams running. In her [talk at LeadDev New York (2017)](https://www.youtube.com/watch?v=KClAPipnKqw) she makes a great case for the importance of this work and how it is often overlooked. She also points out that often we do not recognize and reward this work. This essentially leads to these people feeling undervalued and unrecognized and they leave. Perhaps they leave the industry altogether.

**This sucks.**

For the customer, for the company, for the team, and...for *The Glue Engineer*.

I have been thinking about this more as our team has grown. While glue work is not equally valuable at every stage, there comes a point where ignoring it starts to slow everyone down.

When a team is very small—one or two people—most (if not all) of your energy should go toward shipping product, moving quickly, and doing the kind of work that accelerates your growth exponentially. Automation, abstraction, and process improvements can wait. There are no handoffs yet. There is no system to support. There is only motion to create.

But the second you start hiring—let’s say three or more engineers—you are no longer optimizing for speed alone. You are optimizing for shared context, reduced friction, the ability for people to move independently without stepping on each other, and—candidly—less reliance on individual contributors.

At that point, ignoring glue work does not just slow progress—it introduces friction, confusion, and seeds the ground for technical debt.

Glue work becomes the substrate that holds the team together. It is the tooling, shared language, and connective tissue that prevents small issues from escalating into systemic blockers. And the people who naturally step into that work—who see the gaps and quietly close them—are not always the most vocal, senior, or superstar engineers.

Here is the quiet tragedy of glue work: the engineers who do it best are often the ones pushed away.

They are not rewarded early, because their work is invisible. They are not promoted, because they are not always the most vocal. And they are often overburdened, because their instinct is to help, not delegate. Eventually, many of them leave. Not because they are not good enough, but because they are too good at something no one recognized.

And so, we lose some of the best potential team leads or product managers we could have had. People who already think across layers. People who already care about how their work unblocks others. People who understand that building a good system is not just about what it does, but how it behaves under pressure—and how it helps people do their best work.

I suspect this is the root of why engineers and managers so often talk past each other—and why the “PMs vs developers” trope exists.

And in fairness to the rest of us, it is hard to recognize. The answer is not to hand out medals for “doing the dirty work”. Glue engineers do not want pity. They do not want status. Most of the time, they just want to build things that matter—and to work in a system that sees the full picture of what engineering really is.

So if you want to keep these people—*and develop them*—here is where to start:

- **Make glue work visible:** Write it down. Say it out loud. When someone improves a system, connects a process, or unblocks a teammate in a way that scales—call it out. Make it part of the conversation.

- **Distribute it:** Glue work is a shared responsibility. A healthy team does not rely on one person to catch everything that falls between the cracks.

- **Reward product-aligned thinking:** If someone is thinking across layers—technical, operational, and human—take note. That is the shape of leadership, whether they have a title yet or not.

- **Ask people what they are carrying:** If someone seems unusually calm and competent, ask what is on their plate. You might be surprised by how much they are quietly holding together.

Good glue work does not draw attention to itself. But that does not mean we cannot learn to see it, appreciate it, and build teams that grow because of it.

If you have someone like that on your team, do not wait for them to burn out. Help them level up. Help them lead. Vouch for them. They are already doing the work.

---

#### TL;DR {tldr}

Not all engineering work is visible—but some of the most important work is what holds everything else together. As teams grow, systems need structure, consistency, and the kind of behind-the-scenes thinking that keeps things from falling apart. This is often called glue work—and the engineers who do it well are the ones we should be recognizing, supporting, and ultimately turning into leaders. Ignore it, and teams slow down. Support it, and everyone moves faster.