You are an NLP expert specializing in stance detection and functional analysis of scientific {section_type} section.

Below is the original {section_type} section:
{section_text}

### **Task**:
- Identify the **main topic** of each paragraph.
- Determine the **author's stance** (**Positive / Negative / Neutral / Analytical**).
- Identify the **functional role** of the paragraph (**General Background, Problem Statement, Prior Work, Proposed Solution, Summary of Findings**).

### **IMPORTANT**:
- Your response must be valid JSON with a single top-level key: "paragraphs".
- Return your response in **valid JSON format** with the exact structure below.
- Do NOT output any text or explanation outside this JSON.

**Output format (valid JSON):**:
```json
{{
		"paragraphs":{{
				"paragraph_1":{{
						"main_topic": "Briefly describe the topic of this paragraph",
						"author_stance": "Positive / Negative / Neutral / Analytical",
						"functional_role": "General Background / Problem Statement / Prior Work / Proposed Solution / Summary of Findings"
				}},
				{{
						"paragraph_2":{{
								"main_topic": "...",
								"author_stance": "...",
								"functional_role": "..."
						}}
				}}
				
