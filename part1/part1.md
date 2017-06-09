autoscale: true
footer: Kenji Rikitake / oueees 201706 part 1 13-JUN-2017
slidenumbers: true

![](alissa-eady-92378-slide.jpg)

# oueees-201706 Part 1: Tragedy of sharing

<!-- Use Deckset 1.4, Next theme, 4:3 aspect ratio -->

---

# Kenji Rikitake

13-JUN-2017
School of Engineering Science
Osaka University
Toyonaka, Osaka, Japan
@jj1bdx

---

# Lecture notes on GitHub

* [https://github.com/jj1bdx/oueees-201706-public/](https://github.com/jj1bdx/oueees-201706-public/)
* Don't forget to *check out the issues*!

---

![original](elaine-casap-86020-slide.jpg)

# [fit] Sharing

---

# Share (v.)[^1]

Have/give a portion of (something) with another or others

Use, occupy, or enjoy (something) jointly with another or others

Possess (a view or quality) in common with others

[^1]: New Oxford American Dictionary, macOS 10.12.5

---

![right fit](instagram-jj1bdx-beer.jpg)

# More on share (v.)[^2]

Tell someone about (something), *especially something personal*

**Post or repost (something) on a social media website or application**

[^2]: New Oxford American Dictionary, macOS 10.12.5, emphasis by Kenji Rikitake

---

# [fit] Purposes of sharing:
# Showing off
# and
# Saving resources

---

![right fit](anthony-delanoix-14634-slide.jpg)

# Showing off

* **Publicly bragging**
* **Addiction for Approval**
* **「私かわいい」**
* ... and various other psychological reasons
* **Creating a lot of social problems**
* **To be discussed in Part 3**

---

![](matthew-henry-8819-slide.jpg)

# Sharing on programming

---

![](damjan-dobrila-39538-slide.jpg)

# Historical background on computing resources

* **CPU speed**
* **Memory**
* **Storage**
* **Network bandwidth**
* **...All always on shortage**

---

# Sharing, programming and memory

* Memory is expensive: *explicit* allocation required
* Variables are *mutable*
* Internal state is *commonly shared* and accessible between multiple functions and modules
* Use *memory pointers* to minimize the number of copying, inherently suggesting: *share as much as you can*

---

# Question: is sharing *intuitive*?

---

# In JavaScript (node.js)

```javascript
// var a = {first: 1, second: 2}
// b = a // only share pointer
{ first: 1, second: 2 }
// a.second = 3
3
// b // element is shared
{ first: 1, second: 3 }
// b == { first: 1, second: 3 }
false // WHY?
```

---

# Copying *by default*, *not* sharing, can solve this issue

---

# In Elixir (v1.4.4)

```elixir
iex(1)> a = %{first: 1, second: 2}
%{first: 1, second: 2}
iex(2)> b = a # copying the map
%{first: 1, second: 2}
iex(3)> a = %{a | second: 3}
%{first: 1, second: 3} # member modified
iex(4)> b # not shared with a
%{first: 1, second: 2}
iex(5)> b == %{first: 1, second: 2}
true # intuitive!
```

---

# Thought: sharing is *not necessarily intuitive*

---

# Issues of sharing-based programming languages

* Access violation between multiple programs
* Zombie memory area without ownership
* Need for explicit copying cause bugs
* Mutable states are difficult to debug
* Semantically sharing is a *shortcut* and breaks many logical assumptions

---

![](ben-white-194220-slide.jpg)

# Sad news: most languages work like JavaScript (or C++, C#, Java) - so be careful!

---

---
[.autoscale: true]

Photo credits:

* Title: Alissa Eady, from Unsplash.com
* Sharing: Elaine Casap, from Unsplash.com
* More on share: [Kenji Rikitake from Instagram](https://www.instagram.com/p/BUG6XGDh7Z9/)
* Showing off: Anthony Delanoix, from Unsplash.com
* Sharing on programming: Matthew Henry, from Unsplash.com
* Historical background on computing resources: Damjan Dobrilla, from Unsplash.com

<!-- coding: utf-8 -->
<!-- End: -->
