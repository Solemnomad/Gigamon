* Hybrid port can be used as a source or destination for a flow Map. It can be a loopback port or traffic port. It doesn't need an SFP to be loopback.
* Can encapsulate traffic, can tunnel traffic
* Inside maps, can duplicate traffic to a hybrid port as well as your local tool ports.
* Inside another map, can take the traffic from
* packet slicing can take portions (payload normally to possibly take out CUI, etc) out of traffic.
* Header slicing is what it sounds like. Can also be used to remove encapsulation.
* Can use a pass all map to give everything to a tool port and then filter to (EXCEPT x)
