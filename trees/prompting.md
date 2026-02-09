# Teaching Prompting Skills

### Purpose

Today, we are practicing prompting and specification writing using binary trees.

The goal is to see how vague instructions lead to different results and how adding precise constraints changes what an AI produces. 

You will use an AI tool to generate tree diagrams. Keep your diagrams visible so that you can compare them with the person next to you. The goal is not to be correct but to notice differences when we add different constraints to our prompts.

### Initial Prompt

Run this prompt once individually:

```tsx
Generate a binary tree with 11 nodes.
```

Notice: This prompt does not specify:

- Type of tree
- Values of nodes
- Output format
- Height
- Root

Compare trees with a neighbor. 

- Are they identical?
- If not, where do they differ?

```tsx
Question: What decision did the AI make that you never specified?
```

### Components of a Strong Prompt

We just saw that the same prompt produced many different trees. That’s not because the AI is wrong. We were not specific enough with our prompt. It was missing the structure of what makes a strong prompt.

A good prompt has five key components:

| Component | Description |
| --- | --- |
| Instruction | What action should happen? |
| Context | Which domain are we in? |
| Constraints | What rules must be followed? |
| Input | What data will the AI use? |
| Output | How should results be presented? |

Instruction specifies what action should happen. It’s the verb of the prompt. 

```tsx
Weak
Binary tree with these numbers.

Strong 
Generate a binary tree diagram.
```

The reason the verb matters is that LLM responds differently depending on the task. So, depending on what verb we use, generate, explain, verify, compare, and transform, you are going to get different outputs.

Context specifies the domain. The same word could have different meaning in different domains. 

Constraints reduce ambiguity. So the constraints we could give to a tree are:

```tsx
must be a bst
must be perfect
height = 4
root = 50
```

The fewer constraints we give, the more freedom the system has. Adding constraints guides the model to a narrow solution space. One thing to keep in mind is that good prompting removes degrees of freedom, and that does not necessarily mean writing more words. 

Input is what data is being used and output is how do I want the results to be presented. We are going to rebuild our tree prompts using these five parts. Each round, we will add one component and watch how the outputs converge.

### Adding Input

Update your prompt:

```tsx
Generate a binary tree using these values:

3 9 14 18 27 30 42 53 60 65 71
```

Predict: Will everyone now get the same tree?

Run the prompt and compare again with your neighbors.

### Algorithm LLM Is Using to Insert Elements

Prompt LLM:

```tsx
What method are you using to inserts elements into a tree?
```

### Add Constraint Height

Run this new version and compare again. 

```tsx
Generate a binary tree using the following values:
3 9 14 18 27 30 42 53 60 65 71

The tree height must be 4.
```

Height reduces possibilities but does not define the structure. We still don’t know which node is the root, the ordering rules, the traversal logic, and so on. 

### Add Completeness Constraint

```tsx
Generate a complete binary tree using the following values:
3 9 14 18 27 30 42 53 60 65 71

The tree height must be 4.
```

Run this new version. Compare again. 

### Add Binary Search Tree Constraint

```tsx
Generate a complete binary search tree using the following values:
3 9 14 18 27 30 42 53 60 65 71
The tree height must be 4.
```

Compare trees. Are we close to having identical trees? Why?

Notice that adding a binary search tree still does not force uniqueness. A BST can be constructed in multiple ways unless insertion order or traversals are specified. 

```tsx
Question: What is the minimum information needed so that everyone builds the same tree?
```

### Deterministic Prompt

Run this final prompt and compare. Trees should match.

```tsx
Construct the binary tree defined by:

Preorder:
42 18 9 3 14 27 30 65 53 60 71

Inorder:
3 9 14 18 27 30 42 53 60 65 71

Return ASCII diagram only.

```

### Reflection Questions

1. What changed between our first prompt and this one? 
2. Which prompt left the fewest decisions to the AI?
3. What single constraint made the biggest difference in reducing ambiguity?