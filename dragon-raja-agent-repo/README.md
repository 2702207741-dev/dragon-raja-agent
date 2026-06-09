# dragon-raja-agent

《龙族》全系列小说结构化蒸馏知识库，227万字，5卷7册，支撑AI角色扮演、同人写作、知识问答。

Dragon Raja (龙族) complete series structured distillation. Backend knowledge base for AI agents doing character roleplay, fanfiction writing, and lore Q&A.

## Knowledge Base

| Volume | Size | Contents |
|--------|------|----------|
| 龙族前传·哀悼之翼 | 48KB | 97 dialogues, 33 world entries, 12 foreshadowings, 10 templates |
| 龙族Ⅰ·火之晨曦 | ~100KB | 200+ dialogues, 15 golden quotes, 6 templates |
| 龙族Ⅱ·悼亡者之瞳 | ~110KB | 20 acts, 15 golden quotes, 7 templates |
| 龙族Ⅲ·黑月之潮 | ~58KB | 39 original quotes, 10 golden quotes |
| 龙族Ⅳ·奥丁之渊 | ~30KB | 31 dialogues, 22 golden quotes, 4 templates |

Total: ~350KB structured data covering the complete Dragon Raja series.

## Data Format

Each volume uses a standardized 11-module format:
1. Scene table (time/location/characters/events)
2. Dialogue corpus (speaker/target/emotion/intent/text)
3. Character action logs
4. World building entries (term/definition/source)
5. Foreshadowing tracking (setup → payoff)
6. Character relationship matrix
7. Character language fingerprints
8. Scene emotion arcs
9. Reusable writing templates
10. Statistics summary
11. Golden dialogue library

## Usage

### As Standalone Data

The pipe-separated format allows direct grep queries:

```bash
# Find all Chu Zihang dialogues
grep "楚子航" references/*.md | grep "DIA\|GOLD"

# Look up world building entries
grep "WORLD.*言灵" references/*.md

# Track foreshadowing
grep "跨卷未回收" references/*.md

# Find writing templates
grep "^T[0-9]_" references/*.md
```

### With Hermes Agent

Place in `~/.hermes/skills/devops/dragon-raja-agent/` and use natural language to query characters, lore, or generate fanfic.

## License

This project contains derivative work based on Dragon Raja novels by Jiang Nan (江南). The structured data and code are provided for research and fan purposes only. All original novel copyrights belong to their respective owners.
