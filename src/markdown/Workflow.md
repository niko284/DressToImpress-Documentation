# 🧵 Dress to Impress – Production Workflow (Step-by-Step)

Welcome! This guide explains **how we build and update Dress to Impress** in a way that’s simple, organized, and avoids mistakes — even when many people are working at once.

This includes **programmers**, **UI designers**, and **3D modelers** — we’re all part of the same pipeline. So let’s walk through it together!

---

## 🎯 Why Do We Need a Workflow?

Right now, everyone works in different places. You might be:

- Making new outfits 👗
- Designing a UI screen 🎨
- Coding a new feature 🔧

That’s totally fine — but here’s the problem:

> If one person forgets to copy their work correctly, they might accidentally overwrite someone else’s updates or bring back old bugs. 😨

So this workflow helps us:
- Stay in sync ✅  
- Avoid breaking the game ❌  
- Publish updates safely 🚀

---

## 🧱 Step 1: What Is a Branch?

> A **branch** is just your own private version of the game — your own place to work without anyone else touching your stuff.

Think of it like your own studio or art table.

Each developer has a separate **branch** in Roblox Studio.

### 👥 Example:

- Nick works in **Nick’s Branch**
- Kyle works in **Kyle’s Branch**
- Alex works in **Alex’s Branch**

You can add new features, make model changes, fix bugs — whatever your task is — inside **your branch**.

---

## 📦 Step 2: What Are Packages (And Why Should I Care)?

We use **Packages** to share work across everyone’s branches.

> A **Package** is like a smart folder that everyone can update and sync.

You don’t need to copy-paste anything! Just **publish** a Package when you’re done, and your teammates can **sync** it into their own workspace.

### 🧢 Example:

- You (Nick) are updating a hat model inside a folder called `Accessories/Hats` inside **Nick’s Branch**.
- That folder is under the **Accessories** package.
- Once you’re done, you **publish the Package** (right-click → Publish).
- Later, Kyle (in **Kyle’s Branch**) clicks **Update** on that same Package, and *boom* — he now has your new hat model too!

This keeps everyone up to date and prevents mistakes like:

- Accidentally working on an old version
- Losing someone else’s progress
- Manually moving stuff between places (no more dragging models between games!)

If you’re not sure how to use a Package, check out [Package.md](Package.md).

---

## 🛠️ Step 3: Do Your Task in Your Own Branch

1. Open **your branch**
2. Find the Package you need (like a model folder or a UI folder)
3. **Update it first** to make sure you’re using the latest version
4. Make your changes (model, script, UI, etc.)
5. When you're done, **right-click → Publish to Package**

### 🎨 Example:

- Alex is making a new leaderboard UI in `Assets/UI/Leaderboard`
- He opens **Alex’s Branch**
- He edits the leaderboard design
- He right-clicks the UI package → **Update**, if he has to pull any changes from other developers in.
- When done, he right-clicks → **Publish to Package**

Now everyone can sync her new UI.

---

## 🧪 Step 4: Combine Everything in the Testing Branch

Once everyone finishes their tasks and publishes their Packages:

1. We go to the **Testing Branch** (a special place for final testing)
2. We update **all the Packages** with the latest versions
3. We test everything together as a team

This helps us catch bugs early, before the public sees them.

### 🧪 Example:

- Nick finished a new clothing item
- Alex finished a new UI screen
- Kyle finished a new character animation

In the **Testing Branch**, we sync all their Packages together to make sure it all works nicely.
Now, the Testing Branch will have the new clothing item, the new UI screen, and the new character animation!

---

## 🐞 Step 5: Bug Fixing (Loop Until It’s Perfect)

If bugs are found during testing:

1. The person responsible fixes the bug in **their own branch**
2. They **publish the updated Package**
3. The fix is **synced into the Testing Branch**
4. We test again

This might happen a few times until everything works.

### 🐞 Example:

- A bug is found in the camera when changing outfits
- Kyle originally made that feature
- Kyle fixes it in **Kyle’s Branch**
- He publishes the fix
- Testing Branch pulls the fix
- We test again to confirm

---

## 🚨 Step 6: What If the Live Game Breaks?

If something breaks in the actual live game (not during testing), we follow a **hotfix** procedure:

1. Create a new place called something like `Hotfix_April19`
2. Only sync the Packages needed to fix the issue (not unfinished work!)
3. Fix the bug in that hotfix
