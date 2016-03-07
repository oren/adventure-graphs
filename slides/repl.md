## show all available commands

g.Emit(g.V())

## add quad

:a dan age 34 .
:a josh age 21 .
g.V().All()

let's say i have 2 quads: :a dan age 34 . and :a josh age 19 .  can you show me the query(s) in the repl that will return all people between 20-30?

arr = []; j=0;
for (i = 20; i <= 30; i++) { arr[j] = g.V().Has("age", i.toString()); j++; }
output = arr.filter( function(iterator) {return iterator.All() !== null} )









for (i = 0; i <= arr.length - 1; i++) { console.log(arr[i].All()) }
x = g.V("Has", "21")
x.In("age").All()
