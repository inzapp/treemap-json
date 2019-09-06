# Treemap JSON
JSON with custom comparator using treemap<br>
You can sort json by json key
## Usage
```java
json = new JSONObject(new Comparator<String>() {
    @Override
    public int compare(String a, String b) {
        // parameter a, b is json key
        // just implement your comparator
        return a.compareTo(b);
    }
});
```
Using lambda expression
```java
json = new JSONObject((Comparator<String>) (a, b) -> {
    return a.compareTo(b);
});
```
