# LIBRARY_MANAGEMENTSYSTEM

Project Title: City Library Digital Management System 
Problem Statement: 
The City Central Library has decided to digitize its operations to make book 
management, membership services, and data tracking more efficient. They 
need a Java-based application to handle book records, member details, and 
transactions using File Handling and the Java Collections Framework. 
The system must be capable of: 
• Adding new books and members. 
COs 
CO1 
• Issuing and returning books. 
• Storing and retrieving data from files for persistence. 
• Using collections to efficiently search, sort, and manage records. 
 Project Objectives: 
• Apply File Handling concepts to store and retrieve library data from 
text and binary files. 
• Implement Java Collections Framework (List, Set, Map, Queue) to 
manage records dynamically. 
• Use Comparable and Comparator for sorting books and members by 
different criteria. 
• Practice Buffered I/O, Character Streams, and Byte Streams for 
efficient file operations. 
• Apply Generics in collections for type-safe data handling. 
 
   
 Learning Outcomes (COs): 
• CO4.1: Use Java’s File Handling API for persistent storage of real-world 
data. 
• CO4.2: Implement the Java Collections Framework for dynamic data 
management. 
• CO4.3: Demonstrate sorting and searching using 
Comparable/Comparator. 
• CO4.4: Integrate I/O operations with collection-based data handling 
for real-world scenarios. 
 
 Project Instructions: 
1. Class Design 
Book Class 
• Attributes: 
o bookId (Integer, unique ID) 
o title (String) 
o author (String) 
o category (String) 
o isIssued (Boolean) 
• Methods: 
o displayBookDetails() – Shows book details. 
o markAsIssued() – Updates isIssued to true. 
o markAsReturned() – Updates isIssued to false. 
 
 Member Class 
• Attributes: 
o memberId (Integer, unique ID) 
o name (String) 
o email (String) 
o issuedBooks (List of book IDs) 
• Methods: 
o displayMemberDetails() 
o addIssuedBook(int bookId) 
o returnIssuedBook(int bookId) 
 
 LibraryManager Class 
• Attributes: 
o Map<Integer, Book> books 
o Map<Integer, Member> members 
• Methods: 
o addBook() – Adds a new book to the collection and saves it to 
file. 
o addMember() – Adds a new member and saves to file. 
o issueBook() – Marks a book as issued and updates both 
book and member records in file. 
o returnBook() – Marks a book as returned. 
o searchBooks() – Search by title, author, or category using 
Collections. 
o sortBooks() – Sort by title/author using 
Comparable/Comparator. 
o loadFromFile() – Loads all data at startup. 
o saveToFile() – Saves all data before exit. 
 
   
 2. File Handling Requirements 
• Use FileReader/FileWriter for text-based data storage. 
• Use BufferedReader/BufferedWriter for faster reading/writing. 
• Use FileInputStream/FileOutputStream for binary storage of 
serialized objects (optional advanced). 
• Ensure files are created if not present. 
• Store books in books.txt and members in members.txt. 
 
 3. Collection Framework Requirements 
• List: Store issued book IDs for each member. 
• Set: Maintain a set of unique categories. 
• Map: Store books and members using IDs as keys. 
• Queue (Optional Advanced): Maintain a waiting list for popular 
books. 
• Comparable: Sort books by title. 
• Comparator: Sort books by author or category. 
 
 4. Implementation Steps 
1. Design Book and Member classes with required fields and methods. 
2. Implement LibraryManager with collections to store data in memory. 
3. Load existing records from files when the application starts. 
4. Implement menu options for all operations 
(add/search/sort/issue/return). 
5. Save updated data to files after each operation. 
 
5. Sample Interaction 
Welcome to City Library Digital Management System 
1. Add Book 
2. Add Member 
3. Issue Book 
4. Return Book 
5. Search Books 
6. Sort Books 
7. Exit 
Enter your choice: 1 
Enter Book Title: Java Programming Mastery Enter Author: 
John Smith 
Enter Category: Programming 
Book added successfully with ID: 101
