---
title: Week 9/10 Translating the Idea into the Prototype
date: 11-05-2026
author: Noah Bloom
summary: This post reflects on how we moved from wireframes and planning into the actual build, focusing on prototype structure, data decisions, debugging and version control.
tags:
  - build process
  - prototype
  - technical decisions
  - database
  - GitHub
---

## From Plans to Build: Translating the Idea into the Prototype

The project shifted from planning into building during weeks nine and ten. At this point, we had developed the idea through brainstorming, online ethnography, wireframes, DDD and schema planning. This stage showed that having a strong concept was not the same as knowing how to write the code for it. The main decision became working out how our home cooking hub could fit into the existing BlaBla Corp prototype without breaking the template or moving too far away from the required tech stack.

A decision we made early on was to slow down and understand the prototype structure before adding too many features. In the beginning, it was confusing because different files and folders controlled different parts of the project, including routes, templates, models, public assets and database files. We used an LLM to help explain what each part of the BlaBla prototype was responsible for and where our recipe-related code should sit. This was useful because it helped me understand the existing files and how to use them more carefully.

![Annotated prototype folder structure](assets/images/structure.png)

*Figure 1: Annotated prototype folder structure showing where routes, templates, models, assets and database files sit within the prototype.*

This changed how I approached the build. Instead of trying to add every feature at once, I started writing notes in a separate document about what I wanted each part of the site to do and where that logic might belong. This became a useful bridge between design and implementation. Rather than just saying “make a recipe page”, I could break it down into smaller parts: a recipe list, a recipe detail view, recipe tags, filtering, database queries and visual recipe cards. These notes also made it easier to communicate progress to my group member because I could explain what I had changed, what was working, and what still needed attention.

![Zoom call explaining build changes](assets/images/Zoom.png)

*Figure 2: Zoom call where I explained recent build changes, including how recipe features were being broken into smaller implementation tasks and communicated back to the group.*

The schema and DDD work from the previous week became important here. They helped us see that the recipe hub needed structured data rather than placeholder content. Recipes needed titles, descriptions, images, cooking time, servings and tags. Tags also needed to be handled carefully because one recipe could belong to multiple categories, such as “Italian”, “vegetarian” or “spicy”. To support this, we started separating the recipe data into CSV files rather than keeping everything hard-coded into the page. This supported the earlier design goal of making the browse page filterable and more useful for home cooks. The trade-off was that adding proper data relationships made the build more complex, but it also made the prototype feel more dynamic and closer to our original concept.

![CSV files for recipe data](assets/images/Seed_data.png)

*Figure 3: Screenshot collage of the five CSV files in VS Code, showing how recipe data was separated into structured files for recipes, users, tags, ingredients and relationships.*

Another major learning point was that small implementation errors could break the whole site. Issues such as spelling mistakes, incorrect file paths, or a recipe CSV file having one too many lines could stop the prototype from working properly. These errors were frustrating, but they also showed why it was important to build carefully and test often. One significant issue happened while building the main home page where the recipe cards sit. After creating the CSV files for dummy recipes, a small formatting error caused the page to break and display as a blank HTML document. It took time to trace the issue, even when the console gave clues about where the error came from.

![Debugging process notes](assets/images/Error_message.png)

*Figure 4: Error message collage and blank page screenshot showing how small file or formatting issues affected the prototype.*

GitHub also became a practical constraint during this stage. Because we were working as a group, version control was necessary, but it also introduced its own problems. I had to learn how to manage branches, avoid working over other people’s changes and recognise when a branch had become too messy or broken to keep using. In some cases, it was easier to abandon a broken branch and return to a cleaner version rather than keep trying to patch errors. This was a compromise, but it helped reduce confusion and protect the working prototype.

![GitHub branch planning](assets/images/Branches_png.png)

*Figure 5: GitHub branch planning showing how different branches were used, tested and sometimes abandoned when they became unstable.*

Overall, weeks nine and ten were about translating our design decisions into a buildable structure. The most important decision was not to keep adding features, but to understand how the existing prototype worked and build the recipe system step by step. This meant prioritising database-driven recipe browsing and structured tags over larger ideas like group chat or more advanced social features. Those features still fit the broader community vision, but they were less important than getting the core recipe experience working. This helped keep the prototype focused on the original goal: creating a home cooking hub that supports discovery, contribution and community interaction without becoming just another static recipe site.