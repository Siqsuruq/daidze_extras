# daidze_extras
Some extra things we use in Daidze, but can be used anywhere:

All sql are tested on PostgreSQL server 10-12, but should work on any other:

__Some notes about Usage:__

1. Get list of timezones ordered by alphabet:

```SELECT zone_name FROM timezone ORDER BY zone_name ASC```

2. In "timezone" country_code column is equivalent to iso(2 digits) in country code. Countries with Timezones:

```SELECT country.nicename, timezone.zone_name FROM country LEFT JOIN timezone ON  timezone.country_code = country.iso ORDER BY country.nicename ASC```

Etc.

Have fun!!!
