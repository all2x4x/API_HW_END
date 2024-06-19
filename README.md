# API_HW_END
```Java
import java.util.*;

public class PhoneBook    public static void main(String[] args) {
        // Создаем HashMap для хранения имени и списка телефон
        Map<String, List<String>> phoneBook = new HashMap<>();

        // Добав записи в телефонную книгу
        addContact(phoneBook, "Иванов", "1234567890");
        addContact(phoneBook, "Петров", "9876543210");
        add(phoneBook, "идоров", "5555555555");
        addContact(phoneBook, "Ианов", "1111111111");

        // Выводим отсортированный по убыванию список контактов
        List<Map.Entry<String, List<String>>> sortedContacts = new ArrayList<>(Book.entrySet());
        
       Collections.sort(sortedContacts,
           (contact1, contact2) -> Integer.compare(contact2.getValue().(), contact1.getValue().size()));

       for (Map.Entry<String,List<String>> entry : sortedContacts) {
           String name = entry.getKey();
           List<String> phoneNumbers =.getValue();
           System.out.println("Имя: " + name);
           
            for (String phoneNumber : phoneNumbers) {
                System.out.println("Телефон: "+ phoneNumber);
            }
            
            System.out.println("-----------------");
         }
    }

    private static void addContact(Map<String, List<String>> phoneBook name,String phoneNumber){
         if (!phoneBook.containsKey(name)) {
             // Если имя не существует в тонной книге,
             // добавляем новую запись с пустымком номеров
             phoneBook.put(name,new ArrayList<>());
         }

         Получаем список номеров для данного имени и добавляем новый номер
          List <String> numbers=phoneBok.get(name);
          numbers.add(phoneNumber);
    }
}
```