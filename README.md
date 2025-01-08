# Uncommon HTML Bug: Unexpected innerHTML behavior
This repository demonstrates an uncommon bug related to the use of innerHTML in JavaScript within an HTML document.  The issue arises from attempting to prepend content using innerHTML in a way that isn't intuitive. The initial code incorrectly appends content to the start rather than the end, even though it's written with the intention to prepend.

## Bug Description
The primary problem lies in the order of operations within the innerHTML assignment.  The existing innerHTML is concatenated *after* the new content, leading to the new content being appended at the end, instead of the beginning as intended.

## Solution
The solution involves using methods designed for insertion. Using insertAdjacentHTML provides a more reliable and predictable way to add content to specific locations within the HTML structure.