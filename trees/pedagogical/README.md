# Pedagogical Concept Activity

## Overview
In this activity, students are given a computer science concept (in this activity, trees) by their instructor. They use an AI tool like ChatGPT to explain the concept. Then, the instructor intentionally provides a misleading or partially incorrect statement, and students must identify, explain, and correct the errors by using the AI explanation and finding credible, external sources to back up its claims with evidence.

**The goal is to develop:**
- Critical thinking and error detection
- Responsible and informed use of AI tools
- Correct any common misunderstandings about topics that may arise

## Learning Objectives
By the end of this activity, students will be able to:
- Differentiate between tree structures
  - Binary Tree
  - Binary Search Tree (BST)
- Correctly define and apply structural properties
  - Full vs. complete vs. perfect binary trees
  - Tree height
  - Relationship between tree height and time complexity (e.g., O(log n) vs O(n))
- Develop AI literacy
- Practice verification against course knowledge and definitions

## Instructor Setup
Choose a concept that students think they understand but often confuse. The prompt should be deliberately flawed in a minor way and is designed to trigger misconceptions. Good examples include:

### Misconceptions:

**All nodes must have 2 children**
> "In a properly structured binary tree, internal nodes are expected to have two children to preserve the hierarchical nature of the tree."

**Trees are always balanced**
> "Binary trees naturally remain balanced as elements are added, since values are distributed across multiple levels"

**BSTs are more efficient than linear structures**
> "Binary search trees are inherently more efficient than linear data structures due to their hierarchical organization."

**A binary tree and a binary search tree are basically the same thing**
> "Binary trees and binary search trees differ mainly in terminology rather than structure or behavior."

**A full tree is always perfect**
> "A full binary tree satisfies the conditions of a perfect binary tree."

**Leaves are always at the same depth in a binary tree**
> "Leaves in a binary tree generally occur at the same depth because the tree expands downward in levels."

**Binary trees must be symmetrical**
> "Binary trees are typically symmetrical, with left and right subtrees mirroring each other."

**Searching a tree is always O(log n)**
> "Searching a tree structure runs in O(log n) time due to the logarithmic growth of tree height."

**In-order traversal of any tree produces sorted output.**
> "In-order traversal produces sorted output because it visits nodes in a logical left-to-right sequence."

**Trees must contain unique values.**
> "Tree structures require unique values to avoid ambiguity during insertion and traversal."

**Removing a node is simple—just delete it.**
> "Removing a node from a tree is a straightforward operation that does not significantly affect the overall structure."

## Student Instructions
1. You are given the following instructor-provided concept: [concept]
2. Prompt the AI to give you an explanation about said concept
3. Read the AI's explanation carefully
4. The instructor will provide a misleading statement about the concept
5. For each issue:
   - Quote or paraphrase the problematic statement
   - Identify the problematic part of the statement
   - Explain why it is incorrect definitions, examples, and evidence
   - Provide a corrected statement along with your explanation
6. Share with your peers around you if you came to the same conclusion 
7. Submit a short written response to the assignment

## Key Concepts Students Are Expected to Use

### Binary Tree Classifications

| Term | Definition |
|------|------------|
| Full | Every node has 0 or 2 children |
| Complete | All levels filled except possibly last, filled left to right |
| Perfect | All levels completely filled |
| BST | Not necessarily complete |

### Height and Time Complexity
- A tree has height O(log n) only if it is balanced
- A BST can degrade to height O(n)
- log n comes from branching, not from "being just a tree"

## Example

**Misleading statement:** Operations on a binary tree are always O(log n) due to the tree's level-based structure and branching.

**Why this is incorrect:**
A binary tree does not guarantee logarithmic performance. Only balanced trees (such as AVL trees or Red-Black trees) ensure O(log n) height. A binary tree (like a skewed tree) can degrade into a linear structure, causing operations like search, insert, or delete to take O(n) time.

**Corrected explanation:**
Time complexity in a binary tree depends on its height. Balanced trees have height O(log n), leading to O(log n) operations, while unbalanced trees could have height O(n), resulting in linear-time operations. Therefore, O(log n) performance is not guaranteed unless the tree maintains balance.

## Pedagogical Rationale
This activity targets a whole conceptual understanding of the topic instead of surface recall or overgeneralizations.

Students often overgeneralize properties (e.g., "trees = log n" or "ordered = sorted")

AI responses amplify this problem by:
- Sounding authoritative while providing oversimplified statements
- Blending correct terms with incorrect reasoning

To ensure that they have the correct understanding of the topic, students must:
- Apply definitions
- Defend their reasoning
- Come up with their own examples that disproves the given misleading statement

This aligns with constructivist learning and supports metacognition as students think about how and why they know something is correct.

## If Time Allows:
- Have students rewrite the AI prompt to get a more clear, extensive explanation about the concept 
- Compare AI responses between each other (students) to see how answers can differ based on the prompt provided
