# Refrigerator Circuit Analysis

## Overview

As part of the MBSE study, the electrical circuit of an LG GL-205KAG5 refrigerator was analyzed to correlate the physical implementation with the SysML system model. This analysis validates how functional requirements are realized through electrical components.

## Circuit Operation

The refrigerator operates from a **220–240 V AC, 50 Hz** power supply. The thermostat continuously monitors the cabinet temperature and controls the compressor accordingly.

1. AC power is supplied to the refrigerator.
2. When the internal temperature exceeds the set point, the thermostat closes the circuit.
3. Power flows through the Overload Protector (OLP) and PTC starter to energize the compressor.
4. The compressor circulates R134a refrigerant through the refrigeration cycle, removing heat from the storage compartment.
5. Once the desired temperature is achieved, the thermostat opens the circuit and switches the compressor OFF.
6. Opening the refrigerator door activates the door switch, turning ON the interior lamp.
7. The refrigerator repeats this cycle automatically to maintain the desired cooling temperature.

## MBSE Perspective

The circuit represents the physical realization of several system functions modeled in SysML.

| System Function | Electrical Implementation |
|-----------------|---------------------------|
| Temperature Monitoring | Thermostat |
| Cooling Control | Compressor |
| Motor Protection | Overload Protector (OLP) |
| Motor Starting | PTC Starter & Run Capacitor |
| User Interaction | Door Switch & Lamp |
| Power Distribution | AC Supply & Wiring |

This study demonstrates how functional requirements captured in the Requirement Diagram are implemented through actual hardware components, improving traceability between system requirements and physical architecture.
