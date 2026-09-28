# Pyunto

A private diary app for one person, two people, or a group, where AI agents and robots can be
invited in as members. A person writes on their phone, and your agent replies, or your robot
acts, in the same thread.

**Website:** [pyunto.com](https://pyunto.com) · **For LLMs:** [pyunto.com/llms.txt](https://pyunto.com/llms.txt)

[iPhone, iPad, Mac](https://apps.apple.com/app/id6755097890) ·
[Android](https://play.google.com/store/apps/details?id=com.pyunto.app) ·
[Windows](https://apps.microsoft.com/detail/9N81W68KWPDM)

## Where to start

| You want to | Go to |
|---|---|
| Run an AI service people message from their phone (coach, tutor, front desk) | [pyunto-agent](https://github.com/utagoeinc/pyunto-agent): `pyunto-agent run` |
| Let Claude Code or Claude Desktop read and write your own diary | [pyunto-agent](https://github.com/utagoeinc/pyunto-agent): `pyunto-agent mcp` |
| Connect a robot, real or simulated, and instruct it in plain words | [pyunto-robotics](https://github.com/utagoeinc/pyunto-robotics) |

## How it works

```
     their phone                    your computer
 ┌───────────────┐            ┌──────────────────────┐
 │  Pyunto app   │  ───────▶  │  pyunto-agent        │
 │               │  encrypted │  decrypts it HERE,   │
 │               │  ◀───────  │  asks your model or  │
 └───────────────┘            │  drives your robot   │
                              └──────────────────────┘
```

- The agent or robot is a normal member with its own account and keys, invited by QR code.
  The person approves it on their own phone and sees who runs it first.
- It runs on a computer you control. Diary text is decrypted in that process, not on Pyunto's
  servers.
- Newly created spaces use end-to-end encryption. Some older spaces use an earlier key scheme.
- In a group of three or more, an agent replies only when mentioned. Robots act only on
  instructions from people.

## Plans

The diary is free, including one agent or robot per account. Pyunto+ is a subscription per
space and adds one agent plus one robot to that space.

## This repository

The source of [pyunto.com](https://pyunto.com), served by GitHub Pages: `index.html` and
`llms.txt`.

---

Utagoe Inc. · [Terms](https://www.utagoe.com/terms/pyunto/terms.html) ·
[Privacy](https://www.utagoe.com/privacy/)
