# MKS SERVO42D CAN arduino example
 some basic example code


I am using a Teensy 4.1 but any arduino that has a built in CAN controller should work with a little code modification.

For CAN transceiver I am using Waveshare SN65HVD230 CAN Board. This board seams to have a built in resistor between canH and canL
https://www.amazon.com/gp/product/B00KM6XMXO/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1

Wiring.

canRX on CAN board -> pin 23 on Teensy (CRX1)
cabTX on CAN board -> pin 22 on Teensy (CTX1)
3.3v on CAN board -> Teensy 3.3v
gnd on CAN board -> Teensy gnd

CanH on CAN board -> CanH on motor
CanL on CAN board -> CanL on motor

Motor gnd -> Teensy gnd
Motor can resistor pins get bridged (right under canbus pins)

My code is very basic and not a finished product by any means. It is just meant to be used as a starting point to test and impliment the motor into your own project.

CAN codes and instructions are at https://github.com/makerbase-motor/MKS-SERVO57D/blob/master/User%20Manual/MKS%20SERVO42%2657D_CAN%20User%20Manual%20V1.0.4.pdf
