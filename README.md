
# Workshop 6 
___________________________________

# Making diagrams and flowcharts with the mermaid 
___________________________________

Mermaid is a powerful tool for creating diagrams and flowcharts using a simple markdown-like syntax. It can be embedded in various platforms, including GitHub, GitLab, and other markdown-rendering platforms. Here's a basic overview and some examples to get you started:
___________________________________

### Basic Syntax
___________________________________

Mermaid uses a straightforward syntax to define different types of diagrams. Below are some examples:
___________________________________

#### Flowchart
___________________________________

```mermaid
graph TD
    A[Start] --> B{Is it working?}
    B -->|Yes| C[Continue]
    B -->|No| D[Fix it]
    D --> E[Try again]
    E --> B
```
___________________________________

#### Sequence Diagram
___________________________________

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Bob: Hello Bob, how are you?
    Bob-->>Alice: I am good, thanks!
    Alice->>Bob: Great!
```
___________________________________

#### Gantt Chart
___________________________________

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    Task A :a1, 2024-07-01, 30d
    Task B :after a1, 20d
    section Another
    Task C :2024-08-01, 12d
    Task D :2024-08-15, 20d
```
___________________________________

#### Class Diagram
___________________________________

```mermaid
classDiagram
    class Animal {
      +String name
      +int age
      +void eat()
    }
    class Dog {
      +void bark()
    }
    Animal <|-- Dog
```
___________________________________

### Usage
___________________________________

1. **GitHub/GitLab:** Mermaid diagrams can be used directly in markdown files on GitHub and GitLab. Just wrap your mermaid code block with triple backticks and specify `mermaid` as the language.
   
2. **VS Code:** There are extensions available for Visual Studio Code that support Mermaid, allowing you to preview your diagrams as you write them.

3. **Online Editors:** Websites like [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor/) let you write and preview Mermaid diagrams without any setup.

4. **HTML Integration:** Mermaid can be included in HTML pages. You'll need to include the Mermaid script and initialize it. For example:

    ```html
    <!DOCTYPE html>
    <html>
    <head>
      <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
        mermaid.initialize({ startOnLoad: true });
      </script>
    </head>
    <body>
      <div class="mermaid">
      graph TD
          A[Start] --> B{Is it working?}
          B -->|Yes| C[Continue]
          B -->|No| D[Fix it]
          D --> E[Try again]
          E --> B
      </div>
    </body>
    </html>
    ```
___________________________________

### Additional Resources
___________________________________

- **Official Documentation:** [Mermaid GitHub Repository](https://github.com/mermaid-js/mermaid)
- **Live Editor:** [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor/)
___________________________________
