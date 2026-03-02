This repository contains an interactive HTML guide designed for senior Android developers inspired by articles in the repo: https://github.com/skydoves/compose-performance thanks to @skydoves for study collection.

It provides a deep dive into how the Compose compiler evaluates types and offers practical, "Good vs. Bad" code comparisons to solve real-world performance bottlenecks.

Key Features Included:

The 5 Stability Types: Detailed breakdowns of Certain, Runtime, Unknown, and Parameter stability categories.

Performance "Bug" Catalog: Visual guides to the most common stability killers, including accidental var fields in data classes and the "Unknown" stability of standard List interfaces.

Annotation Mastery: Proper usage of @Stable and @Immutable to hint to the compiler when it is safe to skip recomposition.

Stability Configuration: Instructions for implementing stability_config.conf to treat external or standard library types as stable.

Interactive Decision Flow: A logic-based walkthrough of how Compose determines if a type is skippable at runtime.

8-Step Runtime Checklist: A concise checklist for auditing and fixing recomposition issues using the Layout Inspector.

