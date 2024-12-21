# MongoDB Case Sensitivity in Regular Expressions
This example demonstrates a common issue encountered when using regular expressions within MongoDB queries.  Specifically, it shows how the default case-sensitive behavior of JavaScript regular expressions can lead to unexpected results.

The original query uses `/John/` which will only match the exact string "John", not strings like "john" or "JOHN".  The solution provided demonstrates how to use the `$regex` operator and `$options` to make the match case-insensitive.

This repository provides both the problematic code and a corrected version.