##Project Overview
For this project, students will answer 5 technical interview questions and get feedback from a qualified reviewer.

##Why This Project?
Having the knowledge to get through technical interviews is certainly helpful, but it won’t mean very much if you can’t clearly demonstrate this knowledge. This project will be assessed for correctness, but also criteria a real interviewer would look for, like clear and clean code, an understanding of efficiency, good communication, et cetera.

##What Will I Learn?
You will learn where your interviewing weaknesses lie. Graders have been instructed to be tough, so you cannot pass unless your answers are good enough that a real interviewer would be impressed.

##How Do I Complete this Project?
* Make sure you have some prior knowledge of technical interviewing or have gone through the Technical Interviewing course.
* For each question, create a solution in Swift. All solutions should be functions named as “question1”, “question2”, et cetera. Feel free to make additional helper functions or classes as needed. Code solutions must be submitted as an **OSX Command Line Tool** project in Xcode.
* In your project, **include at least 3 test cases** for each solution. For each test case, write the function call with the input you want to test and print it to the console, like "print(question1())". On the next line, comment out the output you expect to see from that function call. At least 2 of these must be edge cases, testing inputs such as nil values, empty inputs, unusually large values, et cetera.
* Write up an explanation for each question in a single separate text file (called "explanations.txt"). Your paragraph should **not** be a detailed walkthrough of the code you provided, but instead provide your reasoning behind decisions made in the code. For example, why did you use that data structure? You must also explain the efficiency (time and space) of your solution.
* You may submit your project and text file as a single .zip or as a GitHub repo on the website.

##Questions

####Question 1
Given two strings `s` and `t`, determine whether some anagram of `t` is a substring of `s`. For example: if `s = "udacity"` and `t = "ad"`, then the function returns `true`. Your function definition should look like: `question1(s: String, t: String) -> Bool`.

####Question 2
Given a string `a`, find the longest palindromic substring contained in `a`. Your function definition should look like `question2(a: String) -> String`.

####Question 3
Given an undirected graph `g`, find the minimum spanning tree within `g`. A minimum spanning tree connects all vertices in a graph with the smallest possible total weight of edges. Your function should take in and return an adjacency list structured like this:

```swift
["A":[("B", 2)], "B":[("A", 2), ("C", 5)], "C":[("B", 5)]]
```

Vertices are represented as unique strings. The function definition should be `question3(g: [String : [(String, Int)]]) -> [String : [(String, Int)]]`

####Question 4
Find the least common ancestor between two nodes on a binary search tree. The least common ancestor is the farthest node from the root that is an ancestor of both nodes. For example, the root is a common ancestor of all nodes on the tree, but if both nodes are descendents of the root's left child, then that left child might be the lowest common ancestor. You can assume that both nodes are in the tree, and the tree itself adheres to all BST properties. The function definition should look like `question4(t: [[Int]], r: Int, n1: Int, n2: Int) -> Int`, where `t` is the tree represented as a matrix, where the index of the list is equal to the integer stored in that node and a `1` represents a child node, `r` is a non-negative integer representing the root, and `n1` and `n2` are non-negative integers representing the two nodes in no particular order. For example, one test case might be

```swift
question4([[0,1,0,0,0], [0,0,0,0,0], [0,0,0,0,0], [1,0,0,0,1], [0,0,0,0,0]], r: 3, n1: 1, n2: 4)
```

and the answer would be `3`.

####Question 5
 Find the element in a singly linked list that's m elements from the end. For example, if a linked list has 5 elements, the 3rd element from the end is the 3rd element. The function definition should look like `question5(ll: Node, m: Int) -> Int`, where `ll` is the first node of a linked list and `m` is the "mth number from the end". Use the `Node` class below as a representation of a node in the linked list. Return the value of the node at that position.

```swift
class Node {
    var data: Int?
    var next: Node?

    init(data: Int?) {
        self.data = data
    }
}
```

##Evaluation
Your project will be evaluated by a Udacity Code Reviewer according to the rubric. All criteria must "meet specifications" in order to pass.
