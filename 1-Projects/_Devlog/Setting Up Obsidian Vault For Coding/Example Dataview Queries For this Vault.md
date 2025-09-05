# Example Dataview Queries For this Vault

- **All Practice Notes by Language**:
    
    `   TABLE language, topic, status, last-practiced  FROM "1-Practice"  WHERE language  SORT last-practiced DESC       `
    
    _Output_: Lists all practice notes (e.g., from Coddy, SoloLearn) with their language, topic, etc., unaffected by emojis.
- **In-Progress Skills Notes**:
    
    `   TABLE language, topic, level  FROM "3-Skills"  WHERE status = "in-progress"  SORT level ASC       `
    
    _Output_: Shows active learning notes in 3-Skills/Languages/, like Python.md.
- **Snippets by Topic**:
    
    `   TABLE topic, language  FROM "4-Library/Snippets"  WHERE type = "snippet"  SORT topic ASC       `
    
    _Output_: Lists reusable snippets, grouped by topic (e.g., loops, functions).
- **Filter by Platform Tag**:
    
    `   TABLE file.name, language, topic  FROM ""  WHERE contains(tags, "coddy")  SORT file.name ASC       `