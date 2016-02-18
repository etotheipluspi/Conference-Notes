
Mobile intervention:
    * Reaching helath goals
    * There when you need it and not intrusive when you dont (POMDP?)

Track time series:
    * Ot, At, Yt (obs, action, response)
    * Decision times: regular intervals of times or on demand (could do better with POMDP!)
    * Intervals depends on instance (heart vs smoking intervention 10 min vs 2hrs)
    * Reduce self-reported data (collect data automatically)
    * Large state space (location, step cout, calendar data, etc)

UI:
    * Ping with notification on phone: thumbs up, thumbs down, or snooze (no notifications for x hours)
    * System can also choose not to notify


Approaches:
    * Trial design to collect meaningful data
    * batch RL (learn warm-start treatment policy)
    * Online RL

Batch RL, learning treatment policies:
    * Learn stochastic policy pi(a|s) (parameterazied by theta)
    * Actor-critic  - the work here is developing clinical trials that give you meaningful data to learn from
