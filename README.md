# Valarray-cpp

### Valarray is a struct that enable lazy evaluation.

key words: 4 operators; using function objects to handle(+-*/); one binaryproxy
In my implementation, vec_wrap is inheriented from vector or proxy. I used function object(std::plus, std::minus...) to
deal with operator+-*/.  Also, I applied one binaryproxy to deal with all binary operations.
Finally, I use a new struct called Enable to process three different cases(V+V, S+V, V+S).
Therefore, there are overall 4 operators, rather than 12 operators.
