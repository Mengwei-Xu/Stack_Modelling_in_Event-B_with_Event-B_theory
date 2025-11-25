# Stack Example in Event-B and ProB

This repository contains a Rodin project archive:

- `StackProject.zip` – a **Rodin project** that defines:
  - A **theory** `Stack` with a polymorphic datatype `Stack(E)` and operators `pop` and `isEmpty`.
  - A **context** `StackCtx` instantiating stacks over integers and defining a concrete stack.
  - A **machine** `StackM` that maintains a set of stacks and pops a non-empty stack using the theory operators.

Once Rodin, the Event-B Theory support, and ProB are installed, you can import this archive and animate the machine directly.

---

## 1. Install the Rodin Platform

Download the Rodin Platform from:

- <https://sourceforge.net/projects/rodin-b-sharp/>

Choose the distribution for your OS, unpack it, and follow the installation/usage instructions in the Rodin README or documentation.

---

## 2. Ensure the Event-B Theory plug-in is available

In Rodin:

1. Go to **Help → Install New Software…**.
2. In **Work with**, select the main Rodin update site  
   `http://rodin-b-sharp.sourceforge.net/updates`.
   (different version of Rodin may have different naming or multiple listings for this update site)
3. Under the category **Modelling Extensions**, select the **Theory** plug-in (or equivalent).
4. Complete the installation and restart Rodin.

For more details, see the Theory wiki page:  
<http://wiki.event-b.org/index.php/Theory_News_and_Support>

---

## 3. Install the ProB plug-in for Rodin

In Rodin:

1. Go to **Help → Install New Software…**.
2. In **Work with**, select the update site that provides **ProB** (this may be called “ProB for Rodin” or similar, depending on your distribution).
3. Select the **ProB** plug-in and install it.
4. Restart Rodin.

After restart, you should see **ProB** entries in the context menu when you right-click on an Event-B machine or context (e.g. “Start Animation / Model Checking”).

---

## 4. Get this project into your Rodin workspace

> You do **not** need to unzip `StackProject.zip`. Rodin can import it directly.

In Rodin, please go to **File → **Open Projects from File System**…**, then select `StackProject.zip` from this repository. The project will appear in the **Event-B Explorer**. You can then open the theory, context, and machine, and use ProB to animate `StackM`.
