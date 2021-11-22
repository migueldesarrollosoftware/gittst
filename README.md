## Documentation

### Hardware filters in hardware.helper

This document details how the hardware filters in `/hardwadware.helper.js`.
Applied in the "<name_function>" function.

#### The requested parameters for the filter by multiple fields in the /hardware endpoint are

- isDelivery #enter 'true' or 'false' to filter hardware by 'Delivery | Hosted'
```
    filter case example:
        1. isDelivery=true           // by 'Delivery'
        2. isDelivery=false          // by 'Hosted'
```
- isPSP #enter 'true' or 'false' to filter hardware by 'Premium Service Plan Eligible'
```
    filter case example:
        1. isPSP=true                // by 'Premium Service Plan Eligible'
        2. isPSP=false               // non-'Premium Service Plan Eligible'
```
- compass_finance #enter 'true' or 'false' to filter hardware by 'Payment Plan Eligible'
```
    filter case example:
        1. compass_finance=true     // by Payment Plan Eligible
        2. compass_finance=false    // non-Payment Plan Eligible
```
- type #enter 'asic' or 'altcoin' separated by "-" to filter hardware by 'ASIC | ALTCOIN'
```
    filter case example:
        1. type=asic                 // by asic
        2. type=asic-alcoin          // by 'asic' and 'altcoin'
        3. type=alcoitn              // by alcoitn
```
- countries #enter some 'countries' separated by "-" to filter hardware by 'Facility country'
```
    filter case example:
        1. countries=USA               // by USA
        2. countries=USA-Canada        // by 'USA' and 'Canada' [to add countries, separate with "-"]
        3. countries=Canada            // by Canada
```
- online_date #enter interval 'init date' and 'end date' to filter hardware
```
    notes:
        - use to separate the interval "-"
    filter case example:
        1. online_date=initdate-enddate     // by date range for online_date
```
- price #enter interval 'init price' and 'end price' to filter hardware by 'cost'
```
    notes:
        - use to separate the interval "-"
    filter case example:
        1. price=initprice-endprice         // by price range by hardware cost
```
- hashrate #enter interval 'init hashrate' and 'end hashrate' to filter hardware by 'hashrate'
```
    notes:
        - use to separate the interval "-"
    filter case example:
        1. price=inithashrate-endhashrate         // by hashrate range by hardware hashrate
```
- manufacturers_model #enter manufacturer and its selected models to filter hardware by 'Manufacturer and baseModelName'
```
    notes: 
        - use to separate manufacturer "-"
        - use to separate manufacturer and their models "|"
        - use to separate models from a manufacturer ":"

    filter case example:
        1. manufacturers_model=manufact1                                   // by one manufacturer
        2. manufacturers_model=manufact1-manufact2                         // by many manufacturers [to add more manufacturers, separate with "-"]
        3. manufacturers_model=manufact1|xmodel                            // by one manufacturer and one of its models [to add models from a manufacture, separate with "|"]
        4. manufacturers_model=manufact1|xmodel:ymodel                     // by one manufacturer and many of its models [to add more models, separate with ":"]
        5. manufacturers_model=manufact1|xmodel:ymodel-manufact2           // by many manufacturer and many of its models 
        6. manufacturers_model=manufact1|xmodel-manufact2|zmodel           // by one manufacturer and one of its models
        7. manufacturers_model=manufact1|xmodel-manufact2|zmodel:wmodel    // by one manufacturer and many of its models 
```




