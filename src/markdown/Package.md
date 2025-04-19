# 📦 What Are Packages? (And How We Use Them at DTI)

This guide explains what **Packages** are and how we use them in our workflow — even if you’re not a coder.

---

## 🧱 What Is a Package?

Think of a **Package** like a special folder in Roblox Studio that you can:

- Share across multiple places
- Update for everyone else to use
- Avoid copying/pasting things between places

You can package:
- 3D models (like shoes, hats, or props)
- UI screens (like buttons or menus)
- Scripts and game logic

---

## 🧠 Why We Use Packages in DTI

Because every developer works in their **own branch**, we need a way to share work between each other. That’s what Packages do!

Instead of sending files or copying work:

- You **publish** a Package when you’re done
- Your teammates **sync** the new version into their workspace

It’s safe, clean, and avoids problems.

---

## 📁 Common Packages in Our Game

| Package Folder | What’s Inside |
|----------------|---------------|
| `Assets` | Hats, props, stage models, menus, results screens, game HUD |
| `Shared/Modules` | Utility scripts |
| `Client/Controllers` | Controllers |
| `Server/Controllers` | Services |

If you’re editing something nested inside one of these folders — you’re editing a **Package**.

---

## 🛠 How to Use Packages (Step-by-Step)

### 🧑‍🎨 Example: You’re a modeler updating a dress

1. Open your **branch**
2. Go to the `Assets/Models/Outfits` folder
3. Right-click the `Assets` Package → **Update** (this gets the latest version)
4. Edit the model (add your new dress)
5. Right-click again → **Publish to Package**

Now, anyone else who needs that outfit can click **Update** and get your version!

---

## 🔁 Team Workflow With Packages

1. Everyone works on their own branch
2. All shared things (models, UI, scripts) go inside Packages
3. When done, you **publish** your Package
4. Your teammates **update** their version of the same Package

We do this over and over until everything is finished!

---

## 🧼 Package Rules (Very Important)

✅ **Always publish** your Package when you’re done  
✅ **Always update** a Package before editing it, to get the latest changes
✅ **Only work on Packages in your branch**  
✅ **Tell the team** when you publish something  
❌ **Never link packages into the main game**  
❌ **Never manually copy packages between places**  
🟡 **Only tested packages** go into the Testing or Hotfix branches

---

## 📘 Want More Info?

Check out Roblox’s docs on Packages:  
👉 [Roblox Packages](https://create.roblox.com/docs/projects/assets/packages)

---

Packages keep our game stable, prevent accidents, and let us collaborate much more efficiently.  
