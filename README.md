### Hi there 👋

# Dmytro Mitin

Scala & Haskell developer and mathematician interested in **functional programming, type systems, metaprogramming, compilers, semantic tooling, formal methods, and AI-assisted software engineering**.

Much of my current open-source work explores how compiler and semantic infrastructure can make advanced Scala metaprogramming and coding agents more capable and reliable.

## Scala 3 metaprogramming & compiler tooling

### [Macro-Paradise for Scala 3](https://github.com/DmytroMitin/macroparadise-scala3)

Experimental Scala 3 compiler plugin bringing back a Paradise-style model of **pre-typer macro annotations**: annotations can transform definitions and generate members, companions, and sibling definitions before ordinary typing.

Released artifacts are available from Maven Central.

→ [Starter project](https://github.com/DmytroMitin/macroparadise-scala3.g8)

### [Quasiquotes for Scala 3](https://github.com/DmytroMitin/quasiquotes-scala3)

Experimental structural quasiquotes for Scala 3, spanning compiler-free semantic representations, Scalameta, quoted reflection, and exact-version Dotty internals.

The project investigates source-like tree construction and transformation while keeping compiler-independent structure separate from compiler-coupled lowering.

→ [Starter project](https://github.com/DmytroMitin/quasiquotes-scala3.g8)

### [AUXify for Scala 3](https://github.com/DmytroMitin/AUXify-scala3)

Scala 3 continuation of AUXify, using Macro-Paradise and Quasiquotes to implement macro annotations for common functional-programming patterns.

Current annotation families include `@apply`, `@aux`, `@instance`, `@delegated`, and `@self`.

→ [Starter project](https://github.com/DmytroMitin/AUXify-scala3.g8)
→ [Original Scala 2 AUXify](https://github.com/DmytroMitin/AUXify)

Together, these three projects form an experimental stack:

**Macro-Paradise** — annotation execution and source transformation
**Quasiquotes** — structural authoring and tree lowering
**AUXify** — higher-level FP/metaprogramming use cases

### [Allow Experimental](https://github.com/DmytroMitin/allow-experimental)

A bounded Scala 3 compiler plugin allowing selected implementations to use `scala.annotation.experimental` APIs without propagating experimental status to their callers.

Published on Maven Central and tested against several exact Scala 3 compiler versions.

### [Scala Semantic Harness](https://github.com/DmytroMitin/scala-semantic-harness)

Experimental **semantic tooling for Scala coding agents**.

It combines compiler/build evidence, SemanticDB, Presentation Compiler queries, symbol reconciliation, FP-oriented analyses, a CLI, an MCP server, and agent-facing integration layers.

The goal is not to replace the compiler, sbt, tests, or IDE tooling, but to give coding agents substantially richer structured evidence than plain source-text search.

## Earlier Scala metaprogramming work

### [AUXify](https://github.com/DmytroMitin/AUXify)

The original Scala 2 implementation of AUXify: macro annotations and type-level/functional-programming helpers around AUX types, type-class materialization, instance construction, delegation, syntax generation, Shapeless, Scalameta, and Scalafix.

### [Dotty-patched / Eval](https://github.com/DmytroMitin/dotty-patched)

Experiments with Scala 3 staging, runtime evaluation, patched compiler behavior, and using staging from macros. Includes published `eval` and patched-compiler artifacts.

### Smaller compiler & metaprogramming experiments

* [scala-macro-macros](https://github.com/DmytroMitin/scala-macro-macros) — macros expanding into macros
* [scala3-macro-closure-demo](https://github.com/DmytroMitin/scala3-macro-closure-demo) — Scala 3 macro experiments
* [macro-inline-demo](https://github.com/DmytroMitin/macro-inline-demo) — inline/macro experiments
* [compiler-plugin-demo](https://github.com/DmytroMitin/compiler-plugin-demo) — Scala compiler-plugin experiments
* [scalafix-codegen-demo](https://github.com/DmytroMitin/scalafix-codegen-demo) — source generation with Scalafix
* [scalameta-demo](https://github.com/DmytroMitin/scalameta-demo) — Scalameta experiments
* [macrosdemo](https://github.com/DmytroMitin/macrosdemo) — Scala macro experiments

## Talks

### [Can Scala 3 Have Macro Annotations Again? Rebuilding Macro Paradise](https://github.com/DmytroMitin/macroparadise-talk-09-2026)

My London Scala User Group talk on Scala 2 macros and quasiquotes, Scala 3 quotes/reflection and macro annotations, and the alternative pre-typer Macro-Paradise approach.

The repository contains the **talk text, slides, examples, and links to the related projects**.

## Upstream open-source work

Several repositories on this account are working forks used for upstream investigation and contributions rather than independent projects.

### Scala compiler

[`DmytroMitin/dotty`](https://github.com/DmytroMitin/dotty) — working fork of the Scala 3 compiler.

Selected compiler work:

* [scala/scala3#26002 — Fix `summonInline` deferred inline selection](https://github.com/scala/scala3/pull/26002)

### Shapeless

[`DmytroMitin/shapeless`](https://github.com/DmytroMitin/shapeless) — working fork used for type-level programming and macro contributions.

Selected PRs:

* [shapeless#1286 — support `Generic` materialized in a macro-generated companion of a nested case class](https://github.com/milessabin/shapeless/pull/1286)
* [shapeless#879 — fix `Witness` for `TypeRef` singleton types](https://github.com/milessabin/shapeless/pull/879)
* [shapeless#878 — fix `RotateLeft` / `RotateRight` for `Poly` with multiple cases](https://github.com/milessabin/shapeless/pull/878)
* [shapeless#859 — avoid diverging implicit expansion in HList folders](https://github.com/milessabin/shapeless/pull/859)

### Apache Spark

[`DmytroMitin/spark`](https://github.com/DmytroMitin/spark) — working fork of Apache Spark.

* [apache/spark#38740 — product encoders for local classes](https://github.com/apache/spark/pull/38740), involving Scala reflection, type tags, compile-time dealiasing, and encoder derivation.

### ProvingGround

[`DmytroMitin/ProvingGround`](https://github.com/DmytroMitin/ProvingGround) — working fork of the Scala theorem-proving / HoTT project.

Selected work includes:

* [ProvingGround#119 — induction from sum types](https://github.com/siddhartha-gadgil/ProvingGround/pull/119)
* [ProvingGround#112 — vector concatenation / induction](https://github.com/siddhartha-gadgil/ProvingGround/pull/112)
* [ProvingGround#114 — induction-family test follow-up](https://github.com/siddhartha-gadgil/ProvingGround/pull/114)

### ChatGPT Desktop for Linux

[`DmytroMitin/codex-desktop-linux`](https://github.com/DmytroMitin/codex-desktop-linux) — working fork of the community Linux port of ChatGPT Desktop.

Recent upstream work includes Linux-specific Computer Use and Chrome integration:

* [#1097 — fix Computer Use synthetic marketplace manifest path](https://github.com/ilysenko/codex-desktop-linux/pull/1097)
* [#1159 — adapt Computer Use to the monolithic renderer bundle](https://github.com/ilysenko/codex-desktop-linux/pull/1159)
* [#1286 — expose managed Node to the Chrome side-panel app-server](https://github.com/ilysenko/codex-desktop-linux/pull/1286)
* [#1308 — fix Chrome side-panel CLI trust selection](https://github.com/ilysenko/codex-desktop-linux/pull/1308)

### Other Scala ecosystem contributions

* [`avro4s`](https://github.com/DmytroMitin/avro4s) — [macro hygiene fix](https://github.com/sksamuel/avro4s/pull/590)
* [`json-facile`](https://github.com/DmytroMitin/json-facile) — [runtime-reflection / macro outer-accessor fix](https://github.com/readren/json-facile/pull/1)
* [`splain`](https://github.com/DmytroMitin/splain) — [quasiquote serialization fix for case objects](https://github.com/tek/splain/pull/95)
* [`dotty-macro-examples`](https://github.com/DmytroMitin/dotty-macro-examples) — [generic-class macro fix](https://github.com/lampepfl/dotty-macro-examples/pull/33)

## Mathematics & type theory

My background is in mathematics, and I have a long-standing interest in theorem proving, dependent type theory, and the interaction between mathematical structure and programming languages.

Some public repositories related to this work:

* [arend-exercises](https://github.com/DmytroMitin/arend-exercises) — experiments/exercises with Arend and dependent types
* [hott-cubicaltt-exercises](https://github.com/DmytroMitin/hott-cubicaltt-exercises) — Homotopy Type Theory / cubical type theory exercises
* [ProvingGround](https://github.com/DmytroMitin/ProvingGround) — theorem proving and HoTT work in Scala

## Elsewhere

* [Stack Overflow](https://stackoverflow.com/users/5249621/dmytro-mitin) — extensive Scala, type-level programming, macros, reflection, and FP answers
* [Scala course on Stepik](https://stepik.org/course/2294/promo)
* [All public repositories](https://github.com/DmytroMitin?tab=repositories)

---

[![Dmytro Mitin profile views](https://u8views.com/api/v1/github/profiles/12773417/views/day-week-month-total-count.svg)](https://u8views.com/github/DmytroMitin)
