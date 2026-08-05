# DebugVisualizer

<img width="1920" height="1032" alt="Screenshot 2026-08-04 124940" src="https://github.com/user-attachments/assets/2a28316d-a827-4ce0-815a-b74dc50b86bb" />


# DebugVisualizer

**See your program, don't read it.**
An open-source PyCharm plugin that renders algorithms and data structures live inside the Python debugger.

```
pip install text-debugging     →     pip install understanding
```

---

## The Problem

Debuggers show you this:

```python
nums = [5, 4, 3, 2]
```

DebugVisualizer shows you this:

```
 index   0   1   2   3
        ┌───┬───┬───┬───┐
        │ 5 │ 4 │ 3 │ 2 │
        └───┴───┴───┴───┘
                ↑
                i
```

No manual refresh, no expanding nested objects — it updates automatically on every step and breakpoint.

---

## More Examples

**Stack**
```
   TOP
 ┌──────┐
 │  30  │
 ├──────┤
 │  20  │
 ├──────┤
 │  10  │
 └──────┘
```

**Graph**
```
     1
     ●────●2
     │   ╱
     │  ╱
     │ ╱
     ●────●3
      \
       \
        ●4
```

**Heap**
```
           1
         /   \
        3     5
       / \   / \
      7  9  8  10
```

---

## What It Does

| Category | Highlights |
|---|---|
| **Live debugging** | Real-time updates while stepping, timeline playback, snapshot history, pin/focus views |
| **Data structures** | Arrays, matrices, stacks, queues, heaps, linked lists, binary trees, graphs, sets, dicts, custom objects, recursion stacks |
| **Debugger intelligence** | Variable tracking, change highlighting, scope tracking, frame & recursion visualization |
| **Visual polish** | Dark theme, animated diffs, compact multi-view canvas |

---

## Status & Roadmap

```
● v0.1.0 — MVP (current)     Stable visualization engine + PyCharm debugger integration
○ v0.2   — Object detection  Real linked-list/tree detection, pointer overlays, loop visualization
○ v0.3   — Algorithm Tutor   Bubble/Merge Sort, DFS, BFS, Dijkstra, Prim, Kruskal, Binary Search, DP, Backtracking
○ v1.0   — Stable release    Marketplace publication, settings page, packaged engine, docs, sample projects
```

---

## Requirements

- PyCharm
- Python 3.11+
- DebugVisualizer Engine *(packaging planned)*

## Built With

`Kotlin` · `IntelliJ Platform SDK` · `PyCharm Debugger API` · `Python` · `Flet` · `WebSockets`

## Vision

Make debugging *and* learning algorithms intuitive — for students learning data structures, candidates prepping for coding interviews, and instructors teaching algorithms.

---

**License:** MIT · **Contributions welcome** — open an issue or PR.

`pycharm` `jetbrains-plugin` `python` `debugger` `visualization` `algorithms` `data-structures` `education` `graph` `heap` `stack` `queue` `linked-list` `tree` `recursion` `flet` `kotlin` `intellij-platform`


![Build](https://github.com/Sedemsenaya/DebugVisualizer/workflows/Build/badge.svg)
[![Version](https://img.shields.io/jetbrains/plugin/v/MARKETPLACE_ID.svg)](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/MARKETPLACE_ID.svg)](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID)

## Template ToDo list
- [x] Create a new [IntelliJ Platform Plugin Template][template] project.
- [ ] Get familiar with the [template documentation][template].
- [ ] Adjust the [group](./gradle.properties), as well as the [id](./src/main/resources/META-INF/plugin.xml), [name](./src/main/resources/META-INF/plugin.xml), and [sources package](./src/main/kotlin).
- [ ] Adjust the plugin [description](./src/main/resources/META-INF/plugin.xml) (see [Tips][docs:plugin-description]) and this README to describe what your plugin does.
- [ ] Review the [Legal Agreements](https://plugins.jetbrains.com/docs/marketplace/legal-agreements.html?from=IJPluginTemplate).
- [ ] [Publish a plugin manually](https://plugins.jetbrains.com/docs/intellij/publishing-plugin.html?from=IJPluginTemplate) for the first time.
- [ ] Set the `MARKETPLACE_ID` in the above README badges. You can obtain it once the plugin is published to JetBrains Marketplace.
- [ ] Set the [Plugin Signing](https://plugins.jetbrains.com/docs/intellij/plugin-signing.html?from=IJPluginTemplate) related [secrets](https://github.com/JetBrains/intellij-platform-plugin-template#environment-variables).
- [ ] Set the [Deployment Token](https://plugins.jetbrains.com/docs/marketplace/plugin-upload.html?from=IJPluginTemplate).
- [ ] Click the <kbd>Watch</kbd> button on the top of the [IntelliJ Platform Plugin Template][template] to be notified about releases containing new features and fixes.

This Fancy IntelliJ Platform Plugin is going to be your implementation of the brilliant ideas that you have.

## Installation

- Using the IDE built-in plugin system:

  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "DebugVisualizer"</kbd> >
  <kbd>Install</kbd>

- Using JetBrains Marketplace:

  Go to [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID) and install it by clicking the <kbd>Install to ...</kbd> button in case your IDE is running.

  You can also download the [latest release](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID/versions) from JetBrains Marketplace and install it manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>

- Manually:

  Download the [latest release](https://github.com/Sedemsenaya/DebugVisualizer/releases/latest) and install it manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>


---
Plugin based on the [IntelliJ Platform Plugin Template][template].

[template]: https://github.com/JetBrains/intellij-platform-plugin-template
[docs:plugin-description]: https://plugins.jetbrains.com/docs/intellij/plugin-user-experience.html#plugin-description-and-presentation
