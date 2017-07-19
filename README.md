# M-tools

A collection a useful tools for building queries in the Power Query Formula Language ("*M*") used by [Microsoft Power BI](https://powerbi.microsoft.com/).

[Language specification](https://msdn.microsoft.com/en-us/library/mt807488.aspx)

[Type system](https://msdn.microsoft.com/en-us/library/mt809131.aspx)

[Internal function references](https://msdn.microsoft.com/en-us/library/mt779182.aspx) (for usage with these tools)


## Usage

>Power BI does not (appear) to currently support external dependencies so setup is a little rudimentary.

1. Create a new blank query.
2. Copy the content of [m-tools.pqfl] to this query using the advanced editor.
3. Name the query `_`.

Functions may then be access from other queries as records on `_`. For example, `Pipe` may be invoked as `_[Pipe]({functionA, functionB, ...})`.