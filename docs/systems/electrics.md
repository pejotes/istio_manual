# Electrics

_Istio_ runs both a 12V DC system and a 24V DC system.

The battery main switch is located under the navigation station bench.

![Electrical diagram](../assets/electrical-diagram.png)

## Consumption

Typical power consumption on the boat is around 1.2kWh per day in the summer months. In winter and shore power it ranges around 3-6kWh per day depending on how much the diesel heater and the [[engine]] frost guard need to run.

The primary electrical consumers on the boat are:

* Refrigerator
* Engine frost guard
* Diesel heater
* Autopilot
* Personal computers

In situations where batteries are running low, it is a good idea to disable some or all of these. Actual consumption is visible in VictronConnect or VRM.

## Storage

The boat has two battery banks:

* 20Ah Li-Ion battery located in the port cockpit locker
* 120Ah LiFePO4 house bank located under the technical compartment

The two battery banks are normally isolated from each other, except for:

* There is a 30A DC-DC charger to charge house bank from the starter circuit when alternator is running
* The inverter-charger trickle-charges the starter bank from house circuit at 1A when house bank is charging

## Production

### Fixed solar panels

The vessel has two fixed solar arrays:

* 240W array (2×120W panel) on the stern arch
* 120W panel on top of the hatch garage

Each of these is connected to its own Victron SmartSolar charge controller.

### FLINsail

The boat carries a deployable 300W [FLINsail](https://flin-solar.de). This is a set of three panels that can be hoisted in the mast like a mainsail.

#### Deploying the FLINsail

* [ ] Attach the FLINsail bag on top of the boom
* [ ] Open the bag and attach the main halyard to the hook labeled _Head_
* [ ] Pull main halyard so that the lines coming from the _Head_ hook are lifted
* [ ] Attach the hook labeled _Clew_ to the end of the boom
* [ ] Attach the hook labeled _Tack_ to the soft shackle hanging under the boom gooseneck
* [ ] Pull main halyard until first panel is over the sail entry gate
* [ ] Attach the sail slide into the mainsail rail
* [ ] Repeat until all three panels are attached to the rail
* [ ] Pull main halyard until all is nice and tight
* [ ] Turn the panels and the boom towards the sun
* [ ] Get the solar MC4 cable from under the deck solar panel and attach to the connectors on the FLINsail

**Note: The maximum wind speed for deploying the FLINsail is 18kt**

### Shore power charger

The boat's shore power connection runs to a [Victron MultiPlus 500VA](https://www.victronenergy.com/inverters-chargers/multi-500-va) inverter-charger. Shore power RS692 plug is located in the anchor locker. The shore power CEE cord is typically in the lazarette. There is a CEE to Schuko adapter in the lazarette as needed, as well as an extension cord.

The shore power connection is isolated with a Victron galvanic isolator. This is located next to the shore power main breaker in the hull side of the technical compartment.

## Monitoring

The boat's electrical system can be monitored via:

* [Victron VRM](https://vrm.victronenergy.com) remote monitoring system
* [Electricity Grafana dashboard](http://lille-oe-pi.local:3000/d/6EmAzaA7k/electricity?orgId=1&refresh=30s) on board


