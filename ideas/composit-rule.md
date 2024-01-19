# Composit Rule

The ability to combine multiple rules to through a meta rule or composit rule
to have more interesing understanding about the context when detecing a leak.

```
[[rules]]
id="pwn-request"
description="PwnRequest"
rule_expr = "(AND (pwn-request-self-hosted pwn-request-workflow-script-change))"
```

The expression doesn't have to be lisp'y but some kind of nested tree with ANDs
and ORs would be nice.

The results for the other two rules would show up in the results block like normal
but so would the composit rule.

This could be useful if the other two rules didn't have alert tags but the
compsit rule did.

We would have to figure out what the body of the composit rule would look like.
Maybe empty with just the tags being dynamically generated and appending
`type:composit, rule:<rule that triggered it>, ...`
