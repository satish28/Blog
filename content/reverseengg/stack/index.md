---
title: "Stack"
date: 2020-04-28T14:22:33+05:30
description: What is a stack.
tags: ["reverseengg"]
---

## Stack 

Stack is the memory region with the following features: 

* Last-in-first-out (LIFO) - Data added last is removed first.
* Static memory allocation - Stack is used only when the size of the data is known.
* Size of the stack is limited - Stack size is limited and it differs from PC to PC. In a nix based system use the below command to identify the stack size.
	```ulimit -a ```

	``` -t: cpu time (seconds)              unlimited
		-f: file size (blocks)              unlimited
		-d: data seg size (kbytes)          unlimited
		-s: stack size (kbytes)             8192
		-c: core file size (blocks)         0
		-v: address space (kbytes)          unlimited
		-l: locked-in-memory size (kbytes)  unlimited
		-u: processes                       1418
		-n: file descriptors                256
	```
* Temporary Memory - Stack memory is cleared on its own when the function exists.

### Advantages

* Simple and Fast.
* Memory on stack is automatically reclaimed when the function exits.

### Limitation

* Temporary storage - Stack memory clears out when the function exits.
* Size of the data has to be known. 
* Allocating more memory than available on the stack can cause crash due to stack overflow.
* Stack is limited in size. 
