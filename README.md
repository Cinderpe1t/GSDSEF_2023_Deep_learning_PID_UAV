# GSDSEF 2023 Deep learning network engaged PID controller in a UAV
- First presented at 2023 Greater San Diego Science and Engineering Fair (GSDSEF)
- Improved results presented at IEEE HORA 2023 conference
## Codes
- `sonoma_raceway.world`: Gazebo world and wind set up
- `RL_agent_px4_v04_all_v05.ipynb`: Mission controller Python code to train DRL
## Wind plug-in set up with 5m/s average speed
```
    <plugin name='wind_plugin' filename='libgazebo_wind_plugin.so'>
      <frameId>base_link</frameId>
      <robotNamespace/>
      <windVelocityMean>5.0</windVelocityMean>
      <windVelocityMax>7.0</windVelocityMax>
      <windVelocityVariance>1</windVelocityVariance>
      <windDirectionMean>1 1 0</windDirectionMean>
      <windDirectionVariance>0.5</windDirectionVariance>
      <windGustStart>0</windGustStart>
      <windGustDuration>0</windGustDuration>
      <windGustVelocityMean>0</windGustVelocityMean>
      <windGustVelocityMax>0.0</windGustVelocityMax>
      <windGustVelocityVariance>0</windGustVelocityVariance>
      <windGustDirectionMean>0 0 0</windGustDirectionMean>
      <windGustDirectionVariance>0</windGustDirectionVariance>
      <windPubTopic>world_wind</windPubTopic>
    </plugin>
```
