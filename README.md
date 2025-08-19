# week_6_coding-problem

perfect square question

Imagine you have a number, let's say 12. The task is to find the smallest number of perfect squares (like 1, 4, 9, 16...) that add up to that number.

For example, for 12:

You could use 1 + 1 + 1 + ... (twelve times), but that's not the smallest number of squares.
A better way is 4 + 4 + 4 (three times). So, the answer is 3.
This code figures out that smallest number of squares for any given number.

nim game 

The approach is very simple, if the total number of stones are not completly divisible by 4 then you can always with the game

Example: 4 stones

You can pick atmost 3 stones [1, 2, 3]
Your friend can pick 1 stone [4] and win the game
Example: 8 Stones

You can pick atmost 3 stones [1, 2, 3]
Your friend can pick 1 stone [4]
You can pick atmost 3 stones [5, 6, 7]
Your friend can pick 1 stone [8] and win the game
Example: 8 Stones

You can pick 1 stone [1]
Your friend can pick atmost 3 stones [2, 3, 4]
You can pick atmost 3 stones [5, 6, 7]
Your friend can pick 1 stone [8] and win the game


binary tree maximum path sum

Perform postorder DFS traversal.

At each node:

Recursively compute the max gain from the left and right children.
Ignore negative gains (treat them as 0).
Update the global max (ans) with the path going through this node: node.val + leftGain + rightGain.
Return to the parent: node.val + max(leftGain, rightGain) since parent can only continue on one side.
