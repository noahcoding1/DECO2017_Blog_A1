---
title: A3 Reflection - Evaluating the Home Cooks Community Hub
date: 2026-06-04
author: Noah Bloom
summary: This final reflection evaluates the performance, usability, accessibility and functional requirements of our Home Cooks community hub prototype.
tags:
- A3 reflection
- Evaluation
- Performance
- Accessibility
- Functional requirements
---

## A3 Reflection: Evaluating the Home Cooks Community Hub

Looking back at the final prototype, I think our Home Cooks community hub was successful because we were able to turn a broad idea into a working site with a clear user flow. At the start, we had a lot of possible ideas, including featured recipes, a Pinterest-style recipe dashboard, recipe posting, likes and comments, individual profile pages, question spaces, communities, recipe scaling and even ordering missing ingredients through Coles or Woolworths. By the end, the prototype became more focused around the main recipe experience of being able to browse recipes, viewing recipe detail pages, creating recipes, uploading images with alt text, liking recipes, using the profile page, and showing how community features could work.

The final site is not every single thing we brainstormed, but I think that became one of the main lessons of the project. A working prototype needs to prioritise the most important functional requirements first, instead of trying to add every interesting idea.

### Performance

Our prototype was very successful in the Lighthouse audits, especially in the accessibility section where we were scoring 100%. After that, we still needed to do manual checks because Lighthouse can only test some accessibility problems automatically. From our own checks, the main pages were responsive across different screen sizes, the navigation worked clearly, and the load times felt fine during normal use.

![Lighthouse audit showing performance and accessibility results](assets/images/lighthouse_audit.png)

*Figure 1: Lighthouse audit showing the prototype’s performance and accessibility results.*

One issue Lighthouse did mention was reducing image file sizes. This made sense because recipe images became a major part of the site. They helped make the interface feel more polished and suitable for a cooking community, but they also created a performance issue as larger images made the recipe cards and detail pages look better, but they also meant the browser had to load more data than necessary. If we had more time, I would compress the images properly and use smaller versions for recipe cards, while keeping larger images for the recipe detail pages.

A key strength of the site was the polished UI and navigation. I think our site followed a good user flow because it was easy to move from the landing page, to browsing recipes, to opening a recipe detail page, and then back to other sections like the profile or communities page. The layout also made the purpose of the site clear quite quickly. Users could understand that the site was about home cooking, recipe discovery and community contribution without needing much explanation.

### User Experience

The interface was usable and most of the interactions felt clear to me. The recipe cards made the discovery page easy to scan, and the recipe detail pages gave users more information when they wanted to go deeper. Adding creator names, tags and likes also helped the site feel more like a community hub rather than just a static recipe database. This was important because one of our main goals was to make the platform feel like a place where home cooks share and interact, not just a place where recipes are stored.

![Recipe browsing and recipe detail pages](assets/images/Recipe_flow.png)

*Figure 2: Recipe browsing and recipe detail pages showing the core flow from discovering recipes to viewing full recipe information with updates styling.*

I think we met most of the goals we set out to reach, but there were still some things we did not fully get to complete. One of the main features we wanted was saving recipes. The idea was that users could save recipes from the recipe page or browse page, and then view those saved recipes on their profile. We also wanted the profile page to feel more like a personal page, almost like a Tumblr-style page, where users could see recipes they had posted, saved, liked or commented on. We got most of the profile function working, especially around created recipes, but we did not get to that final saved/liked/commented profile system.

![Create recipe overlay and profile page](assets/images/Recipe_flow.png)

*Figure 3: Create recipe overlay and profile page showing how user-created recipes connect back to the logged-in user.*

Another idea that we had that we did not complete was ordering missing ingredients. The concept was that users could open a recipe, see the ingredients, and then order the items they did not have through a Coles or Woolworths link or integration. This could have been useful for home cooks because it connects recipe discovery to actually cooking the meal. However, it was not realistic for our prototype because it would require external links, possible API integration, and a much more detailed ingredient system. Cutting this feature was the right decision because it was outside the main scope and not essential to proving the community hub idea.

The communities section was also an interesting scope decision. Originally, communities were something we thought might be outside the scope of our design. However, once the rest of the site was progressing, we decided to add it in because it fit the broader idea of a community hub. I am happy with how it looks, but if we had more time I would make it fully functional. Similar to the create recipe section, I would want users to be able to create their own communities, join existing ones and see community-specific recipes or discussions.

![Community page and placeholder states](assets/images/Communities_flow.png)

*Figure 4: Community page and placeholder states showing how future social features were represented without overbuilding them.*

We also intentionally only made one community page properly. This was a design decision rather than just something unfinished. We felt that having one working community example was better than making four or five dummy pages that did not add much. Since the prototype is not going public, one developed example was enough to show tutors the direction we were going for and how the feature could work in a more complete version.

