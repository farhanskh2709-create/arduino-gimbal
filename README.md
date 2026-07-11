# Arduino Gimbal

3-axis Arduino gimbal self-stabilizing platform. 3 MG996R servos. MPU6050 sensor. LM2596 buck converter. 20+ soldered connections.

## Status

NOT WORKING

- Buck converter is working (outputs 5V when powered)
- BUT: voltage persists at the IN terminals (0.8V - 1.6V) of the Buck converter even when the switch is off
- Current leakage somewhere in the circuit
- **Video:** [Gimbal structure assembly] https://youtube.com/shorts/tiyTtlmbnWM?feature=share

## What Works

- 3 servos respond to Arduino
- MPU6050 gives sensor readings
- Frame assembled from 3D printed parts
- All soldering complete (20+ connections)
- Buck converter outputs 5V correctly

## What Doesn't Work

- Switch does not fully cut power
- Voltage leakage at IN terminals (0.8V - 1.6V) when switch is off
- Circuit not safe to run

## Problems Found

1. Insulation damage on wires (shorted, caused heat) - fixed with electrical tape
2. Current leakage - voltage persists at buck input even when switch is off

## What I Did

- Soldered switch, battery holder, buck converter
- Used electrical tape on exposed wires
- Measured voltage: 0.8V - 1.6V at buck IN terminals when switch is OFF
- Switch OFF should read 0V, but it doesn't

## Next Steps

- Find the source of the leakage
- Check switch wiring
- Replace switch if faulty
