# Go Learning Roadmap
> For developers with some Go experience — beginner books skipped.
 
---
 
## Legend
- 📘 **Book** — from the repo
- 🌐 **Free** — online resource
- 🎯 **Specialist** — pick only if it matches your goal
- ⭐ **Core** — must read
---
 
## Stage 1B — Gap Fill
**Timeline: 3–5 days**
 
> You have Go experience so skip all beginner books. This stage patches the specific gaps Effective Go leaves — nothing more.
 
### Step 1 — Audit yourself (2–3 hrs, one sitting)
 
| Resource | Type | Notes |
|---|---|---|
| [Go by Example](https://gobyexample.com) | 🌐 Free | Skim only — don't study it. Write down unfamiliar topics on one sheet of paper. That's your gap list. |
 
### Step 2 — Read linearly (3–4 days)
 
| Resource | Type | Notes |
|---|---|---|
| [Effective Go](https://go.dev/doc/effective_go) | 🌐 Free | Read like a book, section by section. When it hits outdated GOPATH content, cross-reference Go by Example. Takes a weekend. |
 
### Step 3 — Patch the gaps (a few hours)
 
| Resource | Type | Notes |
|---|---|---|
| [Generics intro](https://go.dev/blog/intro-generics) | 🌐 Free | What Effective Go completely misses. |
| [Modules](https://go.dev/blog/using-go-modules) | 🌐 Free | Modern replacement for GOPATH. |
| [Error wrapping](https://go.dev/blog/go1.13-errors) | 🌐 Free | `errors.Is`, `errors.As`, `%w` — essential modern Go. |
 
### 🎯 Milestone
You can explain modules vs GOPATH, use `errors.Is` / `errors.As`, and write a basic generic function.
 
---
 
## Stage 2 — Idiomatic Go
**Timeline: 2–3 weeks**
 
> Read Learn Go with Tests and Ultimate Go Notebook in parallel — tests for practice, notebook for depth. Dip into Dave Cheney between chapters.
 
| Resource | Type | Priority | Notes |
|---|---|---|---|
| [Learn Go with Tests — Chris James](https://quii.gitbook.io/learn-go-with-tests) | 🌐 Free | ⭐ Primary | TDD-driven. Builds real testable code. 22k+ GitHub stars. Also in the repo as PDF. |
| Ultimate Go Notebook — William Kennedy | 📘 Book | ⭐ Read alongside | Deep on memory model, design philosophy, how Go actually works. One of the best books in the repo. |
| [Dave Cheney's Blog](https://dave.cheney.net) | 🌐 Free | Dip in | Practical deep dives on errors, interfaces, and idiomatic patterns. Read between chapters, not in one sitting. |
| Data Structures & Algorithms in Go — Hemant Jain | 📘 Book | ⭐ After LGwT | Read this after finishing Learn Go with Tests. You'll know the language well enough to focus purely on the algorithms, not the syntax. In the repo. |
 
### 🎯 Milestone
Rewrite an old Go project using proper interfaces, table-driven tests, and wrapped errors. Implement 3–4 classic data structures (linked list, stack, binary tree, hash map) from scratch in Go.
 
---
 
## Stage 3 — Real Applications
**Timeline: 4–6 weeks**
 
> One primary book. One reference site. Don't get distracted by the other web books in the repo.
 
| Resource | Type | Priority | Notes |
|---|---|---|---|
| Let's Go! — Alex Edwards | 📘 Book | ⭐ Primary | The best Go web book. Builds a full secure web app — routing, middleware, DB, auth, testing. Step by step. Also in the repo as PDF. |
| [Go Web Examples](https://gowebexamples.com) | 🌐 Free | Reference | Quick lookup for specific web patterns — JSON, middleware, templates, routing. Use while building, not as a read. |
 
### 🎯 Milestone
A deployed web app with auth, PostgreSQL, middleware, and integration tests.
 
---
 
## Stage 4 — Advanced Go
**Timeline: ongoing**
 
> Read in the order listed. Concurrency first — everything else builds on it.
 
| Resource | Type | Priority | Notes |
|---|---|---|---|
| Concurrency in Go — Katherine Cox-Buday | 📘 Book | ⭐ Start here | The definitive concurrency book. Goroutines, channels, select, pipelines, patterns. **Not in the repo — buy it.** |
| Let's Go Further! — Alex Edwards | 📘 Book | ⭐ | Advanced APIs, rate limiting, CORS, graceful shutdown, deployment. Direct sequel to Let's Go! **Not in the repo — buy it.** |
| Go with Domain — Laszczak & Smólka | 📘 Book | ⭐ | Domain-driven design in Go. Senior-level architecture thinking. In the repo. Also [free online](https://threedots.tech/go-with-the-domain). |
| Go Faster — Ollie Phillips | 📘 Book | ⭐ | Performance, benchmarking, pprof, memory optimization. In the repo. |
| Production Go — Schaaf & Smith | 📘 Book | ⭐ | Observability, deployment, reliability patterns. Read before launching anything serious. In the repo. |
 
### 🎯 Milestone
Profile a concurrent Go service with pprof, find a bottleneck, fix it. Deploy something with graceful shutdown and structured logging.
 
---
 
## Stage 4 (Specialist) — Pick by Goal
> Don't read all of these. Pick **one** based on where you want to go. All are in the repo.
 
| Resource | If you want to... |
|---|---|
| Distributed Services with Go — Travis Jeffery | Build distributed systems — gRPC, Raft consensus, service discovery. |
| Network Programming with Go — Adam Woodbeck | Build networking tools — TCP, UDP, sockets, protocols from the ground up. |
| Go for DevOps — John Doak | Build CLIs, automation, and infrastructure tooling as your primary Go use case. |
| Black Hat Go — Steele, Patten & Kottmann | Work in security or pentesting — offensive tooling and network attacks in Go. |
 
---
 
## Stage 5 — Expert / Internals
**Timeline: no finish line**
 
> This stage isn't scheduled — it happens naturally after Stage 4. You'll drift here on your own.
 
| Resource | Type | Notes |
|---|---|---|
| Writing an Interpreter in Go — Thorsten Ball | 📘 Book | Builds a language interpreter from scratch. Deep Go and CS fundamentals. In the repo. |
| Writing a Compiler in Go — Thorsten Ball | 📘 Book | Direct sequel. Read back to back with the interpreter book. In the repo. |
| Go standard library source | 🌐 Free | Read `net/http`, `sync`, `encoding/json` internals. The best advanced course that exists, completely free. |
| [GopherCon archive](https://www.youtube.com/@GopherAcademy) + [Go Blog](https://go.dev/blog) | 🌐 Free | Conference talks on scheduler, GC, escape analysis. Deep dives by language designers. |
 
### 🎯 Milestone
You can explain the Go scheduler, GC, and escape analysis clearly to someone else.
 
---
 
## Books to Skip from the Repo
> These are in the repo but not worth your time given your experience level.
 
| Book | Reason |
|---|---|
| An Introduction to Programming in Go — Caleb Doxsey | Too basic. Written for people with zero programming experience. |
| Go Programming Language for Dummies — Wei-Meng Lee | Beginner-focused, nothing new for you. |
| Go in 24 Hours — George Ornbo | Surface level. |
| Go Programming by Example — Agus Kurniawan | Thin and dated. Go by Example online is better. |
| Go, from the beginning — Chris Noring | Beginner only. |
| The Way to Go — Ivo Balbaert | Verbose. Better options exist at every stage. |
| Programacion estructurada en Golang — Luis Muñoz | In Spanish. Skip unless that's your preferred language. |
| The Little Go Book — Karl Seguin | Only useful if you want a 2-hr confidence check. Otherwise skip. |
 
---
 
## Quick Reference — Reading Order
 
```
Stage 1B  →  Go by Example (skim) + Effective Go + 3 blog posts
Stage 2   →  Learn Go with Tests + Ultimate Go Notebook + Dave Cheney → DSA in Go (after LGwT)
Stage 3   →  Let's Go! + Go Web Examples (as reference)
Stage 4   →  Concurrency in Go → Let's Go Further! → Go with Domain → Go Faster → Production Go
Stage 4S  →  Pick ONE specialist book based on your goal
Stage 5   →  Interpreter + Compiler (Thorsten Ball) → stdlib source → GopherCon + Go Blog
```
 
---
 
*Roadmap built May 2026. Books sourced from [KudaChan/GO-Books](https://github.com/KudaChan/GO-Books) repo.*
 
