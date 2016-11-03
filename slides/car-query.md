#  Query

```groovy
graph.traversal()
  .V(CarID).hasLabel('product')
  .in('ordered').hasLabel('person')
  .out('ordered').hasLabel('product')
  .hasNot('id',CarID)
```
