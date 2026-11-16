# MG6
## Devlog
1. If I wrote a for loop inside an Update method, I think the entire loop will complete before the Update Method finishes because the loop is happening every frame before Update() finishes. Therefore, if the for loop takes a REALLY long time to finish, it will make the game lag becuase it's trying to finish the loop. However, the Update method() is stuck in the loop as the loop is really long and so it lags because the Update method cannot continue on without the loop finishing first.

2. An issue that I found while testing the game is that if I jump upwards to the two highest platforms in the game, I'm able to jump again at the bottom of the platform. I think the reason why this happens is because the code is checking the player's velocity to tell if the player can go through the platoform or not. Since I reach the maxmimum height of my jump, the cat's velocity is back to 0 which allows me to jump again because  _collider.enabled becomes true again.
