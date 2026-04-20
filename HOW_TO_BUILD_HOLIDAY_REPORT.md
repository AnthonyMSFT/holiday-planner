# 🏖️ How to Build a Holiday Activities Report with Copilot CLI
## A step-by-step guide to creating an interactive, filterable holiday planner

---

## What You'll End Up With

An interactive HTML report with:
- Every activity available at your destination, with descriptions and booking links
- Filterable by activity type, cost, child age suitability, and more
- Cost estimates for each activity
- "Must-do" highlights marked
- Dynamic map with pins for every activity (filter-synced!) and accommodation overlay
- Weather summary for your travel month
- Country navigation bar linking all your destination reports
- Permanently hosted on GitHub Pages — free, shareable URL
- Themed in your favourite colours

---

## Prerequisites

- **GitHub Copilot CLI** installed and running
- A rough idea of where you want to go (or let Copilot help you decide!)

---

## Step 1: Set the Scene

Tell Copilot about your family, preferences, and constraints. The more context you give upfront, the better the results.

### Example Prompt:
```
I'm planning a family holiday for summer 2026. We are a family of 2 adults 
and 3 children aged 17, 15 and 8. We prefer to fly from [YOUR AIRPORT]. 
We like outdoor adventures, beaches, aqua parks, and cultural experiences. 
We've enjoyed [PAST HOLIDAYS] in the past. Our budget is roughly 
£[AMOUNT] for the whole trip.
```

---

## Step 2: Pick a Destination

Ask Copilot to research flight routes and suggest destinations that match your interests. Be specific about what matters to you.

### Example Prompt:
```
Research which destinations we can fly to directly from [YOUR AIRPORT]. 
We want somewhere with outdoor activities suitable for all ages, 
good beaches or lakes, and interesting culture. Suggest the best 
options and explain why each one works for our family.
```

### Follow-up to narrow down:
```
I like the sound of [DESTINATION]. What would a 2-week holiday 
there look like? What are the main things we could do?
```

---

## Step 3: Research Activities

Once you've picked a destination, ask Copilot to find every possible activity. Push for quantity — you can filter later.

### Example Prompt:
```
List as many activities as you can find for a family holiday in 
[DESTINATION]. Include: adventure activities, water sports, nature 
experiences, cultural visits, markets, food experiences, unique/unusual 
experiences, scenic drives, swimming spots, and anything memorable.

For each activity note:
- What it is (brief description)
- Approximate location
- Whether it's suitable for children aged [AGES]
- Approximate cost
- Any booking links or websites
```

### Push for more:
```
Find more activities we haven't thought of but that the kids will 
remember. Think about things like: [via ferrata, paragliding, 
underwater trails, treasure hunts, steam trains, stargazing, 
food tours, bungee jumping, boat hire, alpine coasters, etc.]
```

---

## Step 4: Build the HTML Report

This is where the magic happens. Ask Copilot to create an interactive, filterable HTML report from all the activities.

### Example Prompt:
```
Create an attractive HTML report with all these activities. Include:

- A hero banner at the top with the destination name and activity count
- A "Top 10 Unmissable" highlights section
- Summary stats showing activity counts by category
- A sticky filter sidebar that lets me filter by:
  - Area/location
  - Activity type (water, adventure, culture, etc.)
  - Suitable for which children (by age)
  - Cost (free, budget, mid-range, premium)
  - Must-do highlights only
- Each activity as a card showing:
  - Description
  - Child suitability tags (colour-coded)
  - Cost badge
  - Link to booking/info website
  - Whether it's a must-do highlight
- A count showing "Showing X of Y activities" that updates as I filter
- Make it mobile-responsive
- Use [COLOUR SCHEME] colours

Save it to [FILE PATH]
```

---

## Step 5: Customise the Look

Make it personal! Ask Copilot to theme it to your favourite team, brand, or colours.

### Example Prompt:
```
Update the colour scheme to match [TEAM/BRAND NAME] — 
check their website at [URL] for the exact colours and fonts.
```

---

## Step 6: Add a Map, Weather & Accommodation

Enhance the report with geographic context and practical info.

### Example Prompt:
```
Add a dynamic interactive map showing every activity as a pin. 
Must-do activities should be orange, others blue. The map should 
respond to the sidebar filters — when I filter by "free", only 
free activities show on the map. Add a scrollable table below 
the map with "More Info" and "Map" links for each activity.

Also overlay accommodation markers (Eurocamp, eco-lodges, resorts) 
in green, with a toggle to show/hide them.

Add a weather summary section showing typical August conditions: 
temperature, sunshine hours, rainy days, sea temperature, and 
any warnings (hurricanes, typhoons, rainy season, extreme heat).
```

---

## Step 7: Host on GitHub Pages (Free & Permanent)

Push your reports to a GitHub repo and enable GitHub Pages for a free, permanent URL.

### Example Prompt:
```
Set up a GitHub repository for this project. Push all the HTML 
reports, images, and assets. Enable GitHub Pages so the site 
is hosted at [USERNAME].github.io/[REPO-NAME]/

Update all internal links to work with the GitHub Pages URL.
```

### To update after changes:
```
Push the latest changes to the GitHub repo so the live site updates.
```

### Alternative: Quick sharing with devtunnel
If you just need a temporary link for a demo or presentation:
```
Host this locally and create a devtunnel link so I can share it 
temporarily. Generate a QR code for the link.
```

---

## Tips for Best Results

1. **Be specific about your family.** Ages matter — Copilot will flag activities 
   that are too old or too young for each child.

2. **Mention past holidays.** This helps Copilot understand your style 
   (resort vs adventure, all-inclusive vs self-catering, etc.)

3. **Push for more activities.** The first list is never complete. Ask 
   "what else?" and suggest specific categories to explore.

4. **Ask for booking links.** Copilot will try to find official websites 
   for each activity — much more useful than just a name.

5. **Request cost estimates.** Even rough per-person costs help you plan 
   a budget and compare activities.

6. **Iterate on the report.** You can ask to add filters, change colours, 
   add a legend, or restructure the layout after the first version.

7. **Don't forget the QR code.** It's a small touch that makes sharing 
   with the family effortless.

---

## The Whole Process in One Session

If you want to do it all in one go, here's a combined prompt to get 
you started:

```
I'm planning a 2-week family holiday to [DESTINATION] in [MONTH YEAR]. 
Our family is [DESCRIBE FAMILY AND AGES]. We fly from [AIRPORT].

Please:
1. Research all available activities in the area — aim for 60+ 
   covering adventure, water, culture, food, nature, and anything 
   unique or memorable
2. For each activity, note: description, location, child suitability 
   by age, approximate cost, and a booking link
3. Build an interactive HTML report with:
   - Filterable sidebar (type, cost, child suitability, must-do)
   - Cost badges on every activity
   - Top 10 highlights section
   - Mobile-responsive design
   - [COLOUR SCHEME] theme
4. Host it via devtunnel and generate a QR code to share

Save everything to [FOLDER PATH]
```

---

## Example Reports Built This Way

- 🇫🇷 **Gorges du Verdon + Côte d'Azur** — 93 activities with filters
- 🇩🇪 **Bavarian Alps** — 86 activities across Berchtesgaden, Garmisch & Salzburg
- 🇭🇷 **Croatia** — Multiple itineraries comparing resorts and destinations
- 🇮🇹 **Sicily + Mount Etna** — Volcano tours, beaches, and baroque towns
- 🇪🇬 **Egypt** — Red Sea resort + Pyramids with organised tours
- 🇦🇹 **Austria** — Zell am See + Lake Como connected by the Bernina Express
