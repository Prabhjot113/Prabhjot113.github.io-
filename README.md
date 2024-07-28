
# Workshop 6 
___________________________________

# Making diagrams and flowcharts with the mermaid 
___________________________________

**Introduction to mermaid**

Mermaid is a Javascript based powerful tool for creating diagrams and flowcharts using a simple markdown-like syntax. 
Mermaid diagrams are supported natively on several platforms which means you can directly use mermaid Syntex without additional extensions.Some of the key platforms include:-

## GitHub:
It supports mermaid diagrams in markdown files (.md) and in issues, pull requests and comments.

## Visual studio code (VS CODE)
With "Markdown Preview Mermaid Support" extension, you can view mermaid diagrams in VS Code.

Other platforms are :- GitLab, Obsidian, Joplin, Notion, etc.

Mermaid allows even non-programmers to easily create detailed through the Mermaid Live Editor.
For a more detailed introduction to mermaid look to the beginner's Guide, usage and tutorials.
____________________________________

### Basic Syntax
____________________________________

Mermaid uses a straightforward syntax to define different types of diagrams. Below are some examples:
____________________________________

#### Flowchart 
____________________________________

```mermaid
graph TD
    A[Start] --> B{Am I visible?}
    B -->|No| C[check it again]
    B -->|Yes | D[now continue]
    D --> E[Try again]
    E --> B
```
____________________________________
