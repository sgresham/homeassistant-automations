# homeassistant-automations

My Automations for Home Assistant relevant to Localvolts and SigEnergy

## Automations

This repository contains 10 automations:

1. **Allow Solar Export to Grid**  
   Exports solar energy to the grid when the battery is full (over 99%), there is profit, and it is daytime (9am-5pm).

2. **Deny Export to Grid when value is greater than 30 cents**  
   Stops exporting to the grid when the value drops below $0.30/kWh during evening hours (6pm-8pm).

3. **Do Not Export when profit is negative**  
   Prevents exporting to the grid if the profit would be negative during the day (9am-5pm) and battery is full.

4. **Off: Buy from grid 12am-5am**  
   Turns off grid buying if the cost is high (> $0.20/kWh) and battery is low (<50%) between midnight and 5am.

5. **Off: Buy from grid 12pm-5pm**  
   Turns off grid buying if the cost is high and battery is low between noon and 5pm.

6. **Off: Pool pump daytime if battery under 25%**  
   Shuts off the pool pump during the day if battery drops below 25%.

7. **On: Allow Export to Grid when value is greater than 30 cents**  
   Enables grid export if the export value is more than $0.30/kWh during evening peak (6pm-8pm).

8. **On: Buy from grid 12am-5am**  
   Turns on grid buying if energy is cheap (< $0.20/kWh) and battery is low between midnight and 5am.

9. **On: Buy from grid 12pm-5pm**  
   Turns on grid buying if energy is cheap and battery is low between noon and 5pm.

10. **On: Pool pump daytime if battery over 25%**  
    Turns on the pool pump during the day if the battery is above 25%.

---

Each automation is stored as a single YAML file and designed for Home Assistant’s Automations UI. See each file for full details and conditions.
