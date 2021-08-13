# Mutation Testing Manifesto

Most prominent bottlenecks when creating software are:

1. Accidental complexity
1. Source code bloat

**Accidental complexity** can be minimized/removed by practicing **Test Driven Development (TDD)**.

**Source code bloat** can be effectively removed by practicing **Mutation Testing**.

## Removing/Preventing source code bloat

When creating software we start from certain expectations. Since there are many ways to skin a cat, satisfying those expectations can take numerous shapes. Software engineering is a discipline that demands that the shape of the solution be as simple as possible.

Source code is text. It tends to be verbose. Verbosity leads to bloat. Bloat is extremely undesirable. Elegant software solutions offer a high level of readability. Quality source code is succinct and devoid of any redundancies. It states what is necessary and follows the principle of Occam’s Razor.

Many software creators strive to achieve the desired levels of simplicity, but find that the challenge is far from easy. A useful tool to assist the process of simplifying the source code is the Mutation Testing discipline (MT).

## How does Mutation Testing eliminate source code bloat?

Businesses need to automate the processing of their policy rules. In the majority of cases the only way to achieve that automation is by creating the source code. The expectations are formally declared in tests and the shipping code is then implemented in the source code.

When all tests are satisfied by the shipping code, it is not clear yet whether the resulting shipping code is bloated or not. The quickest way to gauge potential bloat is to execute mutation testing.

When mutation testing runs, it will locate areas of the source code that are not expected to be there. The immediate conclusion is that identified areas of the redundant source code need to be deleted.

If, upon examining the findings discovered by the mutation testing the team agrees to remove identified areas of redundant code, the bloat has been at least partially eliminated.

If the team disagrees with some or all findings, the seemingly redundant code must be covered by correct assertions. That means new tests must be added.

To fully eliminate any bloat (after removing or remediating the redundant areas of the source code), teams would have to experiment by removing some tests, then running mutation testing to see if there are any surviving mutants. It is important to keep eliminating tests until teams start noticing surviving mutants.

If after removing as many tests as possible there are no new surviving mutants, the bloat has been fully eliminated.

Only mutation testing gives us the tooling to know how to minimize the bloat in tests. It is extremely desirable to have as few tests as possible.

_Alex Bunardzic, August 2021_
