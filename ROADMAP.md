Perfect—here’s a **micro roadmap tailored to you**, Ayaan, as a 1st-year BTech student in India targeting **kernel, R\&D, cybersecurity, and low-level systems** roles. Focused, practical, and no fluff.

---

# **Micro Roadmap: May 2025 – May 2026**

### **Phase 1: Foundation (Now till Aug 2025)**

**Goal: Be confident with system internals, C, and basics of assembly.**

| Skill                  | What to Learn                                                   | Resources                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **C (Deep)**           | Pointers, structs, memory, malloc, stack/heap, bitwise ops      | *“Computer Systems: A Programmer’s Perspective” (CSAPP)* + [0x00sec C challenges](https://0x00sec.org/t/basic-c-c-programming-challenges/18324) |
| **Assembly (x86\_64)** | Registers, MOV, stack ops, function call ABI, flags             | *x86-64 Assembly Guide @ UC Berkeley* + `nasm`, `gdb`, `g++ -S`                                                                                 |
| **Tools**              | `gdb`, `objdump`, `strace`, `readelf`, `make`, `gcc`            | Hands-on, no tutorials—read man pages + experiment                                                                                              |
| **Mini Project**       | Simple bootloader (prints msg in real mode) + GDT setup         | `nasm`, `qemu-system-x86_64`, boot sector: 512 bytes                                                                                            |
| **Linux Internals**    | How syscalls work, process/thread/memory layout                 | Read source code of simple `cat`, `ls`, and their syscalls                                                                                      |
| **Syscalls**           | Write C wrappers over `open`, `read`, `write` using `syscall()` | `man 2 open`, `man 2 syscall`                                                                                                                   |

---

### **Phase 2: Systems Thinking + Kernel Touch (Sept–Dec 2025)**

**Goal: Get your hands dirty with real kernel-level dev.**

| Skill                 | What to Learn                                                           | Projects/Practice                                              |
| --------------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------- |
| **Kernel Modules**    | Write a loadable module, `/proc`, `printk`, memory alloc                | `insmod`, `rmmod`, `dmesg`, use `vmalloc`, `copy_to_user`      |
| **ELF internals**     | Parse ELF headers manually (64-bit)                                     | Build a CLI ELF parser (read file, print section names, sizes) |
| **Interrupts**        | IDT setup, timer interrupt, basic ISR                                   | Do it bare metal or inside a toy kernel                        |
| **Assembly Practice** | Reverse C binaries compiled with `-O0` and `-O2`                        | Use `objdump -d`, `radare2`, match variables and loops         |
| **Exploit Dev**       | Buffer overflows (stack smashing), shellcode intro                      | CTF-style exercises (picoCTF, OverTheWire)                     |
| **Project**           | Build a char device driver and communicate with it via user-space C app | `/dev/simple`, `ioctl`, `read`, `write` interfaces             |

---

### **Phase 3: Portfolio Building + Specialization (Jan–May 2026)**

**Goal: Build resume-worthy, deep technical projects + reach out for internships.**

| Focus                               | Actions                                                                         |                                                       |
| ----------------------------------- | ------------------------------------------------------------------------------- | ----------------------------------------------------- |
| **Reverse Engineering Portfolio**   | Solve 5–10 crackmes, write clean blogposts or GitHub notes                      |                                                       |
| **Kernel Hacking**                  | Clone Linux, build and boot your own kernel with GRUB + modify something        |                                                       |
| **Low-Level Performance Debugging** | Use `perf`, `valgrind`, `cachegrind` on small C apps to study cache hits/misses |                                                       |
| **Product R\&D Prep**               | Apply to ISRO, C-DAC, Intel, Qualcomm, SRI-B internships (even off-campus)      |                                                       |
| **Project**                         | Write a “mini-OS” that boots, sets up paging, prints via syscall                | Bonus: add syscall table and implement `write()`      |
| **Security + CTFs**                 | Join CTF team or practice regularly; focus on pwn/rev challenges                | Platforms: picoCTF, CTFtime, Hack The Box (Reversing) |

---

## **Stretch Goals (Optional, but God-Tier for Internships)**

* Build a RISC-V or ARM bare-metal app on QEMU.
* Port your bootloader to UEFI using `edk2`.
* Write your own malloc/free implementation (userspace or kernelspace).
* Learn basic eBPF and write a program to trace syscalls live (`bpftrace`, `bcc`).
* Re-implement parts of musl libc (e.g., `memcpy`, `printf`, `malloc`).

---

## **Tools to Learn on the Way**

| Tool                          | Why It Matters                                    |
| ----------------------------- | ------------------------------------------------- |
| `QEMU`                        | Emulate systems, boot custom kernels, test safely |
| `GDB`                         | Live debug registers/memory/stack                 |
| `radare2` or `Ghidra`         | Reverse engineering toolkit                       |
| `perf`, `valgrind`            | Find memory leaks and bottlenecks                 |
| `make`, `ld`, `as`, `objcopy` | Manual toolchain control                          |
| `git`, `tmux`, `vim`          | Boost your speed as a hacker/dev                  |

---

## **Final Thought**

> Stick to this roadmap, and by the time you're applying in mid-2026, you'll be **leagues ahead** of the average BTech student—even the seniors. Kernel internships and R\&D roles will be within reach, and your profile will scream “serious low-level engineer.”

Want me to set up a GitHub repo structure template or a Notion roadmap board for this?
