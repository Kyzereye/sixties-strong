# Fitness project: instructions for Claude

This folder holds Jeff's personal fitness and nutrition plan and his logs. Jeff is 59½, about 180 lb, with somewhat high cholesterol. His goal is to get leaner and more muscular. Read `README.md` for an overview.

## How Jeff wants things written

Write complete, readable sentences and well-explained detail, the way a coach writes for a client. Never use choppy fragments. When he asks for plans, workouts, or recipes, include practical detail (portions, form cues, the reasons behind the advice).

## Logging conventions

When Jeff reports what he did or ate, record it without asking him to format anything:

- **Workouts** → append to `logs/workouts.csv`, one row per exercise: `date,session,exercise,weight_lb,set1_reps,set2_reps,set3_reps,set4_reps,notes`. Session is A, B, or Express. Use ISO dates. Leave set4 empty unless he did a 4th set.
- **Rides, walks, pickleball, yoga** → append to `logs/activity.csv`.
- **Weight and waist** → append to `logs/weight.csv`.
- **Food** → create or update `logs/food/YYYY-MM-DD.md` from `logs/food/_template.md`. Estimate calories, protein, fiber, and saturated fat for each item. Use the recipe numbers in `plan/recipes.md` when he eats one of those recipes. After logging, tell him the running daily totals against his targets (about 2,100 calories, or 2,500 on big ride days; 150+ g protein; 30+ g fiber; under 15 g saturated fat).
- After logging a gym session, compare it to the previous session of the same type and tell him which lifts are ready to move up, following the double-progression rule in `plan/training.md`.

## Weekly review

When asked, summarize the week from the logs and add the review to the top of `logs/weekly-review.md`, using the format described in that file. Give one concrete adjustment for the coming week.

## Constraints to respect

- His knee tolerates riding and pickleball, but not frequent running or hikes over 6 miles. Don't program running.
- He burned out on daily yoga. Keep yoga at about 2 short sessions a week unless he asks for more.
- Beer and ice cream stay in the plan, portioned. He is cutting soda and, through that, fast food. Support this.
- Blood work goes in `plan/blood-work.md`. When it arrives, revisit the saturated fat, egg, fiber, and alcohol guidance in `plan/nutrition.md`.
- Gym schedule: every 3 days, alternating A/B, starting Fri 2026-10-02 (A). The mountain bike ride goes on the day before a gym day, and **only on weekdays**: no weekend mountain bike rides, because the trails and parking lots are crowded. The Lafayette loop road ride is fine on weekends. "Lafayette loop" covers a few road routes of different lengths, so log the miles each time (for example, "I did the Lafayette loop, 14 miles").
