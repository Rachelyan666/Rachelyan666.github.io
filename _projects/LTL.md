---
title: "LTL interpreter"
categories:
  - Software
tags:
  - Algorithm
  - OCaml
image: 
  path: /images/buchi.png
  thumbnail: /images/buchi_s.png
  caption: "buchi example diagram"
---

This project is a interpreter written by Ocaml that transfers a natural language that follows LTL rules into an automata graph.

This is a tool that can translate everyday language into something a machine understands. LTL logic, which is the Linear Temporal Language (LTL) will be transformed into Büchi Automata.

This converter takes in strictly-formatted human language, parses and synthesizes it into a simplified Linear Temporal Logic expression, and converts it into a reliable Büchi automaton that is visualized and verifiable. With the automaton being generated, the user is able to verify if their subsequent tentative actions is executable.

Github: <a href="https://github.com/JLjw8/LTL2Buchi">Interpreter</a>

![interpreter](/images/buchi.png)
