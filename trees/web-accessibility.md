# Tree Traversals & Accessibility

## Learning Objectives
After completing this activity, students will be able to:
- Construct a Binary Search Tree (BST) from a sequence of insertions
- Differentiate between preorder, inorder, postorder, and level-order traversals
- Explain how traversal choice affects the clarity and completeness of structural descriptions
- Generate clear, concise alt text that accurately represents tree structure
- Relate accessibility principles in computing to real-world web content
- Critically evaluate LLM-generated descriptions for ambiguity and completeness

---

## Goal
Practice Binary Search Tree (BST) traversals, explore how prompt wording affects LLM output, and understand why clear alt-text matters for accessibility.

By the end of this activity, you will:
- Build a Binary Search Tree
- Use an LLM to generate a traversal-based description (alt text) of your tree
- Exchange descriptions with a partner
- Attempt to reconstruct each other’s trees from text alone

---

## What Is Alt Text?

**Alt text (alternative text)** is a short textual description of an image that conveys the **meaning and purpose** of the image.

Alt text is used by:
- Screen readers for users who are blind or have low vision
- Browsers when images fail to load
- Search engines to understand images

Good alt text balances:
- **Completeness** — all relevant structural information
- **Conciseness** — no unnecessary detail

Guiding question:
> *“If someone cannot see this image, what do they need to know?”*

---

## Step 1 — Build Your Tree (Work Individually)

1. Choose **7 distinct integers**.
2. On paper, insert them into an empty **Binary Search Tree** in the order you choose.
3. Write down or sketch the final tree structure.

---

## Step 2 — Choose Traversals (With a Partner)

Each partner must choose **one** traversal, and **you must pick different traversals**.

Available traversals:
- Preorder
- Inorder
- Postorder
- Level-order

---

## Step 3 — Prompt an LLM to Generate Alt Text

1. Go to the NavigatorAI Chatbot:  
   https://it.ufl.edu/ai/navigator-chat/
2. Select any model.
3. Use a prompt similar to:

```
I have a Binary Search Tree built from these values inserted in the following order:
[list your numbers in insertion order].

Generate alt-text that describes the tree using [chosen traversal].
```

Refine your prompt if the output is unclear or ambiguous.

---

## Step 4 — Partner Exchange & Reconstruction

1. Do **not** show your tree.
2. Read your alt text aloud to your partner.
3. Your partner reconstructs the tree from the description.
4. Compare results and discuss accuracy.
5. Switch roles.

---

## Step 5 — Reflection

Discuss:
- Was the description easy to follow?
- What information was missing or ambiguous?
- How did traversal choice affect clarity?
- How does this relate to web accessibility?

---

## Step 6 — Bonus

Write a program that automatically generates alt text for a Binary Search Tree using a specified traversal.


## Survey Questions on Canvas for Students (Optional)

- Who was your partner?
- Which model did you select on Navigator? If you used an external tool - e.g., ChatGPT, Gemini - state the tool and why did you chose it over Navigator?
- State the prompt that you used when interacting with your chatbot to construct alt-text descriptions.
- I found this activity engaging. <Strongly agree - Strongly disagree>
- After this activity, how would you describe your understanding of digital accessibility (e.g., alt text and why it matters)? <I had little or no understanding of alt-text before and still feel unsure, I had little or no understanding of alt-text before and now have a basic understanding, I had some understanding of alt-text before and now I understand it even better, I already knew how alt-text work before this activity and did not gain anything new>
- Reflect on your interaction with the chatbot and what you learned about accessibility.
