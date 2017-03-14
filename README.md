# Peach trees

Reference: http://www.almanac.com/plant/peaches

## Planting

- Can grow in USDA Zones 5-8 but well suited for 6-7
- Full sun
- well-drained soil
- avoid low areas
- Plant in spring
- Pick one that's about a year old
- Standard: Space them 15-20 feet; dwarf: 10-12 feet
- watering?

## After planting

- Do not fertilize within 2 months of first fall frost

### First year

- After 6 weeks, fertilize trees with 1lb nitrogen fertilizer
- In summer of first year, cut vigorous shoots.  One month later, cut to 3 wide-angled branches

### Second year

- 3/4lb N fertilizer once in spring, again in early summer
- early summer: cut back branches and shoots

### Beyond

- "remove any shoots in the center of the tree"
- Prune annually in mid-later April
- "Pinch" the trees in summer
- Thin fruits to 6-8 inches apart after tree blooms
- pick the fruit when it's ripe

# Peas

# Tomatoes from seed

Reference: http://www.wikihow.com/Grow-Tomatoes-from-Seeds

## Terms

### Loom

- Heirloom - pure-bred
- Hybrid - cross of varieties

### Types

- Determinate - shorter production, smaller plants
- Indeterminate - longer production

### Shape

- globe
- beefsteak
- paste
- cherry

## Harvesting seeds

...

## Planting seeds


### inside

- Start 6-8 weeks before last fronst
- Sow 2-3 seeds 1/4 deep in moist soil
- Store containers in 70-80 degree weather until germination happens
- Mist seeds for first 7-10 days
- water less frequently when you see sprouts

### harden

- When the plants are at least 6" tall and there's no frost outdoors, start hardening them outside about a week before planting
- expose plants to sun hour or less per day, then more.  Bring them in at night

### plant

- Prepare the soil
- pH is best between 6 and 7
- dig hole, put in good food
- fertilize monthly
- water the base
- pluck suckers

## Steps

There are states which require you to do activities regularly (such as watering/misting/weeding/sucker-removing).

Then there are actions you do once.  Some of these actions change the state.

When you do the action can either be based on:

- time before or after some event
- weather
- what you see the plant doing

```
- name: wait
  next_step:
    time: 6-8 weeks before last frost
- name: plant seeds
  actions:
  - plant seeds
  - put seeds inside
- name: wait for sprouts
  actions:
  - mist daily
  next_step:
    time: 7-10 days
    visual: sprouts appear
- name: reduce watering
  actions:
  - water a bit
  next_step:
    visual: 6" tall
    weather: no more frost
    time: 6-8 weeks after start
- name: harden
  actions:
  - put outside for X hours every day
  next_step:
    time: 1 week
- name: plant plants
  actions:
  - plant them
- name: water
  actions:
  - water
- name: fertilize
  actions:
  fertilize
```


2. Wait for sprout.

    duration: 7-10 days
    activity:
        ongoing: mist

```
states:
- name: planting
- name: germination
  conditions:
  - X-Y days have passed
  - 
- name: shoot
- name: seedling
- name: harden
- name: flowering
- name: fruiting
```

