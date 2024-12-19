# Fai Deisign.

Fai is built around the principle of fractal recursion. In contrast to traditional software engineering practices that
favor deterministic loops and end points, fai operates non deterministically over calssical and fractal knowledge structures,
the fidelity of the result depends on how many timecycles it has, with diminishing returns past some point.

At it's core, Fai is a wrapper around a recursive onedshot call to (any) LLM with the same system prompt.
The user prompt changes each time, updated outside of the LLM call, to reflect the output of the recursive call.
The system prompt contains instructions to read this and recursivley return modification deltas to it as output.

The key here is to have the LLM output a delta, a potential chat to some external system. The external system
applys the delta to update the state. This can happen until there is decision to stop the recursive call.

This is hybrid recursive-neural programming without a base case.

It is implemented through function-calling LLMs. It is beleived that the ability of an LLM to reliably read and output
structured data represents a critical boundary dimension for reasoning ability - being able to "think like a programmer"
indicates a latent representation for high level abstract reasnoning, or the ability to approach turning completness
through emergent non-deterministic systesms.

# External State

