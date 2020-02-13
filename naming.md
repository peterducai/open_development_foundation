1. Consistency
Each concept should be represented by a single, unique name.

Consistency is listed first, as it is the simplest and most impactful principle. Even though it may seem easy to obey, it is still very frequently violated. When it is violated, the downstream costs are greater than those of a violation of any other principle, since having multiple names for a single concept can cause those names to have violations of other principles, like understandability and searchability.

2. Understandability
A name should describe the concept it represents.

Ideally, a name will clearly communicate the concept that it describes to the broadest audience possible. If the reader has experience with the domain, they should not need to spend mental effort interpreting the intent of the name. If the reader does not have adequate experience with the domain to be familiar with the concept, then the name should be informative: after the reader has learned the name and its meaning, they should have a better understanding of the domain’s vocabulary and concepts.

3. Specificity
A name shouldn’t be overly vague or overly specific.

There are many ways in which a name can be either too specific or too general, both of which can lead to confusion Specificity can be a nebulous subject, so the most practical way of determining the correct specificity is to avoid common pitfalls, which can be grouped into underspecificity and overspecificity. We’ll explore these in detail in the book.

4. Brevity
A name should be neither overly short nor overly long.

Similar to specificity, this principle has contextual nuance to it, and we can most effectively describe what the appropriate length of a name should be by exploring common anti-patterns. The book explores these and groups them down into violations in which a name is either overly short or overly long.

5. Searchability
A name should be easily found across code, documentation, and other resources.

The searchability of a name provides many benefits: it supports searching the rest of the codebase to understand the implications of modifications, it eases rename refactors, and lets an engineer efficiently learn more about that concept in documentation. There are multiple factors that can contribute to poor searchability, such as a name being too short or too generic. Perfect searchability isn’t always achieveable, especially in large organizations, as a name like “user” may be the most appropriate for a given concept, while being generic enough that there are other valid uses of that name in adjacent domains.

6. Pronounceability
A name should be easy to use in common speech.

Pronounceability makes a name easy to use in everyday communication. Its pronunciation and spelling should be relatively unsurprising and relatively unique. If these attributes are surprising, then it will often be mispronounced, leading to multiple pronunciations and confusion. If its pronunciation and spelling are unique, then it’s also less likely to be confused with other concepts and other names. Homophones are especially troublesome, and these are explored in more detail in the book.

7. Austerity
A name should not be clever or rely on temporary concepts.

It can be tempting to use a bit of humor or a cultural reference in code to lighten the mood a bit, but doing this can violate many principles. For example, a joke name can reduce understandability of the underlying concept and reduce the name’s consistency and searchability. Colloquialisms (which are only understandable to certain audiences) and puns can cause similar issues. They may seem fun initially, but after dealing with them for years, that fun will turn into apathy and (more likely!) antipathy. When in doubt, choose names that are literal and dry.