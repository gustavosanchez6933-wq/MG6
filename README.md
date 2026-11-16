# MG6
## Devlog
1. If I wrote a for loop inside an Update method, I think the entire loop will complete before the Update Method finishes because the loop is happening every frame before Update() finishes. Therefore, if the for loop takes a REALLY long time to finish, it will make the game lag becuase it's trying to finish the loop. However, the Update method() is stuck in the loop as the loop is really long and so it lags because the Update method cannot continue on without the loop finishing first.

