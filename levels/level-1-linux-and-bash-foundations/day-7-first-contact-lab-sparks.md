
# Day 7: First Contact – Lab Sparks

*Level 1: Linux and Bash Foundations*

---

### Log Entry – Aroha

They didn’t say the first encounter would feel like this.

One moment, I was tracing commands in the calm comfort of documentation. The next, I slipped through a gap in the floor—no warning, no prompt—just the silence of a terminal cursor blinking like a pulse in the dark.

I’d fallen into **OverTheWire’s Bandit labs**.
And the air here was different.

The challenge began at **Level 0**, but it didn’t feel like a beginning. It felt like a test I hadn’t trained for. I sat still, breathing in the unease, watching that quiet prompt dare me to move.

I typed:

```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

A key.
A password.
A flicker of connection.

The gate opened.

Inside, I was greeted not by fireworks, but by silence and a command:
*“The password for the next level is stored in a file called readme…”*

But where was it?

I fumbled. I typed `ls`. Nothing.
Then I remembered the hidden layers—things not shown unless asked for.

```
ls -la
```

There it was: **readme**.
Just sitting there, like a secret not trying hard to stay hidden. I pulled it open:

```
cat readme
```

My first flag. Not a trophy, not yet. Just a whisper that said: *keep going*.

---

### The Descent Continues (Levels 1–4)

With each level, something shifted in me.
I moved from *"what am I supposed to do?"*
to *"what else are you hiding?"*

I learned the difference between file types with `file ./*`
I discovered `more`—a scroll into longer texts.
I hid things, revealed them, even changed their names like a ghost whispering across the filesystem.

Then the hidden files came.
**`.hidden`, `.sneaky`, `.silent-readme`**

Not visible unless you *ask*. Linux rewards curiosity.

```bash
ls -lah
```

I learned to tiptoe through them, to read between the lines.
The spacebar became a trap.

I laughed the first time I saw a file named:
**the aroha game**

But I couldn’t open it. Not without escaping the spaces:

```bash
cat the\ aroha\ game
```

Or better:

```bash
cat "the aroha game"
```

Even naming things could break the system—or bend it to your will.

I began seeing patterns.
Flags no longer felt like final destinations. They were breadcrumbs, and each command was a compass.

---

### Failures and Discoveries

There were moments I thought I’d broken everything.
An extra character.
A wrong quote.
A command that froze.

But that’s when I noticed something.

The fear was fading.

In its place, a quiet hunger.
One that whispered: *You didn’t break it. You’re just learning how to bend it.*

---

### Reflections

This was my **first real lab**, and I expected it to look like a monster.
Unsolvable. Cold. Hostile.

But it wasn’t.

It was a whisper, not a roar. A puzzle, not a punishment.

Yes, I slipped. Yes, I panicked.

But in the end—I got back up.

---

**Commands Unlocked Today:**

* `ssh` – enter the gates
* `ls -la` – reveal the unseen
* `cat` – speak with files
* `file ./*` – learn their true forms
* `find` – seek and locate
* `more` – scroll through the depths
* `mv`, `cp`, `rm` – shape the world

**Skills Gained:**

* Navigating hidden files
* Escaping space characters
* Reading subtle clues
* Calming down when things look wrong

---

*The labyrinth isn’t just outside.
Sometimes, it’s in the way you type.*
