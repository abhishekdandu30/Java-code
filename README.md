import java.util.*;

public class CollectionDemo {
    public static void main(String[] args) {
        // Creating a Set of integers
        Set<Integer> numberSet = new HashSet<>();
        numberSet.add(5);
        numberSet.add(2);
        numberSet.add(8);
        numberSet.add(3);
        
        System.out.println("Set of Numbers: " + numberSet);
        
        // Creating a List of strings
        List<String> stringList = new ArrayList<>();
        stringList.add("Apple");
        stringList.add("Banana");
        stringList.add("Cherry");
        stringList.add("Date");
        
        System.out.println("List of Strings: " + stringList);
        
        // Creating a Map of names and ages
        Map<String, Integer> ageMap = new HashMap<>();
        ageMap.put("Alice", 25);
        ageMap.put("Bob", 30);
        ageMap.put("Carol", 28);
        ageMap.put("David", 22);
        
        System.out.println("Map of Names and Ages: " + ageMap);
        
        // Performing operations on the collections
        // Set operations
        numberSet.add(5); // Adding a duplicate element, it will not be added
        numberSet.remove(3);
        
        // List operations
        stringList.add("Fig");
        stringList.remove(1);
        String fruit = stringList.get(2);
        
        // Map operations
        ageMap.put("Eve", 26);
        ageMap.remove("Bob");
        int age = ageMap.get("Carol");
        
        // Displaying the modified collections
        System.out.println("Modified Set: " + numberSet);
        System.out.println("Modified List: " + stringList);
        System.out.println("Modified Map: " + ageMap);
        
        // Iterating through the Map and printing key-value pairs
        System.out.println("Iterating through Map:");
        for (Map.Entry<String, Integer> entry : ageMap.entrySet()) {
            System.out.println(entry.getKey() + ": " + entry.getValue());
        }
    }
}
