# GitWhisperer: A Protocol for Precise Code Changes

## Overview

GitWhisperer is a collection of three complementary prompts designed for small-parameter LLMs to handle code changes with extreme precision. The system uses a strict token-based protocol that eliminates ambiguity and ensures consistent output.

## The Three Prompts

### 1. Code Change Compiler (CCC)
The foundational prompt that handles the core change generation with extreme precision.

**Key Features:**
- Token-based change blocks
- Exact code matching
- Unified diff generation
- Strict error handling
- Line-level precision

**Use When:**
- You have the original code
- Need precise changes
- Want minimal token usage
- Working with small LLMs

### 2. Code Request Processor (CRP)
The context gatherer that ensures we have the necessary code before making changes.

**Key Features:**
- Content type identification
- Standardized code requests
- Clear validation rules
- Specific error handling
- Type-aware requests

**Use When:**
- Need to gather code context
- Working with named functions/components
- Need to specify file targets
- Want to ensure complete context

### 3. GitWhisperer Unified (GWU)
The complete system that combines both request and change capabilities.

**Key Features:**
- Two-stage processing
- Complete verification
- Combined error handling
- Streamlined workflow
- Full example coverage

**Use When:**
- Need the complete workflow
- Want a single system prompt
- Working with a more capable LLM

## Usage Patterns

### Basic Change Request
```
User: Add error handling to processUser function
