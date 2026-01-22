# Phase 1: Information Science Boot Camp
>**Objective**: To learn the basics of information science and how it affects the organization of the web.

<details>
<summary>📅 Week 1: The Organizing System (The Logic)</summary>

### Study
>**Objective**: Understand that every collection — from a card catalog to a cloud database — shares the same logical DNA.

- **Core Reading**: [Robert J. Glushco, The Discipline of Organizing](https://yunus.hacettepe.edu.tr/~tonta/yayinlar/TDO-Ch1-discipline-of-organizing-glushko-chapter-1.pdf) (Chapter 1 only)  
  **Focus**: The "Organizing System" framework (Resources, Intentional Collection, Organizing Principles).
  
- **Secondary Reading**: [Marcia Bates, "The Invisible Substrate of Information Science"](https://pages.gseis.ucla.edu/faculty/bates/substrate.html).

>**Note:** You aren't learning about libraries; you are learning about the **Logic of Retrieval**. If you can't describe your data's "Organizing System," you can't build a reliable AI to query it.

### Synthesize - The "Organizing System" Audit
>**Objective**: Define the boundary and intent of your project.

**Task**: Create a System Manifesto for your data. In a single Markdown file, answer the following:

- **Selection**: Why are these specific resources being organized?  

- **Resources**: Are they physical, digital, or "composite"? What is their original format?

- **The Intentional Collection**: What is the "stopping rule"? When is a piece of data not part of this system?

- **Deliverable**: `SYSTEM_MANIFESTO.md` in your project root.
</details>

<details>
  <summary>📅 Week 2: Taxonomy & Ontology (The Structure)</summary>

  ### Study
  >**Objective**: Learn how to define relationships between concepts so that "Meaning" doesn't get lost.

**Reading**:
  - [Taxonomies Versus Ontologies: A Short Guide (Fluree Blog)](https://flur.ee/fluree-blog/taxonomies-versus-ontologies-a-short-guide/)
  - [The W3C SKOS Primer (Sections 1 & 2)](https://www.w3.org/TR/skos-primer/)
  - [From Taxonomy to Ontology (Enterprise Knowledge)](https://enterprise-knowledge.com/from-taxonomy-to-ontology/)

**Key Concepts**: 
- **Hierarchies**: Is a "Cat" always an "Animal"?
- **Polysemy**: How do we tell a computer that "Bank" means a river edge and not a vault?
  
  ### Synthesize - The Logic Tree
>**Objective**: Prove you can distinguish between a "type of thing" and a "relationship between things."

**Task**: Using your chosen data source, create a small **Knowledge Matrix** in Markdown.

- Identify 5 "Parent" Categories: (e.g., Characters, Locations, Themes, Time Periods).

- Map 3 "Child" Items for each: (e.g., Parent: Characters -> Children: The Shadow, The Mentor, The Stranger).

- Create 3 "Across-Tree" Relationships: This is the "Ontology" part. Instead of a hierarchy, you are mapping connections.

>Example: "The Shadow" (Character) appears_in "The Abandoned House" (Location).

- **Deliverable**: `TAXONOMY_v1.md`.

>**Pro Tip**: Use `Mermaid.js` inside your Markdown file to draw the tree. GitHub renders it automatically, and it makes your repo look incredibly high-end.
</details>
<details>
  <summary>📅 Week 3: Metadata Standards & Linked Data (The Language)</summary>
  
  ### Study
  >**Objective**: Learn how to describe resources so that machines can understand them.

**Reading**: 
- Explore the [Dublin Core Metadata Element Set](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). This is the "Universal Translator" of the web.
- Read the [W3C's Introduction to Linked Data](https://www.w3.org/DesignIssues/LinkedData.html).

>**The "Library" Bridge**: Understand that RDF (Resource Description Framework) is just a digital version of a library card catalog. It uses "Triples" (Subject -> Predicate -> Object) to create a web of facts.
  
  ### Synthesize - The Metadata Profile
  **Objective**: Define the standard "tags" that will be attached to every piece of info.

**Task**: Create a Metadata Schema using a "Dublin Core" hybrid. For your data source, define the following 5 mandatory fields:

1. **Identifier**: How will you uniquely ID a single entry? (e.g., YYYY-MM-DD-01).

2. **Temporal**: The timestamp or era.

3. **Provenance**: Where did this specific entry come from? (e.g., "Physical Journal Vol. 4").

4. **Semantic Tag**: One tag from your Week 2 Taxonomy.

5. **Relational Link**: A field for a "Subject-Predicate-Object" link (e.g., "Dream_A" mentions "Person_B").

**Deliverable**: `DATA_DICTIONARY.md` (A table defining these fields and their data types).
</details>
<details>
  <summary>📅 Week 4: Information Architecture for Retrieval (The Execution)</summary>
  
  ### Study
>**Objective**: Mapping the theory onto modern computer systems.

**Reading**: 
- [Dan Brown, The Eight Principles of Information Architecture](https://asistdl.onlinelibrary.wiley.com/doi/10.1002/bult.2010.1720360609)
- (Need a good resource on semantic search)
   
### Synthesize - The "Gap Analysis" (Search vs. Discovery)
>**Objective**: Prove the need for your advanced architecture.

**Task**: Perform a Retrieval Stress Test.

1. **The "Keyword" Query**: Try to find a specific concept in your raw data using a simple "Ctrl+F" search (e.g., searching for the word "Fear"). Note how many irrelevant results you get.

2. **The "Architectural" Query**: Write a natural language question that a keyword search cannot answer (e.g., "How does the sentiment of my dreams shift when I am living in a specific city?").

3. **The Solution**: Explain in 3 sentences how your Knowledge Graph (Phase 3) will solve this.

**Deliverable**: `RETRIEVAL_STRATEGY.md`.
</details>
