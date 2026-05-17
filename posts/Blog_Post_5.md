---
title: Week 11 - Locking in the Prototype
date: 2026-05-17
author: Noah Bloom
summary: This post reflects on the final stage of A1 development, where we focused on locking in scope, integrating work, polishing the prototype and checking whether the site still matched the original community goal.
tags:
  - integration
  - scope
  - final decisions
  - prototype
  - reflection
---

## Locking in the Prototype: Scope, Integration and Final Decisions

Beginning week eleven, the project shifted from exploring possibilities to locking in what we could realistically complete. Previously, we had talked about many options for the home cooking hub, such as browsing recipes, saving recipes, user profiles, asking questions, leaving comments, creating communities and maybe adding group chat. As the deadline approached, the main design decision became deciding what should stay central and what needed to be simplified or excluded.

The main constraint was scope. Including every social feature would make the home cooking community much larger and harder to finish properly. For instance, group chat and community groups would make the platform feel more social, but they would also add a lot of complexity. They would need more routes, database tables, interaction states and testing. Because of this, we decided to focus on the core recipe experience first. This meant prioritising the pages and features that helped users browse, view and interact with recipes.

![Scope decision board](assets/images/Decision_board.png)

*Figure 1: Scope decision board showing which features were prioritised, simplified or left for future development.*

The strongest part of our concept was not just that users could post content, but that home cooks could discover recipes and learn from other people’s changes, feedback and ideas. For that reason, recipe cards, recipe detail pages, tags and recipe interaction were treated as higher priority than broader social features. This was a compromise, but it helped keep the project aligned with the research insights from earlier weeks.

![Core user flow](assets/images/User_flow.png)

*Figure 2: Core user flow showing how a user moves from browsing recipes to viewing details and interacting with recipe content.*

We also had to make decisions about styling and presentation. At the start, our main concern was whether the site worked at all. By week eleven, the question became whether the prototype clearly communicated the intended community experience. The visual design needed to feel welcoming and suitable for a cooking community, but not so complex that it slowed down development. This meant using a cleaner card-based layout, readable text, clear buttons and simple navigation. The trade-off was that the current design would not include every visual detail from the wireframes, but it would be more achievable and easier to keep consistent for now.

![Prototype styling comparison](assets/images/Styling.png)

*Figure 3: Screenshots of the current prototype styling and layout progress.*

Another design decision was making the blog template visually match the style guide we were developing for the main project. Although the blog is separate from the A2 prototype, it still documents the same design process, so I wanted it to feel connected to the final community hub. This meant using a similar warm colour palette, rounded cards and orange accent colours. This was not essential for functionality, but it helped make the development blog feel more polished and consistent with the overall project identity.

![Blog and prototype style comparison](assets/images/Comparison.png)

*Figure 4: Side-by-side comparison of the blog styling and the main prototype style guide.*

From here, we developed the community hub significantly and created three solid working pages. The first was the landing page, which includes a featured recipes section. Eventually, these featured recipes could be based on user interaction, such as likes, comments or saves. This interaction still needs to be developed further, but the landing page already helps communicate what the platform is about and gives users a clear entry point into the recipe content.

The main page we focused on was the discovery/dashboard page. This was a significant challenge because we needed to move beyond placeholder content and connect recipes properly into the project structure. We had to work out how recipes should be stored, how they should be assigned to existing users, and how they should be displayed as readable recipe cards. This was important because the recipe cards are not just visual elements; they represent the connection between the database, the user system and the interface.

![Discovery dashboard and recipe card code](assets/images/Browse.png)

*Figure 5: Discovery/dashboard page showing recipe cards and the related code used to display recipe data.*

The third key page was the profile page. This page required us to think more carefully about how the prototype behaves for different users. Since the BlaBla Corp prototype assumes users are logged in, the profile page needed to recognise which user was active and display information relevant to them. For example, a user should be able to see recipes they have created and posted on their own profile. This helped connect the prototype back to the brief’s expectation that different users should have different experiences, even though we did not need to build a full login system ourselves.

![Profile page user-specific content](assets/images/Profile.png)

*Figure 6: Profile page showing how user-specific recipe content appears for the logged-in user.*

Overall, week eleven was about making the prototype coherent rather than adding as many features as possible. A larger feature set might have looked more impressive, but it also risked creating a broken or confusing prototype. By narrowing the focus, we were able to protect the core idea: a home cooking hub where users can browse, share and interact with recipe content in a way that still feels community-driven.