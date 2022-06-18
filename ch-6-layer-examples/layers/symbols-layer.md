# Symbols Layer

Symbol layer was for commonly used programming symbols shown in the table below. I have decided to deprecated that layer and instead use [tap-dance / super keys](../../ch-3-layer-activators/3.6-tap-dance-super-keys.md) because I think it is a superior alternative.&#x20;

Super keys allow for 3 keys to be combined into single key. This mean that instead of splitting symbols between the default, shift and symbols layer instead they can all fit into 1 or 2 layers. For this reason I placed this table in the symbols layer to organize symbols super key usage and because they can exist in either the default or shift layer depending on the users preferences.

In VS code and I suspect other editors, when an opening bracket or parentheses is used, then a matching closing symbol is automatically placed behind the cursor. So you are editing content within the bracket and never have to type out the closing symbol. This means the frequency of opening brackets is much higher than closing and by combining them into a super key, 2 adjacent keys can be combined into 1. Sometimes you want to call a function or create an empty object, in which case hold will output a macro that has both the opening and closing brackets or parentheses.

| tap | tap-tap | hold                     |
| --- | ------- | ------------------------ |
| (   | )       | ()                       |
| \[  | ]       | \[]                      |
| {   | }       | {}                       |
| =   | ==      | :=                       |
| <   | <=      | <- (< less than, - dash) |
| >   | >=      | ->                       |
| +   | ++      | +=                       |
| -   | --      | -=                       |
| \*  | &       | $                        |
| ?   | ^       | %                        |
| /   | \\      | \|                       |
| :   | ::      | ;                        |
| \_  | \`      | \~                       |
| !   | !=      | @                        |

