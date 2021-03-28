# Sensor-parameters-and-RTK-system-details
Sensor parameters and RTK system details in ITS paper

## 1. Vehicle Dynamics Parameters

| Parameter                                               | Value  |
| ------------------------------------------------------- | ------ |
| Total Width(kg)                                         | 1079.1 |
| Wheel Base(m)                                           | 2.305  |
| Distance from the center of mass to the front axles (m) | 1.039  |
| Distance from the center of mass to the rear axles (m)  | 1.266  |
| Height of vehicle center of mass (m)                    | 0.54   |
| Transmission ratio from steering wheel to front wheel   | 17.4   |
| Vertical moment of inertia (kg·m2)                      | 1403   |
| Wheel radius (m)                                        | 0.29   |
| Lateral stiffness of front wheels (N/rad)               | -60164 |
| Lateral stiffness of rear wheels (N/rad)                | -63776 |

## 2. The Visual-inertial System Parameters

| Parameter                           | Value                                   |
| ----------------------------------- | --------------------------------------- |
| Frame rate                          | 10-60FPS, settable                      |
| Resolution                          | 1280×720                                |
| FOV                                 | horizontal: 121°vertical: 105°          |
| Focal                               | 2.45mm                                  |
| Exposure                            | global shutter                          |
| IMU Type                            | Bosch BMI088                            |
| IMU rate                            | 100-500Hz，settable                     |
| Zero offset (typ. over life-time)   | (A) : ±20mg<br />(G): ±1°/s             |
| Noise density (typ.)                | (A): 175 μg/√Hz<br />(G): 0.014 °/s/√Hz |
| Camera-IMU Synchronization accuracy | <1ms                                    |

Data for Bosch BMI088 comes from https://www.bosch-sensortec.com/products/motion-sensors/imus/bmi088/

## 3. Useful details for RTK system

#### **The description of the used "position type" in RTK/GNSS measurements:**

**NARROW_INT:** 

Multi-frequency RTK solution with carrier phase ambiguities resolved to narrow-lane integers

Precision: <0.05m

**PSRDIFF:**

Solution calculated using pseudorange differential (DGPS, DGNSS) corrections

Precision: 0.1m-0.9m

**SINGLE:**

Solution calculated using only data supplied by the GNSS satellites

Precision: >1m



#### Signal Sources

GPS、GLONASS、Galileo、BeiDou



#### ALIGN Heading Accuracy

0.5 m baseline 0.40°

1.0 m baseline 0.20°

2.0 m baseline 0.10°



#### More details can be found in:

https://novatel.com/support/previous-generation-products-drop-down/previous-generation-products/span-on-propak6-receiver can download manuals and product sheets of Novatel Protak6 RTK system