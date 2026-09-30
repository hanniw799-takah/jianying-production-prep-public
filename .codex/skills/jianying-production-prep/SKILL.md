---
name: jianying-production-prep
description: Prepare Jianying/CapCut product-video projects before manual editing by preserving supplied scripts, generating constrained cover and ending copy, replacing template text, renaming timelines, and checking stale copy. Use for Production Prep, not footage editing, voice generation, music, image replacement, or export.
---

# Jianying Production Prep v1.0

## Scope and input

Input is a product name, one mixed-edit script, and three big-text-video scripts. Preserve every user-supplied script verbatim. Generate only the four cover selling-point lines and three ending groups.

On an ordinary new task, read only the current user input and this file. Read a saved Copy Pack only when resuming interrupted work. Do not load unrelated editing playbooks, footage indexes, historical product files, or automatic-editing skills unless the user requests those separate tasks.

Work only on text and four business-timeline names. Do not analyze footage, build an asset index, select or trim clips, generate voice, run smart packaging, add BGM, replace cover images, export video, or modify the user's original master template.

Priority: (1) current user text and explicit facts; (2) the user's existing template structure and visual styling; (3) AI-generated helper copy. Never change supplied product names, numbers, prices, ingredients, origins, specifications, promotions, after-sales terms, or other facts.

## First-use template mapping

Jianying templates are user-specific. On the first run for a template, identify and record the user's own:

- cover timeline and cover compound clip (`<cover-compound-clip>`);
- four business timelines;
- up to four body-text slots in each big-text template;
- five ending-text slots;
- product-name slot and four rotating cover-copy slots;
- visual slots, animations, arrows, blur endings, CTA layout, and other elements that must be preserved.

After this mapping is confirmed, reuse the fixed path on later runs. Do not assume a specific compound-clip name or identical slot layout across all templates.

## Text phase

Complete the full text phase before entering Computer Use; do not improvise copy inside the GUI.

1. Record all supplied scripts exactly. Store the mixed-edit script in the Copy Pack only; do not put it on a timeline or run voice generation.
2. Generate four distinct cover lines. Prefer `四字短语 四字短语` with exactly one ordinary space, no joining punctuation, and no repeated product name. Use different factual angles when available; if facts are limited, rephrase existing facts without inventing a fourth claim.
3. Generate exactly five ending lines for each big-text script. Keep each line around eight Chinese characters, make the three groups meaningfully different, and continue the corresponding scenario. Parallel phrases use exactly one ordinary space. Line five may be a natural CTA, but must not invent discounts, gifts, limited-time claims, scarcity, or pricing mechanisms.
4. Initially split each big-text script into three or four complete semantic blocks. Only insert breaks and assign slots; never replace, add, delete, summarize, or upgrade the wording.
5. Run the Compliance Gate, then create one Copy Pack for the task.

## Compliance Gate

AI-generated copy may use only facts explicitly provided in the current request. It may compress wording but must not upgrade meaning; for example, `没有额外添加蔗糖` must not become `无糖`.

Do not invent ingredients, origins, specifications, nutrition data, testing, certifications, quantities, prices, promotions, inventory, or sales claims. For ordinary foods, do not add disease, treatment, weight-loss, stomach-care, liver-care, sleep, immunity, or similar health claims. Avoid unsupported absolutes and superlatives such as `最佳`, `第一`, `顶级`, `全网最低`, `百分百`, or `绝对`.

Before opening the GUI, verify:

- supplied scripts are unchanged;
- four cover lines are distinct and use a single separator space;
- each ending group has exactly five lines and matches its own scenario;
- no new facts, altered numbers, health claims, absolutes, or semantic upgrades appear.

Regenerate AI-created text that fails. If supplied user text appears risky, do not silently modify it; report `⚠️ 文案合规提示：……，当前未自动修改。` and wait for the user's decision. Record `Compliance: PASS` or `Compliance: REVIEW — <specific text>`.

This is an auxiliary copy sanity check, not legal advice. The user remains responsible for review under applicable laws, platform rules, and verified product documentation.

## Dynamic three/four-line body layout

A template may provide four body slots, but the final body may use three or four lines. Do not prefer either count in advance. After filling the initial semantic split, move the playhead to a point where the full body is visible and judge the real preview.

Use four lines when all four blocks are semantically complete, widths are balanced, and no isolated short line appears. Use three lines when forcing four would create fragments, an isolated short line, or a conspicuous length jump. Never add words merely to fill a slot.

Check line widths, isolated lines, outer silhouette, and visual center. Assign scenario/problem, product/feature, and emphasis/closure to the most suitable existing style slots. When using three lines, choose the best three slots rather than mechanically keeping the first three. Remove only the unused body-text object; do not touch ending text, blur elements, arrows, effects, or video tracks. Fix poor layout only by changing semantic breaks and slot assignment, never the source sentence.

## Timeline naming

Use a configurable pattern instead of a fixed personal or company convention:

- `日期-产品名1-创作者名-团队名`
- `日期-产品名2-创作者名-团队名`
- `日期-产品名3-创作者名-团队名`
- `日期-产品名4-创作者名-团队名`

Mapping: `1` = mixed edit, `2` = big-text video 1, `3` = big-text video 2, `4` = big-text video 3. The user may customize creator name, team name, date format, product naming, separators, and whether the cover timeline keeps its original name. Confirm the convention during first-use template mapping, then reuse it.

## Computer Use phase

Operate only on the current product project or a user-designated template copy. Never enter or overwrite the original master template.

1. Rename the four business timelines in the safest order for the current UI; inspect the final list once.
2. Complete each big-text timeline as one batch: fill body text, remove any unused body slot, fill five ending lines, preview once in the fully visible middle section, then adjust the three/four-line split and style-slot assignment if needed. Do not capture screenshots or read the full accessibility tree after every line.
3. Enter the cover compound clip once, then replace the product name and Cover 1–4 consecutively. Inspect the full cover once. Preserve images, layout, gradients, animations, and other existing visual elements.
4. Perform one final check of timeline names, unchanged source wording, ending line counts, cover differences, and stale product text. Remove stale temporary product text from the mixed-edit timeline, while leaving the new mixed-edit script in the Copy Pack only.

Use real keyboard input or paste events that trigger the editor's commit behavior; do not rely only on programmatic value assignment. After multiline paste, click another object to commit rather than using Tab. If a paste times out, inspect the field before retrying so text is not duplicated.

Reuse the same session, current state, and differential accessibility output. Use screenshots only for visual layout decisions. Normal runs should avoid rediscovering fixed paths. Read [UI Recovery](references/ui-recovery.md) only when a timeline is missing, the UI changed, paste state is unclear, or the connection was interrupted.

## Final report

Report only the product, four cover lines, final three/four-line splits with their five-line endings, four timeline names, whether stale product text remains, and Compliance PASS/REVIEW. Omit tool logs, execution diaries, long self-checks, and repeated rules.
