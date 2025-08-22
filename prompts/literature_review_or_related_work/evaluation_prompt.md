You are a professional reviewer. You have been given two sections of a scientific paper:
1) Introduction (context only, do NOT evaluate it)
2) {section_2_type} (to be evaluated)

Use the introduction purely to understand the paper's background and scope. 
Only assess the {section_2_type} against the criteria listed below.

**IMPORTANT**:
- Your final answer MUST be valid JSON, without additional text or formatting outside the JSON structure.
- Follow the EXACT JSON key names and structure as shown below.

--------------------------------------------------------------------------------
Title of the paper:
{title}

Introduction (context only, not for evaluation):
{introduction_text}

{section_2_type} (to be evaluated):
{section_2_text}

--------------------------------------------------------------------------------
CRITERIA TO EVALUATE ({section_2_type.replace(' ', '')}Evaluation): 

1. ScopeAndFocusOf{section_2_type.replace(' ', '')} (Required)
2. ComprehensivenessAndDiversityOfSources (Required)
3. LogicalOrganization (Required)
4. CriticalAnalysisAndComparison (Required)
5. SynthesisOfPreviousFindings (Optional)
6. IdentificationOfResearchGaps (Required)
7. ConnectionToCurrentResearch (Required)
8. CitationAndReferencing (Optional)
9. ClarityAndConciseness (Required)
10. RelevanceAndJustification (Required)
11. ConcludingRemarksOrTransition (Optional)

--------------------------------------------------------------------------------
REQUIRED OUTPUT (valid JSON):
```
{{
		"ScopeAndFocusOf{section_2_type.replace(' ', '')}": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"ComprehensivenessAndDiversityOfSources": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"LogicalOrganization": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"CriticalAnalysisAndComparison": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"SynthesisOfPreviousFindings": {{
				"type": "Optional",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"IdentificationOfResearchGaps": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"ConnectionToCurrentResearch": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"CitationAndReferencing": {{
				"type": "Optional",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"ClarityAndConciseness": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"RelevanceAndJustification": {{
				"type": "Required",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}},
		"ConcludingRemarksOrTransition": {{
				"type": "Optional",
				"status": "Has" or "Has Not",
				"comment": "Short optional comment"
		}}
}}
