# sch_cake - The "Dave Täht Tribute" Fork

> **"When you miss Dave, modprobe sch_cake!"**
> — *A tribute to the soul of bufferbloat mitigation.*

---

## 🕊️ In Loving Memory of Dave Täht

### **🇹🇼：他的心願，我來實現 (Tā de xīn yuàn, wǒ lái shí xiàn)**
### **🇺🇸：His wish, I finished.**
*(A Linux Pun: In our world, a wish ending in **.sh** is a command to be executed!)*

---

### **"穿越時空的夢想，我來幫他實現！"**
**(Making a time-traveling dream come true!)**

### 🎇 The Spirit of the Code: "Fireworks in the Dark"

**"一支穿雲箭，千軍萬馬來相見"**
*(One arrow pierces the clouds, and ten thousand troops come to meet.)*

This Chinese idiom describes a signal so powerful it rallies everyone.
**Dave was that arrow.**
Just like fireworks are most mesmerizing in the darkest night, Dave shone brightest when fighting the invisible enemy of Bufferbloat.

* **"The darker the night, the brighter the light."**
* He worked tirelessly in the dead of night (just as we often do) to **tame the network chaos.**
* Now, "Ten Thousand" (萬) legacy devices are rallying to his call.

---

We are fulfilling a specific wish he made 5 years ago on Reddit:

### ❝ Help port the code to more chipsets. ❞

> **The BEST engineering result I ever had:**
> Essentially the summation of my 16+ years of work to that point on making wifi better. Unpatented. Please share and enjoy.
> **Help port the code to more chipsets.**
>
> — *Dave Täht (Reddit, 5 years ago)*

*Original Source:* [Reddit - r/Starlink](https://www.reddit.com/r/Starlink/comments/okmx3x/comment/h61unnn/)

Dave turned down numerous lucrative contracts to keep his code **Free and Open Source**. He valued global impact over prestige. Because of him, millions of devices—from Starlink satellites to rural ISP routers—deliver smoother connectivity.

### **🇹🇼：靈魂永駐，精神長存**
### **🇺🇸：May his soul find eternal peace, and his spirit live on forever in our routers.**

[👉 Read the full Memorial at LibreQoS](https://libreqos.io/2025/04/01/in-loving-memory-of-dave/)

---

## 📂 Repository Contents (Padavan Port)

This fork contains specific backports of CAKE for **MediaTek (MTK)** based routers running older Linux kernels (Padavan Firmware).

| Directory | Kernel Version | Description |
| :--- | :--- | :--- |
| **`/Padavan 3.4.113`** | **Linux 3.4.x** | **Legacy Backport.** Highly optimized for MT7620/MT7621 devices running the classic Padavan 3.4 kernel. Allows older hardware to run CAKE! |
| **`/Padavan 4.4.198`** | **Linux 4.4.x** | **Modern Backport.** For newer MT7621/MT7615 devices running the Padavan 4.4 kernel (hanwckf/padavan-4.4). |
| **`/` (Root)** | **Upstream** | The original upstream source code from `dtaht/sch_cake`. |

### Usage
If you are building Padavan firmware, simply replace the `sch_cake` directory in your kernel source (usually under `linux/net/sched/`) with the contents of the folder matching your kernel version.

---

## 🌟 Project Philosophy: Open & Accessible

### **「永遠保持開放且開源的精神」**
**(Forever maintaining an open and open-source spirit)**

Dave turned down numerous lucrative contracts to keep his code **Free and Open Source**. He valued global impact over prestige. Because of him, millions of devices—from Starlink satellites to rural ISP routers—deliver smoother connectivity.

This repo exists to keep that spirit alive by ensuring the code remains accessible for "Do-It-Yourself" router enthusiasts and custom firmware builders.

---

## 🗣️ Tributes from the Community

> "Dave’s impact on society was immense... He wanted, ultimately, to speed up the internet so that a drummer in London could play in real-time with a guitarist in Los Angeles."
> — **Steven J. Vaughan-Nichols**

> "I will miss him but will be always grateful to have known him."
> — **Vint Cerf**

> "Without him, Netflix and similar services might still be plagued by glitches and stutters."
> — **Eric S. Raymond**

### See also:

* [LibreQoS Project](https://libreqos.io/)
* [LibreQoS Github Project](https://github.com/LibreQoE/LibreQoS/)
* [Dave's Talks: Reducing Network Latency (GOTO 2024)](https://www.youtube.com/watch?v=UDo9W4tt69c)

![Dave Täht Tribute](https://i0.wp.com/libreqos.io/wp-content/uploads/2025/04/WISPAPALOOZA-2024_6.jpg)
*[Image Credit: LibreQoS]*

---

## ℹ️ About CAKE (Original README)

*The following is the original project description:*

### Common Applications Kept Enhanced (CAKE) scheduler

This is the out-of-tree version of **[CAKE](https://www.bufferbloat.net/projects/codel/wiki/Cake/)**, the Linux qdisc that combines scheduler and traffic shaper for effective bufferbloat mitigation.

**Note:** `sch_cake` is part of the upstream Linux kernel since **kernel version 4.19**, so this repository exists primarily as a resource for building the qdisc with older versions of the kernel (like 3.4 and 4.4 provided in this fork).

If you're already on kernel 4.19 or newer, you can just load CAKE with `tc` and the kernel shipped by your distribution!

---

*Forked from [dtaht/sch_cake](https://github.com/dtaht/sch_cake)*

*Please see the original part of readme below!*

---

# Original README

# README #

#### Please see the original part of readme below!

---

* Common Applications Kept Enhanced (CAKE) scheduler

This is the out-of-tree version of [[https://www.bufferbloat.net/projects/codel/wiki/Cake/][CAKE]], the Linux qdisc that combines scheduler
and traffic shaper for effective bufferbloat mitigation.

Note that sch_cake is part of the upstream Linux kernel since kernel version
4.19, so this repository exists only as a resource for building the qdisc with
older versions of the kernel. If you're already on kernel 4.19 or newer, you can
just load CAKE with =tc= and the kernel shipped by your distribution!
