## Documentation

### Hardware filters in hardware.helper

This document details how the hardware filters in `/hardwadware.helper.js` are applied in the "<name_function>" function.
#### The requested parameters in the /hardware endpoint are

- type #enter 'asic' or 'altcoin' separated by "-" to filter hardware by 'ASIC | ALTCOIN'
```
    filter case example:
        1. type=asic                // by asic
        2. type=asic-alcoin         // by 'asic' and 'altcoin'
        3. type=alcoitn             // by alcoitn
```
- isPSP #enter 'true' or 'false' to filter hardware by 'Premium..........'
```
    filter case example:
        1. isPSP=true               // hardware filter by 'Premium..........'
        2. isPSP=false              // non-'Premium..........' hardware filter
```
- isDelivery #enter 'true' or 'false' to filter hardware by 'at home | other'
```
    filter case example:
        1. isDelivery=true          // hardware filter by 'Premium..........'
        2. isDelivery=false         // non-'Premium..........' hardware filter
```
- compass_finance #enter 'true' or 'false' to filter hardware by 'Plan..........'
```
    filter case example:
        1. compass_finance=true     // by 'Plan..........'
        2. compass_finance=false    // non-'Premium..........' hardware filter
```
- online_date #enter interval 'init date' and 'end date' to filter hardware
```
    notes:
        - to separate the interval "-"
    filter case example:
        1. online_date=initdate-enddate     // by date range for onlinde_date
```
- price #enter interval 'init price' and 'end price' to filter hardware by 'cost'
```
    notes:
        - to separate the interval "-"
    filter case example:
        1. price=initprice-endprice         // by price range by hardware cost
```
-   manufactur_model #enter manufacturer and its selected models to filter hardware by 'Manufacturer and baseModelName'
```
    notes: 
        - to separate manufacturer use "-"
        - to separate manufacturer and their models use "|"
        - to separate models from a manufacturer use ":"

    filter case example:
        1. manufactur_model=manufact1                                   // by one manufacturer
        2. manufactur_model=manufact1-manufact2                         // by many manufacturers [to add more manufacturers, separate with "-"]
        3. manufactur_model=manufact1|xmodel                            // by one manufacturer and one of its models [to add models from a manufacture, separate with "|"]
        4. manufactur_model=manufact1|xmodel:ymodel                     // by one manufacturer and many of its models [to add more models, separate with ":"]
        5. manufactur_model=manufact1|xmodel:ymodel-manufact2           // by many manufacturer and many of its models 
        6. manufactur_model=manufact1|xmodel-manufact2|zmodel           // by one manufacturer and one of its models
        7. manufactur_model=manufact1|xmodel-manufact2|zmodel:wmodel    // by one manufacturer and many of its models 
```




