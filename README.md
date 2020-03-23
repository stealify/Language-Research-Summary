# Language-Research-Summary
A Collections of facts about Polyglot Application Optimization and Coding Language Research 2020

## JIT vs AOT
- It turns out that AOT Compiled Languages perform better on startup and they are fast in general
- It turns out that JIT Can outperform AOT in a lot of cases it does that via Optimization of the code while it is running
- It also can be sayed that if the AOT Software would be written as optimized as the result from JIT it would Outperform JIT
- Optimizing pre build AOT Code is relativ hard and not so easy do able in general.
  - The biggest Problem of AOT is that it gets not Optimized for the Machine it is running on.
- With a lot of user code that is not optimized JIT Outperforms AOT.
- JIT has Higher Startup time and also a Warmup Time.
- GC is one of the most big places to Optimize in JIT Languages.

## Definition
- node === node + llhttp + js
- es4x === node-graalvm + vertx-web +js
- esax === deno + actix + js

## Examples and results
- es4x outperforms node
- esax outperforms es4x

## Development Time
- node - Lowest development time as of now (c++,wasm)
  - It is possible that wasm can superseed the c++ bindings
- deno - evolving could lead to be the prefered way to run JS
- rust + wasm is probally the future and running it via wasmer or a other wasi wasmi-bindgen

# Why Rust and WebAssembly + ECMAScript / Javascript?
Low-Level Control with High-Level Ergonomics
JavaScript Applications struggle to attain and retain reliable performance. JavaScript's dynamic type system and garbage collection pauses don't help. Seemingly small code changes can result in drastic performance regressions if you accidentally wander off the JIT's happy path.

Rust and WAs gives programmers low-level control and reliable performance. It is free from the non-deterministic garbage collection pauses that plague JavaScript. Programmers have control over indirection, monomorphization, and memory layout.
as also other low level language flavors.

near any static language can compile to wasm

and wasm runtimes that support wasi allow it to use low level hardware access. So it is Really Polyglot. It Replaces Java for sure over the next decade of years.

