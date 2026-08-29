# The future of communication, your assumptions tested, and the one thing to build

Written 2026-08-29 after building three versions of the wrong thing.

---

## First, my mistake, so you can discard it cleanly

I shipped three surfaces: a four-lane email board, a call-me interview, and a voice-first single
screen. Three places, three metaphors, no product. Each one was a feature answering the last thing
you said. That is the failure mode you named, and it is on me.

The rest of this file is one product.

---

## What is actually changing in communication

**1. The message stops being the unit.**
For fifty years the unit of every communication tool was the message: inbox, thread, channel,
DM. Every product innovation was a better way to sort messages. That whole line is finished,
because if an agent reads the messages, sorting them is not a job anymore.

The next unit is the **commitment**. Something you owe a person, or a person owes you.
"Get back to Oscar." "Send Dana the invoice." "Nadia owes me a yes or no."
A commitment can arrive by email, text, call, or in person. It survives the channel it came in on.

**2. The channel becomes a delivery detail.**
You do not care whether your reply to Oscar goes by email or SMS. The agent should pick. Today
you pick, because tools are organised by channel. That is backwards and it is the reason you have
an inbox, a messages app, a CRM, and a follow-up list that do not know about each other.

**3. Both ends stop being human.**
Within a few years your agent negotiates with their agent, and the thread is a machine-to-machine
transcript you see the outcome of. Email survives this because an address is still the only way to
reach a stranger without a platform's permission. The inbox does not survive it.

**4. The bottleneck moves from writing to deciding.**
When drafting is free, the scarce thing is your judgment. So the interface should spend all of its
surface on decisions and none on text you did not write.

---

## Your assumptions, tested

**"Kanban view for email."**
Half right, and I built the wrong half. Kanban over *messages* is wrong, because a board implies
you manage the cards, and the entire premise is that you should not have to. Kanban over
*commitments* is right, because a commitment genuinely has a state that changes over time and that
you genuinely need to see. Keep the board. Change what is on it.

**"Regular CRM is too bulky."**
Correct, and the reason is specific. A CRM is bulky because a human has to fill it in, so it needs
fields, forms, stages, and custom objects. If the agent fills it in from your actual conversations,
you need none of that. Three columns is enough. This is the real product insight of the night.

**"Email is outdated."**
The inbox is. The address is not. Do not try to replace the protocol, that is a graveyard. Replace
the interface on top of it.

**"AI should call me and interview context out of me."**
Strong, but it is a different product with different buyers, and I already researched it: the
customer-research version is crowded and funded, the developer-facing version is open. Do not fuse
it in. Ship it separately later. Inside this product, voice is just the fastest way to add a
commitment, not a forty-minute interview.

**"Cheap model classifies everything."**
True and necessary, but it is infrastructure, not the product. Nobody buys classification. They
buy "I stopped dropping things."

**"This might be a goldmine."**
The consumer version is a hard sell, because consumers do not have enough open commitments to feel
the pain. The person who feels it is you: a solo operator with more open loops than working memory,
no team, and no tolerance for a CRM. Freelancers, consultants, agency owners, solo founders,
recruiters, brokers. That is a real market and it is underserved precisely because it is too small
for Salesforce and too structured for a notes app.

---

## The one product

**Name it after the unit: an open loop.**

One board. Three columns. Nothing else.

**Waiting on them.** You did your part. The agent chases on a schedule, changes the angle each
attempt, and stops when told. Each card shows who, what you want, and when it next moves.

**Waiting on you.** The agent cannot proceed without a decision only you can make. Never more than
a handful. Each card is a question with two buttons, or a draft with a send button.

**Closed.** Today's, then it disappears. Proof of work, not an archive to maintain.

That is the whole interface. No inbox, no folders, no settings, no stages to drag.

**Input is voice.** One button. "Here's Oscar's email, I can do GTM for him, chase him until he
answers." A card appears in Waiting on them. That is the entire capture flow.

**Every channel feeds it.** Email first because it has an API and no permission problem. Then SMS,
then calls. A loop does not care which one it arrived on, and neither should you.

**It learns by example, not by configuration.** After any action: "Always do that?" One tap, and
the rule exists. No automation builder, ever. That is how you get workflow automation without a
workflow builder, which is the thing that makes every competitor bulky.

---

## What to cut, since Elon and Steve both said the same thing

Cut the fourth column. Cut the handled log. Cut the stats row. Cut the reasoning drawer, and put
one honest sentence on the card instead. Cut the boot animation. Cut the pitch text at the bottom.
Cut every number that is not a count of open loops.

If a designer asks what the product is, the answer should be four words: **it holds your loops.**

---

## The honest risk

The chasing has to actually be good, or this is a to-do list with extra steps. The defensible part
is not the board, it is that the agent writes a *different and better* follow-up each attempt using
context you never typed. If the follow-ups are generic, nothing here matters.

That is the thing to prove first, before any more UI.

---

## What I would do next, in order

1. One board, three columns, voice capture, teach-once rules. Delete the other two demos.
2. Wire real mail through AgentMail, since the key is already in your env and it needs no OAuth.
3. Prove the follow-up quality on your own two CEO pitches. If attempt two beats attempt one on a
   real human, you have a company.
