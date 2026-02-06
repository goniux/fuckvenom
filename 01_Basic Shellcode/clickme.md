🧪 Custom Shellcode Experiment — MessageBox Payload

As part of understanding shellcode fundamentals, I created a simple custom Windows shellcode that displays a message box.
To test it in a realistic scenario, I integrated the shellcode into a legitimate executable (putty.exe) using a PE code-injection approach. The modified binary executed successfully and triggered the payload as expected.

This experiment was purely educational and done in a controlled lab environment.

🤔 Why Write Custom Shellcode Instead of Using Tools?

While frameworks like Metasploit or automated payload generators are convenient, relying only on them can limit deeper understanding.

Some key reasons for building shellcode manually:

1. Learning Depth

Automated payloads abstract away critical details:

Memory execution flow

Calling conventions

Windows API interaction

Binary structure nuances

Understanding these fundamentals builds stronger exploitation skills.

2. Flexibility & Customization

Handwritten shellcode allows:

Environment-specific adjustments

Payload optimization

Greater control over behavior

This is especially important when working with constrained or unusual targets.

3. Reduced Tool Dependency

Over-reliance on automation can:

Slow skill development

Limit problem-solving ability

Reduce understanding of underlying mechanisms

Manual experimentation helps build engineering intuition.

4. Detection Awareness

Common automated payloads may be easier to detect due to:

Known patterns

Reused structures

Signature-based detection

Studying shellcode internals also helps understand how defenders identify malicious behavior.

🧠 Position-Independent Code (PIC)

While exploring shellcode development, I encountered the concept of Position-Independent Code (PIC) — a fundamental principle in shellcoding.

Key ideas:

Code must execute correctly regardless of memory location

Absolute addressing is avoided

Dynamic resolution of APIs is often required

PIC enables shellcode to remain portable and functional across varying execution contexts.

📚 Primary Learning Influence

For this experiment, I followed research and notes from the ired.team knowledge base, which provided strong foundational insights into:

Windows shellcode structure

PIC implementation concepts

Practical debugging workflows

Additional independent experimentation and analysis were performed to reinforce understanding.

🧠 Key Takeaways From This Exercise

Writing shellcode manually improves understanding of low-level Windows behavior.

Position-independent code is essential for reliable payload execution.

Debugging and experimenting provided deeper insight than automated tooling alone.

Combining offensive experimentation with defensive awareness is critical for well-rounded security expertise.

📎 Resources
1) https://www.ired.team/offensive-security/code-injection-process-injection/writing-and-compiling-shellcode-in-c#c-shellcode.cpp
2) https://www.ired.team/offensive-security/code-injection-process-injection/backdooring-portable-executables-pe-with-shellcode
3) https://youtu.be/wDKagbDJC38?si=NZnDhwcbGix0VsbK
4) https://vxug.fakedoma.in/papers/VXUG/Exclusive/FromaCprojectthroughassemblytoshellcodeHasherezade.pdf   (USE WAYBACK MACHINE TO FIND THE PDF)
