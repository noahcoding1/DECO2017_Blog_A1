---
title: Week 8/9 — From Concept to Wireframes
date: 2026-05-01
author: Noah Bloom
summary: This post is the journey on how wireframing helped us move from a broad home cooking concept into clearer pages, layouts and components for the prototype.
tags:
  - Wireframes
  - Design development
  - Home cooks
  - Prototype planning
  - User flows
---

## From Concept to Wireframes: Bringing the Home Cooking Hub to Life

After choosing home cooks as our community and identifying the risk of becoming a generic recipe-sharing site, the next step was to start turning the idea into something more concrete. This post focuses on wireframing, which helped us move from broad feature ideas into actual pages, layouts and user flows. At this stage, the wireframes are not intended to be final designs. Instead, they are a way to test the structure of the site and work out what components would be needed in the prototype.

The main design decision was deciding what the home cooking hub should centre around. From our early research, recipe sharing alone did not feel strong enough because many existing platforms already allow users to find and save recipes. Instead, we wanted the site to support the more social parts of home cooking: adapting recipes, asking questions, giving feedback and learning from other people’s changes. This shifted the concept from a simple recipe library towards a community hub where recipes could be discussed and improved over time.

![Concept sketches showing the design shift](assets/images/Sketches.png)

*Figure 1: Early concept sketches showing the shift from simple recipe sharing to a stronger focus on adaptation, discussion and feedback.*

Wireframing helped us break the project into key views. The first view we considered was the main recipe browsing page. This page needed to show enough recipe content to feel active, but not so much that it became overwhelming. We discussed using recipe cards with images, recipe titles, cuisine tags, difficulty levels and dietary labels. This would allow users to quickly scan recipes and decide what to open. The trade-off here was between visual appeal and simplicity. A Pinterest-style layout could be engaging, but it could also become cluttered or difficult to implement, so a more structured card layout seemed more realistic for the prototype.

![Full wireframes created in Figma](assets/images/Wireframes.png)

*Figure 2: Our Figma wireframes showing the main pages, including the home page, browse recipes page, recipe detail page, create recipe page and profile page.*

After creating our initial wireframes, we used class time to annotate and refine them. This helped us move from visual layout into a more technical way of thinking. The process followed a rough flow:

1. Wireframes  
2. DDD  
3. ERD  
4. Schema  

This was useful because it showed that the pages were not just screens, but collections of dynamic components. For example, a recipe card would need a recipe title, tags, preparation time, serving size, likes and creator information. The recipe detail page would need more information, including ingredients, steps, comments, adaptations and possibly serving size controls.

![Annotated wireframe breakdowns](assets/images/Breakdown.png)

*Figure 3: Annotated wireframes and breakdowns from class, showing how we began identifying components, data and possible interactions.*

One of the more difficult parts was thinking through the recipe system. We wanted users to be able to input recipes in a structured format so that recipe information could appear on the home page, browse page and profile page. We also discussed a recipe scaling feature, where users could change serving sizes and have ingredient quantities adjust. This was interesting because it directly supported home cooks, but it also created extra complexity. For the prototype, we need to decide whether this is a core feature or something that should be simplified.

We also began listing possible tags for filtering recipes. These included cuisine tags such as Italian, Indian, Mexican, Mediterranean, Thai and Japanese; dietary tags such as vegan, vegetarian, dairy-free and gluten-free; and spice-level tags such as non-spicy, mild, medium and spicy. These tags made the browsing experience more useful, but also showed why the database would need to be carefully structured.

![DDD recipe system breakdown](assets/images/DDD.png)

*Figure 4: Early DDD breakdown showing the information needed for recipe cards and recipe detail pages.*

To move from our DDD into a clearer data model, we used ChatGPT and dbdiagram.io to help map out an ERD/schema. This helped us understand how different parts of the system could connect, such as users, recipes, tags, ingredients, comments and saved recipes. It also helped us see why some parts, like recipe tags, may need a join table rather than being stored as plain text. This was important because it made the prototype feel more buildable and gave us a clearer starting point before moving into VS Code to do this.

![ERD and schema planning](assets/images/Schema.png)

*Figure 5: ERD/schema planning created from our DDD work, showing how recipe-related data could connect in the prototype.*

Overall, this week helped us move from concept to structure. The wireframes made the idea more concrete, while the DDD and schema planning showed what information the prototype would need to store and display. The biggest trade-off was balancing interesting features, like recipe scaling and ingredient ordering, against what we could realistically build. Going forward, the priority is to keep the prototype focused on the core community experience: browsing, creating and discussing recipes in a way that supports home cooks rather than becoming just another recipe platform.