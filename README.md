# pxt-sonar
A PXT package to use sonar sensors (ping) such as the HC-SR04

## Usage

This package contains a ``ping`` block that can return the distance to an obstacle detected by the sonar.

```sig
sonar.ping(DigitalPin.P1, DigitalPin.P2, PingUnit.Inches);
```

## Charting the distance

Use the ``plot bar graph`` block to visualize the distance reported by your sensor.

```blocks
basic.forever(() => {
    let p = sonar.ping(DigitalPin.P1, DigitalPin.P2, PingUnit.Inches);
    led.plotBarGraph(p, 0);
})
```

## License
MIT

## Supported targets
* for PXT/microbit
(The metadata above is needed for package search.)

```package
sonar=github:Microsoft/pxt-sonar
```