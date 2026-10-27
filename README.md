# Celestial Bodies Database

Completed PostgreSQL project for the freeCodeCamp Relational Databases certification. Built and tested in the official GitHub Codespaces environment using CodeRoad.

## Database

The catalog uses fictional names and measurements for demonstration purposes.

| Table | Rows | Purpose |
| --- | ---: | --- |
| galaxy_type | 3 | Galaxy classifications |
| galaxy | 6 | Galaxies and their classifications |
| star | 6 | Stars linked to galaxies |
| planet | 12 | Planets linked to stars |
| moon | 20 | Moons linked to planets |

Every table has an automatically incrementing primary key and a unique, non-null VARCHAR name. Foreign keys preserve the relationships, and CHECK constraints reject invalid ages, counts, distances, and sizes. The schema uses INT, NUMERIC, TEXT, and BOOLEAN columns as required.

## Submission file

`universe.sql` is the complete database export, including the schema, data, constraints, and sequences.

Restore it in the freeCodeCamp PostgreSQL environment with:

```sh
psql -U postgres -f universe.sql
```

This export was generated with:

```sh
pg_dump -cC --inserts -U freecodecamp universe > universe.sql
```

## Validation

All official CodeRoad project tests passed, and the tutorial displayed its completion confirmation.
