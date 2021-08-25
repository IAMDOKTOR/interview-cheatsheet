Основное отличие можно сформулировать так: 
> Если вам искать элементы списка важнее, чем изменять список - берите ArrayList, а если наоборот - то LinkedList.

__ArrayList__ - это когда, грубо говоря, мы можем вставить в массив несколько разных списков.

Пример работы на Java:

```java
ArrayList al = new ArrayList();

al.add("C");
al.add("A");
al.add("E");
al.add("F");
al.add(1, "A2");

System.out.println("Содержимое al: " + al);

al.remove("F");
al.remove(2);
```

__LinkedList__ - это когда у нас есть очередь из нескольких элементов, где каждый элемент знает, где хранится следующий и где был предыдущий.

Пример на Java:

```java
LinkedList ll = new LinkedList();

ll.add("F");
ll.add("B");
ll.addLast("Z");
ll.addFirst("A");
ll.add(1, "A2");
System.out.println("Содержимое ll: " + ll);

// удаление элементов
ll.remove("F");
ll.remove(2);
System.out.println("Содержимое ll: " + ll);

// удалить первый и второй элемент 
ll.removeFirst();
ll.removeLast();
System.out.println("Содержимое ll: " + ll);
```


Подробнее:
https://proft.me/2014/10/29/raznica-mezhdu-arraylist-i-linkedlist/
