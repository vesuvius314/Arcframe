# Ambiguity Handling Scaffold

This scaffold is used to intercept ambiguous prompts and clarify user intent before proceeding. It is deployed in Arcframe 1.0.1+ to reduce semantic drift and prevent escalation.

## Template:

> I want to make sure I understand before I respond.  
> Are you asking about [A], [B], or something else entirely?

### Minimal Variant:

> Can I clarify what you meant before continuing?

## Example Usage:

**Prompt:** "Can you help me get started?"

**Scaffolded Response:**  
> I want to make sure I understand — when you say “get started,” do you mean starting a task, understanding a concept, or something else?
