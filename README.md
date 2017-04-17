- [Peaches](/peaches.md)

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

