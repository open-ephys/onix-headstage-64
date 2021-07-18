# Coaxial Cable Module
This small board has castellated edge contacts and is soldered onto the
headstage's center contacts to provide coax IO. It contains a portion of the
power conditioning circuit on the main board and is therefore necessary for
headstage operation. There are two variants:

1. coax-adapter-protected (recommended)
    - Contains over/under-voltage lockout circuit that ensures unregulated
      input voltage will not damage headstage but requires that the user tune
      the power supply to account for cable voltage drop
    - Has extra bulk capacitance, which reduces noise
1. coax-adapter-regulated
    - Contains a step-down regulator that ensures proper 5.5V supply to the
      headstage so long as input voltage is greater than 5.5V
    - Has less bulk capacitance and switching supply may introduce noise

## Bill of Materials
The bill of materials for this device can be found
[here](https://docs.google.com/spreadsheets/d/1pUGBYAdJs2eZZaEnTpPPK72m9BNobIhAjmIrxtYpmq0/edit?usp=sharing).

## Manufacturing Requirements
This PCB has the following requirements:

- 4 copper layers
- 0.6 mm (or thinner) total thickness
- Castellated edge contacts
