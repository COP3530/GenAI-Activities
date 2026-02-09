## **Tree Concepts Learning and Verification**

## Placement in Course Workflow
Students are familiar with Binary Search Tree Insertion and Traversals.

## Learning Objectives
Practice Binary Search Tree (BST) concepts and analyze prompts.

## Goal
Develop critical thinking and responsible AI use through binary search trees.  The goal is to see how AI-generated explanations may miss some intricacies about concepts themselves so while it’s helpful to use AI to explain topics, there may be some missing elements. 

## Tasks

You will use an AI tool to explain a specific computer science concept about binary search trees. Then provided a deliberately flawed statement by your instructor, your task is to verify, correct, and justify your understanding by searching the web and using definitions and credible sources and coming up with examples to prove the flawed statement wrong.

The goal is to learn how to evaluate AI output carefully and thoughtfully.

---

### Step 1 - **Initial Prompt**

Run this prompt individually:

Explain the following computer science concept: Explain tree data structures in computer science, including their properties and use cases.

Read the AI’s explanation carefully.

Mentimeter: What claims did the AI make about the tree data structure? Did the AI specify any assumptions (balance, insertion order, tree type)?

---

### Step 2 - **Instructor Statement**

Your instructor will now provide a misleading or partially incorrect statement about the same concept.

Example statements:

* “Searching a tree structure runs in O(log n) time due to the logarithmic growth of tree height.”  
* “A full binary tree is always perfect.”  
* “Removing a node from a tree is a straightforward operation that does not significantly affect the overall structure.”

---

### Step 3 - **Student Task**

In the instructor’s statement:

1. Quote or paraphrase the problematic part  
2. Identify what is incorrect or misleading  
3. Explain why it is incorrect without using AI through:  
   * Definitions  
   * Examples or counterexamples  
     1. What is the simplest tree that would prove the statement to be false  
   * Evidence from course material or credible external sources  
4. Provide a corrected statement that accurately represents the concept

Share your reasoning with peers nearby and see if you identify the same issues.

Mentimeter: Under what conditions could this statement actually be true? Is this statement about all trees, or a specific kind of tree?

---

### Step 4 - **Reflection Questions**

*Submit to an in class participation assignment or as a mentimeter*

* Did the AI explanation help you catch the error, or did it reinforce it?  
* Which definition or property was most important in identifying the mistake?  
* How could the original AI prompt be improved to reduce ambiguity or oversimplification?

---

### Step 5 - **If Time Allows**

* Rewrite your original AI prompt to request a more precise and rigorous explanation  
* Compare AI explanations with classmates:  
  * What differed?  
  * Which prompt produced the clearest result?  
* Explore other misconceptions

---

## **\[FOR INSTRUCTOR\]**

## **Other Possible Misconceptions**

* In a properly structured binary tree, internal nodes are expected to have two children to preserve the hierarchical nature of the tree.  
* Binary trees naturally remain balanced as elements are added, since values are distributed across multiple levels.  
* Binary search trees are inherently more efficient than linear data structures due to their hierarchical organization.  
* Binary trees and binary search trees differ mainly in terminology rather than structure or behavior.  
* In-order traversal produces sorted output because it visits nodes in a logical left-to-right sequence.  
* Tree structures require unique values to avoid ambiguity during insertion and traversal.

---

## **Activity Example**

**Concept:**  
Explain tree data structures in computer science, including their properties and use cases.

**Misleading statement:**  
Searching a tree structure always runs in O(log n) time due to its hierarchical organization.

**Why this is incorrect:**  
A tree does not guarantee logarithmic performance. If the tree is unbalanced, its height becomes O(n). In such cases, operations like search, insertion, or deletion take linear time. For example, if we have a right skewed tree like 1-\> 2-\> 3 \-\> 4 \-\> 5, then searching for the value 5 requires visiting every node.

**Corrected explanation:**  
Time complexity in tree-based structures depends on height. Balanced trees have height O(log n), leading to efficient operations. Unbalanced trees may degrade to linear performance. Therefore, O(log n) time is not guaranteed unless balance is enforced.

