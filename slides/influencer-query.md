#  Query

```groovy
graph.traversal()
  .V(TwitterHandle).hasLabel('person')
  .both('follows').hasLabel('person')
  .as('firstdegree')
  .order().by(select('firstdegree').count())
  .out('follows').hasLabel('person')
  .hasNot('id',TwitterHandle)
```
