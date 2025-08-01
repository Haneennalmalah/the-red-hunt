
### Day 9: Bash Blade Forging

*(Level 1 - Linux & Bash Foundations)*

The forge was still warm from the previous day — the air thick with the metallic scent of compiled language. But today’s craft was older. Rougher. Cruder.

Aroha returned to the training chamber. No silent elegance, no polished binary. Just raw, volatile energy.

This wasn’t about summoning a tool.
This was about learning to wield it.

The Bash blade.

---

### Phase I: Awakening the Blade — Your First Script

She etched her first rune:

```bash
nano aroha.sh
```

Within it, she scribbled the ritual:

```bash
#!/bin/bash
echo "The forge awakens"
```

To breathe life into it:

```bash
chmod +x aroha.sh
./aroha.sh
```

The blade vibrated. The terminal replied:

> The forge awakens

The blade lived.

---

### Phase II: The Curse of Echoily

But her second attempt backfired.

She tried adding:

```bash
echoily "This should work"
```

But the blade sputtered.

```bash
./aroha.sh: line 5: echoily: command not found
```

A ghost laughed in the darkness. She had written a non-existent spell. A typo. A moment of recklessness.

She learned: **every letter mattered**. Every command had to be forged with intention.

---

### Phase III: Enchantments and Variables

She crafted a box — a variable — to store her name:

```bash
name="Aroha"
echo "The wielder is $name"
```

Aroha. The system remembered.

Then, the secrets of **arguments** revealed themselves:

* `$0` → the name of the blade itself (the script filename)
* `$1`, `$2` → the whispers passed to the blade at execution time

```bash
echo "Script is: $0"
echo "First argument: $1"
```

She tried it:

```bash
./aroha.sh hello
```

And the terminal spoke back.

---

### Phase IV: Rituals of Repetition — Loops

The labyrinth loves repetition.

To test her endurance, she summoned:

```bash
for x in {1..10}; do
  echo "$x"
done
```

Then with new parameters:

```bash
for i in {10..20}; do
  echo "$i"
done
```

Numbers flooded the screen. A flood of power — orderly, brutal.

She opened a scroll named `xyz.txt`:

```bash
cat xyz.txt
```

It whispered:

```
Aroha
You’re
Done
```

So she invoked a loop through it:

```bash
for i in $(cat xyz.txt); do
  echo "$i"
done
```

Each word echoed through the forge like drumbeats of war.

---

### Phase V: Hidden Scrolls and Shadowed Files

She learned to create hidden files:

```bash
nano .secret.txt
```

And to find them:

```bash
ls -lah
```

There they were — silent, cloaked in the shadows.

To rename them, to unmask them:

```bash
mv .secret.txt revealed.txt
```

The veil lifted. The file was no longer hidden.

---

### Mindset Check: Thoughts from the Edge

She had no idea what a “Bash” was before this. Now, she wielded it like a jagged knife.

It didn’t always respond gently. Sometimes it bit her hand. Sometimes it mocked her typos.

But it was loyal.
And raw.
And real.

She had learned how to loop, to pass arguments, to forge variables. She’d peeked beneath the system’s skin and bent it with her will.

Her Bash Blade was no longer in the sheath.

It was sharp.

And it was hers.

---

Let me know when you're ready to commit it to GitHub — or move forward to the next arena.
