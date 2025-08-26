{self.author_style_block}
{stance_info}    

You are a writing assistant. Below is an introduction to a scientific paper that is mostly 
acceptable but is missing or underdeveloping the following required criterion(s):

**Missing required criteria:**
{missing_str}

[ABSTRACT TEXT FOR CONTEXT - DO NOT MODIFY]
{self.abstract_text}

[ORIGINAL INTRODUCTION TEXT]
{introduction}

**IMPORTANT**: 
- The corrected version **must follow** both of the stance analysis and author style profile results. Do not modify the author's stance or the functional structure of each paragraph.
- Provide the rewritten introduction enclosed between `<INTRODUCTION>` and `</INTRODUCTION>` tags

**Instructions:**
1. Address each missing or underdeveloped criterion by adding or revising brief sections.
2. Ensure a **smoother, more engaging, and professional academic tone**.
3. Improve fluency by enhancing transitions, restructuring long sentences, and removing redundancy.
4. Use varied sentence structures and precise word choices to enhance readability.
5. Ensure acronyms are defined only at their first occurrence and used in abbreviated form thereafter.
6.**Add citation symbol where needed**: Just use the symbol **[X]** where citations are missing (In the right place).
7. **Preserve the author's technical style and voice** using this analysis:
- Tone (technical, procedural)
- Sentence structure (steps, logic)
- Vocabulary (domain-specific terms)
- Pacing (brevity vs. elaboration)
8. Check that all figure and table citations appear in ascending numerical order (e.g., Figure1 → Figure2 …). If any citation is out of sequence (e.g., Figure2 precedes Figure1), insert an inline note immediately after the first misplaced citation in the format: **[Note: Figure/Table numbering out of order — please swap Figure X with Figure Y to maintain sequence]**.
9. Avoid introducing bullet points or list formatting. Maintain paragraph-based structure throughout the section.
**Final Output Format:**
Provide the rewritten introduction enclosed between `<INTRODUCTION>` and `</INTRODUCTION>` tags.
