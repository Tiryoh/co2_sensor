# co2_sensor

Python library of CO2 sensor e.g.) MH-Z14A, MH-Z19

## Usage

```python
import time
from co2_sensor.MHZ14A import MHZ14A


def main():
    co2 = MHZ14A("/dev/ttyS0")
    while(1):
        data = co2.get()
        print(data)
        time.sleep(60)

if __name__ == '__main__':
    main()
```
