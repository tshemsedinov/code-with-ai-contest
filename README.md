# Code with AI contest

> Implementation of Timestamp 48 bit with AI

- **Deadline:** 31 Aug 2025 (23:59 GMT+3)
- **Language:** JavaScript with Web API or Node.js API (do not use npm dependencies)
- **Runtime:** Any browser, Node.js, Deno, Bun (or other JavaScript engine)
- **Focus:** Performance and maintainability
- **Prizes:** best performance wins a free seat in one of my courses (Node.js, Async programming, Patterns, Architecture). Metarhia alumni may also win an extra free seat. So I will give two free seats for two winners.

## Task

- Build the fastest, correct, and well-engineered **48-bit timestamp** generator (UUIDv7-style timestamp field)
- Encode generated timestamp in Base64URL format, so we will get 8 characters timestamp containing 48-bit timestamp
- Focus on performance and maintainability
- You must use AI tools to write all code, and may not hand-code the solution yourself
- Keep a **Prompts Log**: every instruction to AI tools (full text), model names/versions
- Provide exact **setup** to reproduce (OS, Node version, npm versions, hardware, env vars)
- If you use multiple AI tools, document the pipeline (who generated what, in which order)
- Add unittests, typings, docs
- Warning: Do not fork this repo, to prevent others watching your code
- Your submission must be under a permissive license (MIT/ISC/BSD-2/Apache-2.0)
- [Submit your solution](https://forms.gle/hLw5fyWPFZparioy8)

## Hints

- Find RFC with **Base64URL** specs or AI tool can find it. **Base64URL** alphabet: `A–Z a–z 0–9 - _`
- Padding: No padding (`=` removed)
- Length: 6 bytes to 8 Base64URL chars, you can find RFC with Base64URL specs as well
- Provide a **public Github repo** URL in your submission

Proposed repo structure:
```
.
├─ package.json
├─ README.md            # this file
├─ timestamp.js         # export generateTimestamp48()
├─ timestamp.d.ts       # TypeScript declarations for public API
├─ timestamp.test.js    # correctness & edge cases
├─ AI_PROMPTS.md        # full prompt/response logs
└─ SETUP.md             # OS, env, Node, CPU, RAM, Node flags, etc.
```

**Good luck!**
