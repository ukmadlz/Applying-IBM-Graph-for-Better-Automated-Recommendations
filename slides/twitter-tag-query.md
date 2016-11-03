#  Query

```groovy
graph.traversal()
  .V(TwitterHandle).hasLabel('person')
  .out('tweeted').hasLabel('hashtag')
  .in('tweeted').hasLabel('person')
  .hasNot('id',TwitterHandle)
```
