<div align="center">

# 🏭 Supplier-Consumer - Threads and Wait/Notify

### Java · Concurrency · Multithreading

Ten suppliers and ten consumers coordinated through a shared meeting room using synchronized wait/notify, with timestamped logging.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Concurrency](https://img.shields.io/badge/Concurrency-5382A1?style=for-the-badge&logoColor=white)
![Multithreading](https://img.shields.io/badge/Multithreading-6E4C13?style=for-the-badge&logoColor=white)

</div>

## What it does

| Feature | Detail |
|---|---|
| 10 suppliers + 10 consumers | Twenty threads sharing one bounded resource |
| Wait/notify coordination | Producers wait when the room is full, consumers wait when it is empty |
| Synchronized access | `MeetingRoom` guards shared state so threads never corrupt it |
| Timestamped logging | Each supply/consume event is logged with its time |

## Run

```bash
javac *.java
java SupplierConsumerSimulation
```

## Files

- `SupplierConsumerSimulation.java` - driver (grade: 9/10)
- `Supplier.java`, `Consumer.java` - producer and consumer threads
- `MeetingRoom.java` - shared, synchronized meeting room

> Originally a Java Programming II (CIS 36B) project, extracted here as a standalone repo from [java-algorithms-and-concurrency](https://github.com/afshinmalek/java-algorithms-and-concurrency).
