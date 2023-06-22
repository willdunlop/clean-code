# Meaningful Names

In programming, we name every thing. Variables, functions, directories etc. Since we do so much of it, we should aim to do it well. Make sure each name tells you all about the thing you have named

## Use Intention-Revealing Names

- Names should reveal intent
- It takes time to come up with a good name, but doing so will save time down the track
- Feel free to change names later if you come up with a better one
- A name should explain:
    - Why it exists
    - What it does
    - How it is used
- Something like `const d = 3 // elapsed time in days` should instead just be `const elapsedTimeInDays = 3`
    - Or `const daysSinceCreation = 3`
    - Or `const daysSinceModification = 3`
    - Or `const fileAgeInDays = 3`
    - Whatever is most appropriate for its context
- Even simple code can become a nightmare to interpret if poor naming has been used throughout

## Avoid Disinformation

- Its important to avoid leaving false clues when naming variables
- Do not name something `accountList` unless it is actually a list
- "List" will very much imply an array is in use. If there isn't, then it is misleading
- Even then, it's not great to encode a type into your variable names, types provide us with that information already
- In this case the simple name of `accounts` tells us we are dealing with more than one account, and that should be enough

- It is also good to be cautious of names that vary in small ways
- You don't want to have to try and distinguish between something like `XYZControllerForEfficientHandlingOfStrings` and `XYZControllerForEfficientStoringOfStrings`
- On close inspection we can see one handles and the other manages storing, but that is also very easy to miss

- Spelling similar concepts similarly is *information*
- Using inconsistent spellings is *disinformation*
- IDEs these days grace us with autocomplete
- It becomes helpful if the name for similar things appear in that list

- Even something like naming a variable `l` or `O` is disinformation.
- A quick first glance can make it difficult to tell if that may be `1` or `0`

## Make Meaningful Distinctions

- Do not name your variables to please the compiler
- You may come accross moments when two seperate variables could more or less use the same name
- They are different vairables, but 1 name is valid for each of them
- Obviously you cant have 2 seperate variables with 1 name, so it may be tempting to name it the same thing but with a variation in spelling
- Doing something like this creates a situation where correcting a spelling mistake leads to compilation errors
- If a compiler requires a different name, then the two variables should mean something different
- Figure out that difference and name it accordingly

- Number-series naming (`a1`, `a2`, `a3`) is not disinformation, it's non-information
- All it tells us is that this part of the code is confusing to read
- This is similar to using "noise" words
- It is very difficult to ascertain the difference between the three classes (`Product`, `ProductInfo`, `ProductData`)
- These are different names, but they dont mean anything different
- `Info` and `Data` could more or less be interchangeable with one another
- `variable` should never appear in a variable declaration
- Nor should a table ever have the word `Table` in it
- We already know a var is a var and a table is a table
- Good naming makes sure that we have chosen words that distinguish what the differences are

## Use Pronounceable Names

- If you can not pronounce your class name, how are you going to be expected to discuss it
- For example what does the function `genymdhms` do?
- It generates a date with year, month, day, hour, minute and second. You wouldn't know that until you read the actual code though
- Nor can you even refer to it in conversation. Not without sounding unprofessional

Compare the two, which class would be easier to have a conversation about?

```
class DtaRcrd102 {
    private Date genymdhms;
    private Date modymghms;
    private final String pszqint = "102";
}

/** OR */

class Customer {
    private Date generationTimestamp;
    private Date modificationTimestamp;
    private final String recordID = "102";
}
```

## Use Searchable Names

- It can be very hard searching for a single letter variable name
- Every use of that character in your codebase will return if you run a global search on it
- Single letter var names should only be used (if at all) as local variables inside short methods
- The length of a name should correspond to the size of its scope
- Something like `customers.map((c) => c.id)` at the very least infers what the single letter means (a single customer)


## Prefixes

- In Javascript, private variables are often prefixed with an `_`
- `function getAccounts` is public, but `function _init` would be private
- In Typescript, we have the ability to prepend the functions access properly
- There is no need for the prefix if the code reads as `private function init`
- It makes sense when the language does not supply a way to differentiate
- But it will just add unnecessary confusion if it does































