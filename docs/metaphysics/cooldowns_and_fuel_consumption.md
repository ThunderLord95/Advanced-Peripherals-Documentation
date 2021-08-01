# Cooldowns and fuel consumption

All world changing operations will consume turtle fuel (of course, not if you disable fuel usage in the CC:Tweaked configuration).

Also, most of these operations have cooldowns, so you should consider this when making your code. Hopefully, every active cooldown can be recived via peripheral methods.

If you think that the cooldowns are too long, then this is why the fuel consuming rate is here to help!

A bigger fuel consuming rate will reduce the cooldown, but obviously increase fuel consumption. For example, if a click operation requires 1 fuel point to perform it will have a 5 second cooldown, but with a fuel consumption of 2, you can perform a click operation in half the time at 2.5 seconds, but with a cost of 2 fuel points.

However, the fuel consumption rate is not so simple! Every mechanic soul has a max fuel consumption limitation that can be retrieved via the `getConfiguration()` method.

Also, the amount of fuel points consumed will grow more than the cooldown reduces. For example, a fuel consumption of 3 will require 4 fuel points, and the fuel points used will keep increasing the higher the fuel consumption is set to.
