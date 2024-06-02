```java
public static void main(String[] args) {
    MemoryMonitor monitor = new MemoryMonitor();
    monitor.start();
    System.out.println(monitor.getUsedMemory());
    List<String> list=new ArrayList<>();
    for (int i = 0; i < 100000; i++) {
        list.add(String.valueOf(i));
    }
    System.out.println(monitor.getUsedMemory());
}
```

