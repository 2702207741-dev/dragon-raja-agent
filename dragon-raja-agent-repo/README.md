     1|# dragon-raja-agent
     2|
     3|《龙族》全系列小说结构化蒸馏知识库，227万字，5卷7册，支撑AI角色扮演、同人写作、知识问答。
     4|
     5|Dragon Raja (龙族) complete series structured distillation. Backend knowledge base for AI agents doing character roleplay, fanfiction writing, and lore Q&A.
     6|
     7|## Knowledge Base
     8|
     9|| Volume | Size | Contents |
    10||--------|------|----------|
    11|| 龙族前传·哀悼之翼 | 48KB | 97 dialogues, 33 world entries, 12 foreshadowings, 10 templates |
    12|| 龙族Ⅰ·火之晨曦 | ~100KB | 200+ dialogues, 15 golden quotes, 6 templates |
    13|| 龙族Ⅱ·悼亡者之瞳 | ~110KB | 20 acts, 15 golden quotes, 7 templates |
    14|| 龙族Ⅲ·黑月之潮 | ~58KB | 39 original quotes, 10 golden quotes |
    15|| 龙族Ⅳ·奥丁之渊 | ~30KB | 31 dialogues, 22 golden quotes, 4 templates |
    16|
    17|Total: ~350KB structured data covering the complete Dragon Raja series.
    18|
    19|## Data Format
    20|
    21|Each volume uses a standardized 11-module format:
    22|1. Scene table (time/location/characters/events)
    23|2. Dialogue corpus (speaker/target/emotion/intent/text)
    24|3. Character action logs
    25|4. World building entries (term/definition/source)
    26|5. Foreshadowing tracking (setup → payoff)
    27|6. Character relationship matrix
    28|7. Character language fingerprints
    29|8. Scene emotion arcs
    30|9. Reusable writing templates
    31|10. Statistics summary
    32|11. Golden dialogue library
    33|
    34|## Usage
    35|
    36|### As Standalone Data
    37|
    38|The pipe-separated format allows direct grep queries:
    39|
    40|```bash
    41|# Find all Chu Zihang dialogues
    42|grep "楚子航" references/*.md | grep "DIA\|GOLD"
    43|
    44|# Look up world building entries
    45|grep "WORLD.*言灵" references/*.md
    46|
    47|# Track foreshadowing
    48|grep "跨卷未回收" references/*.md
    49|
    50|# Find writing templates
    51|grep "^T[0-9]_" references/*.md
    52|```
    53|
    54|### With Hermes Agent
    55|
    56|Place in `~/.hermes/skills/devops/dragon-raja-agent/` and use natural language to query characters, lore, or generate fanfic.
    57|
    58|## License
    59|
    60|This project contains derivative work based on Dragon Raja novels by Jiang Nan (江南). The structured data and code are provided for research and fan purposes only. All original novel copyrights belong to their respective owners.
    61|