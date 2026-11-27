# Campaign Ledger
Static character sheet for the expanded 2024 D&D campaign. No dependencies, backend or build step.

## GitHub Pages
1. Create a GitHub repository (for example `campaign-ledger`).
2. Upload `index.html`, `style.css`, `app.js`, and this README to the root of the main branch.
3. In Settings → Pages, select Deploy from a branch, main, / (root), and Save.
4. Open the Pages URL shown by GitHub.

Characters are saved in localStorage in the current browser and origin. Export JSON regularly; import adds copies rather than overwriting. Players on different devices do not share data. Print prints the current section. Class and species features, HP, effective caster level, prerequisites and supplemental progression are manually tracked; no licensed sourcebook text is bundled. The default new character is a level 3 Fighter placeholder; change it in Classes. Point buy is validated visually, not enforced. Skill proficiency selectors use 0/1/2. The sheet is not a complete rules engine.

## v1.2
Adds subclass suggestions from the campaign working catalog, combat dice rolls with advantage/disadvantage and history, and milestone advancement with manually entered HP gain. Existing local storage key and JSON schema remain compatible. Catalog names are suggestions, not a verified rules database. Replace all four files when updating.

## v1.3
Adds spell slot expenditure, cast history, configurable resources, rest actions and a searchable class/subclass library with custom entries. Existing local storage key is unchanged. Hit Dice recovery, prerequisites, preparation, special rest rules and concentration remain manual. Export a backup before upgrading. No external rules database is bundled.

## v1.4 Automatic statistics
Open Automatic statistics and enable HP, AC and magic calculations individually. Existing characters default to manual. Fixed-average HP assumes the first listed class was taken first. Third-party hit dice must be entered in Classes; third-party caster contributions and special AC formulas require overrides. Export a backup before enabling automation. No live browser testing performed.

## v1.5
Combat automation tab: calculated weapon attacks, finesse, proficiency, magic bonuses, optional melee flanking, normal and Crunchy Critical damage, temporary HP, healing and death saves. Damage resistance, massive damage, critical damage at zero HP, potion inventory consumption and special features remain manual. Existing storage key unchanged.

## v1.6
Opt-in Character features tab: core backgrounds, starting class saves, Tough, selected armor, selected class resources and feature summaries. Manual third-party effects remain supported.

## v1.7
Origins & heritage tab: opt-in core background ability allocations, species speed and vision reference, heritage selection budget, class skill grants, Tough detection, defense records and level-gated custom subclass records. Remove duplicate manual background bonuses before enabling. Third-party effects and prerequisites are not encoded. Existing save key retained.

## v1.8 Mechanical effects
New Mechanical effects tab: reversible per-character effects with optional class-level gates. Supports ability scores, proficiency/expertise, saves, HP/AC, initiative, speed, spell and weapon modifiers, and defense records. Use exact target names or All. Enable manually when applicable; no automatic attunement or condition evaluation. Numeric effects stack, so avoid duplicates. HP/AC require automatic statistics. Existing storage key unchanged.
