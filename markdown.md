Program Overview
- Read consumer data from an input file
- Calculate tariffs for consumers
- Sort consumers by tariff
- Write sorted data to an output file

Structures
- Consumer
  - name (string)
  - type (char)
  - time (int)
  - energy (double)
  - tariff (double)

Functions
- calculateTariff(consumer)
  - Calculate tariff based on type and time
- readConsumersFromFile(&consumers, &numConsumers, "input.txt")
  - Open input file
  - Read number of consumers
  - Allocate memory for consumers array
  - Read consumer data
  - Calculate tariff for each consumer
- writeConsumersToFile(consumers, numConsumers, "output.txt")
  - Open output file
  - Write sorted consumer data
- main()
  - Read consumers from input file
  - Sort consumers by tariff
  - Write sorted data to output file
  - Free memory

Data Flow
- Input file ("input.txt") -> readConsumersFromFile -> Consumer array
- calculateTariff -> Update tariff for each consumer
- Sorted Consumer array -> writeConsumersToFile -> Output file ("output.txt")

Control Flow
- main() function controls the program flow
- Reads, processes, and writes data

File Operations
- Input file ("input.txt")
- Output file ("output.txt")

Sorting Algorithm
- Bubble sort used to sort consumers by tariff

Error Handling
- Check for file opening errors
- Memory allocation error
