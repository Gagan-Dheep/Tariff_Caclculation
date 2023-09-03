- C Code Mind Map

  - Include Statements
    - #include <stdio.h>
    - #include <stdlib.h>

  - Structure Definition
    - struct Consumer
      - char name[50]
      - char type
      - int time
      - double energy
      - double tariff

  - Function Definitions
    - void calculateTariff(struct Consumer *consumer)
      - Calculate Tariff
        - Domestic Consumer
          - Tariff = 0.1 * energy
        - Industrial Consumer
          - Tariff = 0.15 * energy
      - Time-Dependent Charges
        - Daytime (9 AM - 5 PM)
          - Additional Charge = 0.05 * energy
        - Nighttime
          - Lower Charge = 0.03 * energy

  - Main Function
    - Declarations
      - int numConsumers
      - struct Consumer *consumers
    - Input (Number of Consumers)
      - scanf("%d", &numConsumers)
    - Memory Allocation
      - malloc(numConsumers * sizeof(struct Consumer))
    - Consumer Data Input Loop
      - for (int i = 0; i < numConsumers; i++)
        - Input
          - Name
          - Type
          - Time
          - Energy
        - Calculate Tariff
          - calculateTariff(&consumers[i])
    - Display Tariffs
      - for (int i = 0; i < numConsumers; i++)
        - printf("Name: %s, Type: %c, Tariff: $%.2lf\n", consumers[i].name, consumers[i].type, consumers[i].tariff)
    - Memory Deallocation
      - free(consumers)

- Conclusion
  - C code to calculate electricity tariffs for consumers based on type, time, and energy consumption.

- Note
  - Proper memory management is essential to prevent memory leaks.
