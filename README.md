## documentation

### hardware filters in harware.helper

This document details how the hardware filters in `/harwadware.helper.js` are applied in the "<name_function>" function.

#### the requested parameters in the /hardware endpoint are:

    -  type                    #type [multiple select] enter 'asic' or 'altcoin' separated by "-" to filter hardware by 'ASIC | ALTCOIN'
        cases:
            type=asic          // hardware filter by asic
            type=asic-alcoitn  // hardware filter by 'asic' and 'altcoin'
            type=alcoitn       // hardware filter by alcoitn
        
    -   isPSP                   #enter 'asic' or 'alt mint' to filter hardware by 'ASIC | ALTMINT'
    -   compass_finance         #enter 'asic' or 'alt mint' to filter hardware by 'ASIC | ALTMINT'
    -   manufactur_model        #enter 'asic' or 'alt mint' to filter hardware by 'ASIC | ALTMINT'
    -   online_date             #enter 'asic' or 'alt mint' to filter hardware by 'ASIC | ALTMINT'




