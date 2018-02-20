# Brentford Market Place Bus display

## Why? 

The original one was nice, but I felt that there could be improvements in the javascript & html. Also, I wanted an example which used the bus timetable api.
It shows the next n-buses going towards Chiswick and away from Chiswick from a single bus stop 



## Customisation 

The following .getJSON:

```  $.getJSON("https://api.tfl.gov.uk/StopPoint/910GPCKHMQD/arrivals" ```

Can be customised to any TFL station, by changing the `910GPCKHMQD, the code can be found by searching this link 

``` https://tfl.gov.uk/travel-information/stations-stops-and-piers/ ``` 

and snipping the link of the result. For example, Caledonian Road's URL is

```https://tfl.gov.uk/overground/stop/910GCLDNNRB/caledonian-road-barnsbury-rail-station/?Input=Caledonian+Road+%26+Barnsbury+Rail+Station```

Thus it's unique identifier is 910GCLDNNRB. 


Enjoy! 

###    Typical example of an entity:  

```
    "$type": "Tfl.Api.Presentation.Entities.Prediction, Tfl.Api.Presentation.Entities"
    bearing: "76"
    currentLocation: ""
    destinationName: "Eastbound"
    destinationNaptanId: ""
    direction: "outbound"
    expectedArrival: "2018-02-18T22:19:21Z"
    id: "-415760652"
    lineId: "237"
    lineName: "237"
    modeName: "bus"
    naptanId: "490004292F"
    operationType: 1
    platformName: "BN"
    stationName: "Market Place"
    timeToLive: "2018-02-18T22:19:51Z"
    timeToStation: 49
    timestamp: "2018-02-18T22:18:32Z"
    timing: Object { "$type": "Tfl.Api.Presentation.Entities.PredictionTiming, Tfl.Api.Presentation.Entities", countdownServerAdjustment: "-00:00:00.1398078", source: "2018-02-16T11:55:04.668Z", … }
    towards: "Chiswick, Hanwell or Northfields"
    vehicleId: "LK10BXS"
```
