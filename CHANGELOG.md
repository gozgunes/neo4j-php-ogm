1.0.0-RC2 (not released yet)



1.0.0-RC1 (2017-02-27)

- BaseRepository now implements Doctrine's `ObjectRepository` and `Selectable` ([#87](https://github.com/graphaware/neo4j-php-ogm/pull/87))
- Added `SKIP` and `LIMIT` to via the `findBy` Repository method ([#86](https://github.com/graphaware/neo4j-php-ogm/pull/86))
- BC : `EntityManager::buildWithHost()` has been removed ([#98](https://github.com/graphaware/neo4j-php-ogm/pull/98))

1.0.0-beta22

- Refactored Proxisation of Relationships ([#67](https://github.com/graphaware/neo4j-php-ogm/pull/67))
- BC: criteria arguments are passed as array (#67)
- BC: `@Lazy` relationship has been removed
- BC: Direct property access do not trigger lazy loading (`$this->actors` should become `$this->getActors()`
- Fix circular reference : ([#68](https://github.com/graphaware/neo4j-php-ogm/pull/68))
- Fix proxy generation for php7 return types ([#76](https://github.com/graphaware/neo4j-php-ogm/pull/76))
- Added the possibility to add order by via the findBy method ([#84](https://github.com/graphaware/neo4j-php-ogm/pull/84))

1.0.0-beta19

- ClassMetadata implements DoctrineCommon ClassMetadata
- `getClassMetada` in EntityManager now handle node and relationship entity classes
- `@Lazy` on a non-collection relationship doesn't have a lazy effect

1.0.0-beta17

- fixed a bug where fetched RE entities were not marked as managed
- fixed a bug where fetched lazy simple relationships were not marked as managed
- lazy loaded simple relationships have their non-lazy associations marked as lazy

1.0.0-bet13,14,15, 16

- multiple bug fixes

1.0.0-beta12

- Order By on Lazy Loaded Relationship Entities
- Order By on Relationship Entities

1.0.0-beta11

- Some bug fixes with relationship entities
- Real world usage test

1.0.0-beta10

- Lazy loading RelationshipEntities

1.0.0-beta9

- `OrderBy` working with Lazy and findAll()

1.0.0-beta8

- Added `OrderBy` annotations

1.0.0-beta7

- Added proxy implementations

1.0.0-beta6

- Added lazy loading first implementation

1.0.0-beta4

- Added the possibility to define relationship direction as BOTH

1.0.0-beta3

- BC : Renamed `Manager` to `EntityManager`
- Fixed an issue with entities having multiple properties with the same relationship type

1.0.0-beta2

-  Fixed a bug where a related entity was not set on the inversed side
-  Refactored metadata reflection https://github.com/graphaware/neo4j-php-ogm/pull/2

1.0.0-beta1

- First release