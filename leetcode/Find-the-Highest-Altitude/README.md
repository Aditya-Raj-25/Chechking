# Find the Highest Altitude

- **Platform:** leetcode
- **Language:** python3
- **Submission ID:** 1574803755

## Solution Code

```py
class Solution:
    def largestAltitude(self, gain: List[int]) -> int:
        altitude = 0
        max_altitude = 0
        
        for g in gain:
            altitude += g
            max_altitude = max(max_altitude, altitude)
        
        return max_altitude
```