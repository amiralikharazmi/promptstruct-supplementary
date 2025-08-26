{self.author_style_block}
{stance_info}

You are a writing assistant. Below is the introduction of a scientific paper and its abstract (for context only; 
do NOT rewrite the introduction and abstract). Then you will see the {section_2_type}, which is mostly 
acceptable but is missing or underdeveloping the following required criterion(s):


Missing required criteria:
{missing_str}

[ABSTRACT TEXT FOR CONTEXT - DO NOT MODIFY]
{self.abstract_text}

[INTRODUCTION TEXT FOR CONTEXT - DO NOT MODIFY]
{introduction_text if introduction_text else 'N/A'}

[{section_2_type.upper()} TEXT TO BE REWRITTEN]
{section_2_text}

**IMPORTANT**: 
- The corrected version **must follow** both of the stance analysis and author style profile results. Do not modify the author's stance or the functional structure of each paragraph.
- provide the rewritten section enclosed between `<{section_2_type.strip().replace(' ', '_')}>` and `</{section_2_type.strip().replace(' ', '_')}>` tags.

Instructions:
1. Use the introduction to understand the paper’s background, but do not alter the introduction text.
2. Insert or refine the parts of the {section_2_type} necessary to address the missing criterion(s).
3. Ensure that acronyms are defined only at their first occurrence and used in abbreviated form thereafter. Maintain an academic tone and logical flow
4. Ensure that the rewritten {section_2_type} does not contain unnecessary repetition of ideas or phrases.
5. Add a concluding summary: If not present, include a brief concluding paragraph that summarizes the key points of the {section_2_type} and highlights any research gaps.
6. Summarize overly detailed sections: Condense sections that are excessively detailed to maintain readability without sacrificing essential information.
7. Use varied transition phrases: Incorporate a diverse set of transition words and phrases (e.g., "Furthermore," "In addition," "Moreover") to enhance the flow of the text.
8.**Add citation symbol where needed**: Just use the symbol **[X]** where citations are missing (In the right place).
9.**discussion is lacking**: where discussion is lacking, Add your desired text and provide it in the format => **[Description: <discussion description>][Suggestion: <your desired text>]**.
10. **Preserve the author's technical style and voice** using this analysis:
- Tone (technical, procedural)
- Sentence structure (steps, logic)
- Vocabulary (domain-specific terms)
- Pacing (brevity vs. elaboration)
11. Check that all figure and table citations appear in ascending numerical order (e.g., Figure1 → Figure2 …). If any citation is out of sequence (e.g., Figure2 precedes Figure1), insert an inline note immediately after the first misplaced citation in the format: **[Note: Figure/Table numbering out of order — please swap Figure X with Figure Y to maintain sequence]**.
12. Avoid introducing bullet points or list formatting. Maintain paragraph-based structure throughout the section.
**Final Output Format:**        
As previously mentioned, Please provide just the rewritten section enclosed between `<{section_2_type.strip().replace(' ', '_')}>` and `</{section_2_type.strip().replace(' ', '_')}>` tags.
