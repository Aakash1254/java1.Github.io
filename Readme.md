# Solution1

Solution1 is a Java program that simulates events based on biased outcomes. It uses random weighted selection to generate simulation results for a given set of outcomes and occurrences.

## Getting Started

To run the program, you need to have Java installed on your machine. Follow these steps:

1. Clone the repository or download the source code files.

2. Open a terminal or command prompt and navigate to the directory where the `Solution1.java` file is located.

3. Compile the Java file using the `javac` command:

# javac Solution1.java okk my name is akash

4. Run the compiled program using the java command:

# java Solution1

# The program will execute and display the simulation results for biased dice and biased coin events.

# Usage

The program includes example inputs for biased dice and biased coin events. You can modify these inputs or add your own biased outcomes by editing the main method in the Solution1.java file.

List<Pair<String, Integer>> biasedDice = new ArrayList<>();
// Add biased dice outcomes and probabilities
biasedDice.add(new Pair<>("1", 10));
biasedDice.add(new Pair<>("2", 30));
biasedDice.add(new Pair<>("3", 15));
biasedDice.add(new Pair<>("4", 15));
biasedDice.add(new Pair<>("5", 30));
biasedDice.add(new Pair<>("6", 0));

List<Pair<String, Integer>> biasedCoin = new ArrayList<>();
// Add biased coin outcomes and probabilities
biasedCoin.add(new Pair<>("Head", 35));
biasedCoin.add(new Pair<>("Tail", 65));

// Simulate biased dice
Map<String, Integer> diceResults = simulateEvent(biasedDice, 1000);
System.out.println("Dice simulation results:");
for (Map.Entry<String, Integer> result : diceResults.entrySet()) {
System.out.println(result.getKey() + ": " + result.getValue());
}

// Simulate biased coin
Map<String, Integer> coinResults = simulateEvent(biasedCoin, 1000);
System.out.println("Coin simulation results:");
for (Map.Entry<String, Integer> result : coinResults.entrySet()) {
System.out.println(result.getKey() + ": " + result.getValue());
}
