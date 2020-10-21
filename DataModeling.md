# Data models

### Metrics

- **SortedSets** 
- **TimeSeries** 

**SortedSets**

- Key as: f"metric:{unit.value}:{time.strftime('%Y-%m-%d')}:{site_id}" 
  (metric:wHg:2020-01-01:1)
- Data as: 1 -> 1:19.5, 2 -> 2:18.0 
    1. score: minute as int(to preserve ordering on retrieve)
    2. data: minute prefix(to make it unique):metric value (like tC)


