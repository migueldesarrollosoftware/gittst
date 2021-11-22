## documentation

### hardware filters in harware.helper

This document details how the hardware filters in `/harwadware.helper.js` are applied in the "<name_function>" function.

```
    - type                    #[multiple select] enter 'asic' or 'altcoin' separated by "-" to filter hardware by 'ASIC | ALTCOIN'
        cases:
            1. type=asic          // hardware filter by asic
            2. type=asic-alcoitn  // hardware filter by 'asic' and 'altcoin'
            3. type=alcoitn       // hardware filter by alcoitn
```

#### the requested parameters in the /hardware endpoint are:
```
    - type                    #[multiple select] enter 'asic' or 'altcoin' separated by "-" to filter hardware by 'ASIC | ALTCOIN'
        cases:
            1. type=asic          // hardware filter by asic
            2. type=asic-alcoitn  // hardware filter by 'asic' and 'altcoin'
            3. type=alcoitn       // hardware filter by alcoitn
```

    - isPSP                   #enter 'true' or 'false' to filter hardware by 'Premium..........'
        cases:
            1. isPSP=true          // hardware filter by 'Premium..........'
            2. isPSP=false         // non-'Premium..........' hardware filter

    -   compass_finance         #enter 'true' or 'false' to filter hardware by 'Plan..........'
        cases:
            1. compass_finance=true          // hardware filter by 'Plan..........'
            2. compass_finance=false         // non-'Premium..........' hardware filter

    -   manufactur_model        #enter manufacturer and its selected models to filter hardware by 'Manufacturer and baseModelName'
        notes: 
            - to separate manufacturer use "-"
            - to separate manufacturer and their models use "|"
            - to separate models from a manufacturer use ":"

        cases:
            1. manufactur_model=manufact1          // hardware filter by 'Plan..........'
            2. manufactur_model=false         // non-'Premium..........' hardware filter
    -   online_date             #enter 'asic' or 'alt mint' to filter hardware by 'ASIC | ALTMINT'




