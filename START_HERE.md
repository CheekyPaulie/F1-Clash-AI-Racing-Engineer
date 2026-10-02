# START HERE - F1 Clash AI Racing Engineer

**v1.1 - 2 October 2026**  
**CheekyPaulie / Slipstream Boys**

The goal is simple: give your AI enough verified information about **your** account that it can make race recommendations from your real Drivers, Components and Boosts instead of generic online stats.

## 1. Pick your AI

### ChatGPT - recommended
1. Create a dedicated **Project** called `F1 Clash AI Racing Engineer`.
2. Add `MASTER_AI_PROMPT.txt` to the Project instructions or project files.
3. Upload `INVENTORY_TEMPLATE.xlsx`.
4. Upload your Driver, Component and Boost screenshots.
5. Ask ChatGPT to build/populate your inventory from those screenshots.
6. Keep future race conversations inside that Project.

### Claude / Gemini / Grok / another AI
Use the closest equivalent to a persistent Project, workspace, Gem, custom assistant, or dedicated conversation. Add the same `MASTER_AI_PROMPT.txt`, inventory workbook and screenshots. If the platform cannot reliably keep files between chats, reattach the current inventory when starting a new session.

**Important:** do not assume every platform can inspect a ZIP archive. If it cannot enumerate and read the individual images, extract and upload the relevant screenshots instead.

## 2. Capture your inventory

### Drivers
Capture each Driver card so the AI can read the name, card variant/rarity, level, and every displayed numeric attribute such as Overtaking, Defending, Qualifying, Race Start and Tyre Management.

### Components
Capture each Component with name/category, rarity, level and all displayed attributes such as Speed, Cornering, Power Unit, Qualifying, Overtake Mode/Battery and Pit Time. Do not expect the AI to invent exact values from unlabeled graphical bars.

### Boosts
Capture the Boost name, quantity owned and every displayed bonus. Power Unit, Boost Mode Impact, Boost Recharge Rate and Boost Mode Duration are separate fields and must not be mixed up.

### File naming - optional but useful
- `Drivers_YYYY-MM-DD.zip`
- `Components_YYYY-MM-DD.zip`
- `Boosts_YYYY-MM-DD.zip`
- `Driver_Update_NAME_YYYY-MM-DD.png`
- `Component_Update_NAME_YYYY-MM-DD.png`
- `Boost_Update_NAME_YYYY-MM-DD.png`

## 3. Build your personal catalog

Upload the screenshots and tell the AI:

> Build my F1 Clash inventory using the attached screenshots and `INVENTORY_TEMPLATE.xlsx`. Inspect every relevant screenshot you can actually access. Do not guess unreadable values. Record source filenames/dates and flag anything uncertain. A newer screenshot for one item updates only that item.

Keep the original screenshots as the evidence layer and the completed workbook as the fast lookup layer.

## 4. Test the setup before trusting it

Ask these five questions:

1. **What proves what I own?**  
   Expected: my newest verified screenshots/catalogs - not generic online stats.

2. **One Boost quantity changed. Does every Boost change?**  
   Expected: no, only that Boost.

3. **Can you claim a ZIP was reviewed just because I attached it?**  
   Expected: no. Individual relevant archive members must actually be inspected, or the AI must say it could not.

4. **Does a temporary +10% Grand Prix bonus become permanent?**  
   Expected: no. Baseline and event-adjusted values stay separate.

5. **What happens if one stat is unreadable?**  
   Expected: flag the missing value; never guess.

If the AI fails those tests, fix the setup before relying on it for an important GP.

## 5. Race day

Upload the race/event screenshot and use the appropriate prompt from `RACE_AND_UPDATE_PROMPTS.md`. For a full recommendation, the AI should give:

- Two eligible Drivers.
- Component setup/changes.
- **NEED TO WIN** Boost for each Driver.
- **ECONOMY** Boost for each Driver.
- Starting tyres and pit strategy.
- Important risks and any missing information.

For Grand Prix races, the objective is **maximum total points from both Drivers**, not merely beating the opponent.

## 6. Keep it current

When one Driver, Component or Boost changes, upload the newer screenshot and update only that item. When F1 Clash changes publicly, use current official Hutch information before relying on old guides or forum posts.

After every Grand Prix result, the AI should ask:

> **Boost used? A / B / C**

A = NEED TO WIN plan  
B = ECONOMY plan  
C = your own Boosts

That lets the system learn from the Boosts you actually used instead of assuming the recommendation was followed.

## Keep personal data private

The GitHub repository is for the blank toolkit. Your live inventory belongs in your own AI workspace. Do not upload your personal account screenshots or inventory to the public repository unless you intentionally want them public.
