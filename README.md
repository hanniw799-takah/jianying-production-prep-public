# Jianying Production Prep

A Codex Skill for preparing repetitive Jianying / CapCut product-video projects before manual editing.

## What it does

The user provides:

- a product name;
- one mixed-edit script;
- three big-text-video scripts.

The Skill prepares:

- four distinct cover selling-point lines;
- three five-line ending groups;
- a lightweight advertising-copy compliance sanity check;
- semantic body-copy splitting with a visual choice between three or four lines;
- four configurable timeline names;
- template text replacement while preserving existing visual styling;
- a final stale-copy check.

## What it does not do

- automatic video editing;
- source-footage analysis;
- voice generation;
- smart packaging;
- BGM;
- cover-image selection or replacement;
- video export.

## Input example

```markdown
产品：示例酸奶

混剪：
这里是用户提供的混剪正文……

大字报：
1. 这里是用户提供的第一条正文……
2. 这里是用户提供的第二条正文……
3. 这里是用户提供的第三条正文……
```

The Skill preserves supplied scripts verbatim. It creates only the constrained cover and ending copy from facts present in the current input.

## Installation

```text
git clone <public-repository-url>
```

Open the cloned repository with Codex and confirm that the Skill exists at:

```text
.codex/skills/jianying-production-prep/
```

Then invoke it with the input format above.

## Customization

Jianying templates differ. On first use, let the Agent identify your own timeline names, cover compound clip, body and ending text slots, cover structure, and visual-style slots. Customize the timeline naming convention, creator/team placeholders, date format, product naming, text-slot structure, and cover structure for your workflow. The Skill does not claim universal compatibility with every Jianying template.

## Compliance notice

The included Compliance Gate is an auxiliary copy sanity check and does not constitute legal advice. Commercial publication remains the user's responsibility under applicable local laws, platform rules, and verified product documentation.

## Privacy

This public edition contains no company data, product assets, private project copies, credentials, or historical commercial copy.

## Version

`v1.0`

License: All rights reserved unless otherwise stated.
