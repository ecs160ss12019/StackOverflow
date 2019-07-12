# Acceptance Criteria

## GUI

1. The GUI should include:
    a. Left button, to move the Phoenix 3000 left.
    b. Right button, to move the Phoenix 3000 right.
    c. Shoot button, to shoot physical signals from the Phoenix 3000.
    d. Score counter on the top, to display player’s score.
    e. Lives counter on the top right, to display the number of lives left for Phoenix 3000.

2. Given the player shoots, if a Malware is hit, then score should be updated on top of the screen.

3. Given the number of lives for Phoenix 3000 starts with 3, if the Phoenix 3000 gets hit or clears a wave of Malware, then the number of lives should decrease or increase accordingly on the top right of the screen.

4. Given the Phoenix 3000 gets hit, if it’s out of lives, then the game should end and a screen should ask for a name and then display the top 10 high scores.


## Phoenix 3000

1. Given the Phoenix 3000 shoots, if the physical signal hits a Malware, then that Malware gets destroyed.

2. Given the Phoenix 3000 shot, if the physical signal did'nt hit a Malware or reach the top of the screen, then the player cannot shoot another shot.

3. Given the Phoenix 3000 shoots a Malware, if that Malware is the last in the Wave, then the round starts again with a new Wave which moves 1 level below where it started in the previous wave.

## Malware

1. Given a Malware shoots a virus, if the virus hits the Phoenix 3000, then the Phoenix 3000 gets destroyed and loses a life.

2. Given a Malware moves left to right side at the start of the game, if the right most Malware hits the end of the screen, then they move down and continue in the opposite direction to repeat the same process.

3. Given the Malware hit either end of the screen, if they move down, then their movement and fire rate speed increases.

4. Given 3 Malwares have shot and it has'nt hit or touched the bottom end of the screen, if another Malware tries to shoot a virus, then that Malware is unable to shoot the virus.

5. Given that there are 3 different types of Malware, if Phoenix 3000 hits any one of them, then the player gets a score of 10, 20, or 30 points depending on which type of Malware was hit.

6. Given randomly every 30 seconds a Huge Malware appears at the top of all the Malwares, if the Huge Malware is hit, then the player gets a random score under 300 points.


## Firewall

1. Given the game starts with 4 defense firewalls, if the firewall is hit by a virus or by a physical signal, then the defense firewall should break a little but not let the projectile pass through.

2. Given there is some firewall, if it gets hit and clears a path between the firewall, then the projectile should pass through,

3. Given the Phoenix 3000 hits a Malware, if the wave is finished, then the new game should start with the same condition of firewall and it won’t be replenished.