The same applies to comments and adaptations. Right now, the comments and adaptations are not fully recipe-specific, so each recipe can show similar content. In a final public version, this would need to change. Each recipe should have its own comments and adaptations linked to the recipe ID. However, for this prototype, we felt it was enough to communicate the intended interaction pattern and show how home cooks could discuss changes, substitutions or improvements under a recipe.

### Functional Requirements

When I compare the final prototype to our original functional requirements, I think we achieved the main core of the site, but not every possible feature from the brainstorm.

| Functional requirement     | Final outcome   | Reflection                                                                      |
| -------------------------- | --------------- | ------------------------------------------------------------------------------- |
| Browse recipes             | Achieved        | This became the main discovery experience.                                      |
| Filter recipes             | Achieved        | Useful for cuisines, dietary needs and recipe discovery.                        |
| View recipe details        | Achieved        | Important because users need full recipe information.                           |
| Create recipes             | Achieved        | Users can create recipes that save to the users profile                         |
| Upload images and alt text | Achieved        | Helped both visual design and accessibility.                                    |
| User profile page          | Mostly achieved | Shows user-created recipes, but saved/liked recipes could be expanded.          |
| Likes                      | Achieved        | Worked, but required lots of debugging between cards and detail pages.          |
| Comments and adaptations   | Partly achieved | Present as a concept, but not fully recipe-specific yet.                        |
| Communities                | Rescoped        | One working example shows the idea without overbuilding.                        |
| Recipe scaling             | Achieved        | Users can changes each recipes ingredients to their desired serving size easily |
| Ingredient ordering        | Cut             | Would require external integration and was outside the realistic scope.         |

This reassessment showed that our original goal was strong, but the full scope was too large. We reached the main goals of creating a home cooking hub with recipe discovery, recipe creation, user profiles and community direction. However, on the wider scope of every idea we had, we did not get to everything. AS we underestimated how tough getting these main ideas working actully was. This was not necessarily a failure. It showed that scoping is a major part of web development, and that features need to be prioritised based on what the prototype actually needs to prove.

### Development Process and Lessons Learned

Throughout the development process, I learned a lot, especially about working with GitHub in a group. I had not really done coding work in a group before, so using branches and merging changes was difficult at the start. We would often work on separate tasks, but then merging them back into main created conflicts or unexpected issues. We found it much easier to discuss conflicts in person or over Zoom before merging, because otherwise it was easy to accidentally break something that was working on someone else’s computer.

![GitHub and debugging evidence](assets/images/Git_errors.png)

*Figure 5: Example of GitHub, debugging or error evidence from the development process.*

The biggest issue overall was code errors. We ran into a lot of errors throughout the development of the community hub, and they were often random or hard to understand at first. Sometimes an issue would appear on one person’s computer but not on the other person’s. For example, there were times where the system gave errors about not being able to find files in the `lib` section, but this was only broken on my computer and not my group member’s. There were also times where CSS worked on my computer but not on hers. To fix these kinds of problems, we had to try things like clearing caches, reinstalling files, checking dependencies and switching branches.

I had to uninstall and remove GitHub from my computer twice, and my group member had to do similar things like clearing the cache and reinstalling files to get each other’s code working. This was frustrating, but it also became one of the biggest technical learning points. A lot of web development is not just writing new code, but understanding why something that should work is not working in a specific environment.

There were also smaller bugs caused by missing letters, missing commas, brackets, file path issues or small syntax mistakes. These were annoying because they could break a whole page even though the actual mistake was tiny. Over time, I got better at reading error messages and using them as clues. At the start, an error message felt like the whole site had failed. By the end, I was more comfortable tracing the issue through the model, controller, template, CSV file or route to find where the problem was actually coming from.

Another important lesson was that design decisions and technical decisions are connected. For example, choosing to have recipe tags was not only a visual design choice. It meant we needed to think about how tags were stored, how recipes connected to tags, how filtering worked, and how the interface showed the selected filter. Similarly, choosing to include created recipes meant thinking about the logged-in user, the database, image uploads, alt text, the form structure and the profile page. This helped me understand that functional requirements are not just a feature list. They shape how the whole site has to be built.

If I continued developing the prototype, I would focus on a few improvements. First, I would optimise image file sizes so the site stays fast as the community expands and more recipes are added. Second, I would make comments and adaptations fully recipe-specific. Third, I would finish the saved recipes feature so users can save recipes and see them on their profile. Fourth, I would make communities fully functional so users can create and join polished and working communities. Finally, I would do more manual usability and accessibility testing, especially around navigation, mobile layout and whether first-time users properly understand what to click.

Overall, I think the prototype was successful because it became a focused version of the home cooks community hub rather than trying to include every feature from the brainstorm. The strongest part of the final site is the core journey: discovering recipes, viewing them, creating them and beginning to interact with them as community content. The project taught me that a successful prototype is not about adding the most features, but about making sure the features that are included actually support the chosen community and work together properly.
