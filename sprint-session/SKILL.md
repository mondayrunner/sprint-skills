---
name: sprint-session
description: >
  Prepares a sprint in three steps: a Product Vision Canvas, then user stories, then a Messaging Canvas. Each step builds on the output of the previous one. Use when the user wants to start a new project, work out a product idea, prepare a sprint, or go from idea to backlog and message in one go. This skill orchestrates the skills sprint-product-vision-canvas, sprint-user-stories and sprint-messaging-canvas.
---

# Sprint Session

This skill is an orchestrator that prepares a sprint: it calls three other skills in a fixed order and passes the output of each step to the next. You ask questions, the user answers. You never fill in what you do not know.

Never start a step before the previous one is finished and confirmed by the user.

## Step 1: Product Vision Canvas

Load the skill `sprint-product-vision-canvas`. Work through the five swimlanes from the outside in: Target Group, Needs, Product, Business Goals, Vision. Ask focused questions, summarize, and ask for confirmation before you go on.

## Step 2: User Stories

Load the skill `sprint-user-stories`. Write user stories based on the canvas, grouped per swimlane or theme. Format: "As a [type of user], I want [action], so that [value]", with acceptance criteria in Given-When-Then style.

Default is at least 10 stories as short headlines for the backlog. Order them by value and work out only the top three to five in full, with acceptance criteria. Offer to put the backlog on a board.

## Step 3: Messaging Canvas

In a short sprint, skip this step and do it in a later sprint, when you need to explain the product to someone. Otherwise load the skill `sprint-messaging-canvas`. Use the Product Vision Canvas and the user stories as input. Work through the six steps: Struggle, Solution, Hesitations, Awareness, Differentiators, Success. Use Feature, Ability and Benefit for every proposition element.

## Closing

Present one summary of the three results. Ask the user what they want to do first: build the first story, test the message with a real person, or improve one of the canvases.

## Make it your own

The order and the questions are a starting point. Add a step (for example a pricing check or a copy review by another skill), remove one, or change the questions. That is how an orchestrator grows into your own way of working.
