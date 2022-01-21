@@@ atlas-signature
Query
-->
TimeSeriesExpr
@@@

Compute the average recorded value for [timers] and [distribution summaries]. This
is calculated by dividing the total amount recorded by the number of recorded values.

[timers]: ../../spectator/core/meters/timer.md
[distribution summaries]: ../../spectator/core/meters/dist-summary.md

@@@ atlas-example { hilite=:dist-avg }
Before: /api/v1/graph?w=200&h=125&s=e-3h&e=2012-01-01T07:00&tz=UTC&q=name,playback.startLatency,:eq
After: /api/v1/graph?w=200&h=125&s=e-3h&e=2012-01-01T07:00&tz=UTC&q=name,playback.startLatency,:eq,:dist-avg
@@@