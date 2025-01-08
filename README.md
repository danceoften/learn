### C# .NET Core Developer
**Durata:** 6 settimane

**Obiettivi del corso:**
- Utilizzo corretto della metodologia di lavoro Agile
- Approccio all'analisi e sviluppo del software tramite i pattern architetturali
- Conoscenza della programmazione ad oggetti con .NET Core con linguaggio C#
- Apprendimento delle metodologie di gestione, archiviazione ed estrazione dei dati tramite SQL

**Argomenti pratici del corso:**
- Applicazioni Console in C#
- Applicazioni Web Restful API ed MVC
- Docker Desktop e containerizzazione
- Prerequisiti di SQL
- Entity Framework Core
- Sicurezza in applicazioni .NET
- Basi di Cloud computing

**Prerequisiti Hardware e Software per PC discenti:**
- **HW:** Vedi [Requisiti di sistema per Visual Studio 2022](https://learn.microsoft.com/en-us/visualstudio/releases/2022/system-requirements#hardware)
- **SW:** Un Azure Pass per ogni discente

**Capacità e conoscenze acquisite al termine del corso:**
- Utilizzo di Visual Studio Code e Visual Studio Community Edition
- Linguaggio C#
- Sviluppo di App, Servizi, API Restful e MVC Web Apps
- TDD (Test Driven Development)
- Design Patterns
- SQL ed Entity Framework Core
- Cloud computing
- Sicurezza in applicazioni .NET

**Programma del corso**

**Week 1**
- **Introduzione**
  - **Introduzione al programma del corso**: Presentazione del corso, degli obiettivi e delle aspettative.
  - **Installazione degli strumenti di sviluppo per la programmazione con .NET, C# e SQL**: Configurazione dell'ambiente di sviluppo con Visual Studio, .NET SDK e SQL Server.
  - **Introduzione a .NET Core**: Panoramica delle caratteristiche principali di .NET Core, come la cross-platform e le performance migliorate.
  - **Il Version Control System Git**: Introduzione a Git per il controllo delle versioni del codice, con esempi di commit, branch e merge.
    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    git branch feature-branch
    git checkout feature-branch
    ```
  - **Installazione Xunit**: Configurazione di Xunit per i test unitari in .NET Core.
    ```xml
    <PackageReference Include="xunit" Version="2.4.1" />
    <PackageReference Include="xunit.runner.visualstudio" Version="2.4.3" />
    ```

- **Metodologia di sviluppo:**
  - **Agile**: Introduzione alla metodologia Agile, con esempi di sprint, backlog e stand-up meetings.
  - **XP**: Pratiche di Extreme Programming, come il pair programming e il refactoring continuo.
  - **DDD**: Domain-Driven Design per modellare il dominio del problema e separare le responsabilità.
  - **DevOps**: Integrazione continua (CI) e distribuzione continua (CD) per automatizzare il ciclo di vita dello sviluppo.

- **Strumenti DevOps**
  - **Git**: Utilizzo di Git per il versioning del codice, con esempi di commit e branching.
  - **Azure DevOps**: Configurazione di Azure DevOps per la gestione del ciclo di vita del software.
  - **Azure Boards**: Utilizzo di Azure Boards per la gestione dei task e delle attività.
  - **Scrum**: Implementazione del framework Scrum per la gestione dei progetti Agile.

- **Sprint**

- **Il linguaggio C#: tipi**
  - **Tipi**: Introduzione ai tipi di dati in C#, come int, string e DateTime.
    ```csharp
    int number = 10;
    string name = "John Doe";
    DateTime date = DateTime.Now;
    ```
  - **Variabili**: Dichiarazione e utilizzo delle variabili in C#.
    ```csharp
    int age = 30;
    ```
  - **Casting**: Conversione di tipi di dati, con esempi di casting esplicito e implicito.
    ```csharp
    double d = 123.45;
    int i = (int)d;
    ```
  - **Tipi di valore e tipi di riferimento (Value Types e Reference Types)**: Differenze tra value types (come int) e reference types (come classi).
    ```csharp
    int valueType = 10; // Value type
    string referenceType = "Hello"; // Reference type
    ```
  - **Tipi di valore Nullable**: Utilizzo di Nullable<T> per gestire valori nulli.
    ```csharp
    int? nullableValue = null;
    ```
  - **Espressioni**: Utilizzo di espressioni lambda e LINQ.
    ```csharp
    var numbers = new List<int> { 1, 2, 3, 4, 5 };
    var evenNumbers = numbers.Where(n => n % 2 == 0);
    ```
  - **Operatori aritmetici e logici (booleani)**: Operazioni aritmetiche e logiche in C#.
    ```csharp
    int sum = 5 + 3;
    bool isTrue = (5 > 3) && (2 < 4);
    ```
  - **Controllo di flusso**: Utilizzo di if, else, switch e loop.
    ```csharp
    if (age > 18)
    {
        Console.WriteLine("Adult");
    }
    else
    {
        Console.WriteLine("Minor");
    }
    ```
  - **Console App in C#**: Creazione di una semplice applicazione console in C#.
    ```csharp
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
    ```

**Week 2**

- **Il linguaggio C#: sintassi**
  - **Costrutti iterativi**: Utilizzo di for, while e foreach per iterare su collezioni.
    ```csharp
    for (int i = 0; i < 10; i++)
    {
        Console.WriteLine(i);
    }
    ```
  - **Arrays**: Dichiarazione e utilizzo di array unidimensionali e multidimensionali.
    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5 };
    ```
  - **Stringhe**: Manipolazione di stringhe con metodi come Substring e Replace.
    ```csharp
    string text = "Hello, World!";
    string substring = text.Substring(0, 5);
    ```
  - **Le collezioni (List, Set, Dictionary)**: Utilizzo di collezioni generiche come List<T>, HashSet<T> e Dictionary<TKey, TValue>.
    ```csharp
    List<int> list = new List<int> { 1, 2, 3 };
    HashSet<int> set = new HashSet<int> { 1, 2, 3 };
    Dictionary<string, int> dict = new Dictionary<string, int> { { "one", 1 }, { "two", 2 } };
    ```
  - **Boxing e Unboxing di tipi di valore**: Conversione tra value types e reference types.
    ```csharp
    int number = 123;
    object obj = number; // Boxing
    int unboxed = (int)obj; // Unboxing
    ```
  - **I tipi generics**: Creazione di classi e metodi generici.
    ```csharp
    public class GenericClass<T>
    {
        public T Value { get; set; }
    }
    ```
  - **Le collezioni generics (System.Collections.Generic)**: Utilizzo di collezioni generiche.
    ```csharp
    List<int> list = new List<int> { 1, 2, 3 };
    ```
  - **IEnumerable e IEnumerator**: Implementazione di interfacce per l'iterazione su collezioni.
    ```csharp
    public class MyCollection : IEnumerable<int>
    {
        private List<int> _list = new List<int> { 1, 2, 3 };

        public IEnumerator<int> GetEnumerator()
        {
            return _list.GetEnumerator();
        }

        IEnumerator IEnumerable.GetEnumerator()
        {
            return GetEnumerator();
        }
    }
    ```
  - **Il costrutto iterativo foreach**: Iterazione su collezioni con foreach.
    ```csharp
    foreach (var item in list)
    {
        Console.WriteLine(item);
    }
    ```

- **Fasi del rilascio**
  - **Build**: Compilazione del codice sorgente in artefatti eseguibili.
    ```bash
    dotnet build
    ```
  - **Deploy**: Distribuzione degli artefatti su ambienti di produzione.
    ```bash
    dotnet publish
    ```
  - **Pipelines**: Configurazione di pipeline CI/CD con Azure DevOps.
    ```yaml
    trigger:
    - main

    pool:
      vmImage: 'ubuntu-latest'

    steps:
    - task: UseDotNet@2
      inputs:
        packageType: 'sdk'
        version: '6.x'
    - script: dotnet build
      displayName: 'Build project'
    ```

- **OOP: incapsulamento, casting, polimorfismo, interfaccia**
  - **La programmazione orientata agli oggetti**: Introduzione ai concetti di OOP.
  - **Classi e oggetti**: Definizione di classi e creazione di oggetti.
    ```csharp
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
    }

    Person person = new Person { Name = "John", Age = 30 };
    ```
  - **I membri di classe (Campi e Metodi)**: Definizione di campi e metodi in una classe.
    ```csharp
    public class Car
    {
        private string _model;
        public void Drive()
        {
            Console.WriteLine("Driving");
        }
    }
    ```
  - **Modificatori di visibilità**: Utilizzo di public, private e protected.
    ```csharp
    public class Animal
    {
        public string Name { get; set; }
        private int Age { get; set; }
        protected void MakeSound()
        {
            Console.WriteLine("Sound");
        }
    }
    ```
  - **I tre pilastri fondamentali della OOP (Incapsulamento, Ereditarietà, Polimorfismo)**: Esempi di incapsulamento, ereditarietà e polimorfismo.
    ```csharp
    public class Animal
    {
        public virtual void MakeSound()
        {
            Console.WriteLine("Sound");
        }
    }

    public class Dog : Animal
    {
        public override void MakeSound()
        {
            Console.WriteLine("Bark");
        }
    }
    ```
  - **I costruttori**: Definizione di costruttori per inizializzare oggetti.
    ```csharp
    public class Person
    {
        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
    ```
  - **Le Proprietà**: Utilizzo di proprietà per accedere ai campi privati.
    ```csharp
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
    }
    ```

- **Gerarchie di Classi ed ereditarietà**
  - **Auto-Implemented Properties**: Utilizzo di proprietà auto-implementate.
    ```csharp
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
    }
    ```
  - **Il modificatore static**: Definizione di membri statici.
    ```csharp
    public class MathUtils
    {
        public static int Add(int a, int b)
        {
            return a + b;
        }
    }
    ```
  - **Il Polimorfismo**: Esempio di polimorfismo con interfacce e classi astratte.
    ```csharp
    public interface IAnimal
    {
        void MakeSound();
    }

    public class Dog : IAnimal
    {
        public void MakeSound()
        {
            Console.WriteLine("Bark");
        }
    }
    ```
  - **Classi astratte e interfacce**: Definizione di classi astratte e interfacce.
    ```csharp
    public abstract class Animal
    {
        public abstract void MakeSound();
    }

    public class Dog : Animal
    {
        public override void MakeSound()
        {
            Console.WriteLine("Bark");
        }
    }
    ```
  - **Classi e interfacce**: Implementazione di interfacce in classi.
    ```csharp
    public interface IAnimal
    {
        void MakeSound();
    }

    public class Dog : IAnimal
    {
        public void MakeSound()
        {
            Console.WriteLine("Bark");
        }
    }
    ```
  - **Generics**: Creazione di classi e metodi generici.
    ```csharp
    public class GenericClass<T>
    {
        public T Value { get; set; }
    }
    ```

**Week 3**

- **Retrospective**

- **Sprint**

- **Uso delle interfacce**
  - **Dependency Injection**: Iniezione di dipendenze tramite interfacce.
    ```csharp
    public interface ILogger
    {
        void Log(string message);
    }

    public class ConsoleLogger : ILogger
    {
        public void Log(string message)
        {
            Console.WriteLine(message);
        }
    }

    public class OrderService
    {
        private readonly ILogger _logger;

        public OrderService(ILogger logger)
        {
            _logger = logger;
        }

        public void ProcessOrder()
        {
            _logger.Log("Order processed");
        }
    }
    ```
  - **Factory Service**: Utilizzo di factory per creare oggetti.
    ```csharp
    public interface IProduct
    {
        void Display();
    }

    public class ProductA : IProduct
    {
        public void Display()
        {
            Console.WriteLine("Product A");
        }
    }

    public class ProductFactory
    {
        public IProduct CreateProduct(string type)
        {
            if (type == "A")
            {
                return new ProductA();
            }
            // Other products
            return null;
        }
    }
    ```

- **Design patterns, DDD, TDD**
  - **S.O.L.I.D.**: Principi di progettazione del software.

- **IO, Serializzazione, attributi**
  - **Streams, IO, File system**: Lettura e scrittura di file con StreamReader e StreamWriter.
    ```csharp
    using (StreamReader reader = new StreamReader("file.txt"))
    {
        string content = reader.ReadToEnd();
        Console.WriteLine(content);
    }

    using (StreamWriter writer = new StreamWriter("file.txt"))
    {
        writer.WriteLine("Hello, World!");
    }
    ```
  - **Serializzazione e Deserializzazione degli oggetti**: Utilizzo di JsonSerializer per serializzare e deserializzare oggetti.
    ```csharp
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
    }

    Person person = new Person { Name = "John", Age = 30 };
    string json = JsonSerializer.Serialize(person);
    Person deserializedPerson = JsonSerializer.Deserialize<Person>(json);
    ```
  - **Attributi**: Utilizzo di attributi personalizzati.
    ```csharp
    [AttributeUsage(AttributeTargets.Class)]
    public class CustomAttribute : Attribute
    {
        public string Description { get; }

        public CustomAttribute(string description)
        {
            Description = description;
        }
    }

    [Custom("This is a custom attribute")]
    public class MyClass
    {
    }
    ```

- **Windows Forms App**
  - **Lo sviluppo desktop con Windows Forms**: Creazione di applicazioni desktop con Windows Forms.
  - **La programmazione orientata agli eventi**: Gestione degli eventi con event handlers.
    ```csharp
    private void button1_Click(object sender, EventArgs e)
    {
        MessageBox.Show("Button clicked");
    }
    ```
  - **Creazione degli Event Handlers**: Definizione di event handlers per gestire gli eventi.
    ```csharp
    this.button1.Click += new System.EventHandler(this.button1_Click);
    ```
  - **Gestione degli input dell’utente**: Gestione degli input utente con controlli come TextBox e Button.
    ```csharp
    private void textBox1_TextChanged(object sender, EventArgs e)
    {
        string input = textBox1.Text;
    }
    ```
  - **Utilizzo di DLL**: Caricamento e utilizzo di librerie DLL.
    ```csharp
    [DllImport("user32.dll")]
    public static extern int MessageBox(IntPtr hWnd, string lpText, string lpCaption, uint uType);
    ```
  - **La direttiva using**: Utilizzo della direttiva using per includere namespace.
    ```csharp
    using System;
    using System.Windows.Forms;
    ```

- **Retrospective**

**Week 4**

- **Sprint**

- **DLL, Eventi, Threading async await, Tasks**
  - **Gli Assembly**: Creazione e utilizzo di assembly.
    ```csharp
    public class MyClass
    {
        public void MyMethod()
        {
            Console.WriteLine("Hello from assembly");
        }
    }
    ```
  - **NuGet Package Manager**: Gestione delle dipendenze con NuGet.
    ```xml
    <PackageReference Include="Newtonsoft.Json" Version="13.0.1" />
    ```
  - **IDisposable**: Implementazione dell'interfaccia IDisposable per la gestione delle risorse.
    ```csharp
    public class MyResource : IDisposable
    {
        public void Dispose()
        {
            // Clean up resources
        }
    }
    ```
  - **La direttiva using all’interno di metodi e proprietà**: Utilizzo della direttiva using per la gestione delle risorse.
    ```csharp
    using (StreamReader reader = new StreamReader("file.txt"))
    {
        string content = reader.ReadToEnd();
    }
    ```
  - **Il Multithreading**: Creazione di thread per eseguire operazioni in parallelo.
    ```csharp
    Thread thread = new Thread(new ThreadStart(MyMethod));
    thread.Start();
    ```
  - **La classe Task**: Utilizzo della classe Task per eseguire operazioni asincrone.
    ```csharp
    Task.Run(() => MyMethod());
    ```
  - **Il costrutto lock**: Utilizzo del costrutto lock per la sincronizzazione dei thread.
    ```csharp
    private readonly object _lock = new object();

    public void MyMethod()
    {
        lock (_lock)
        {
            // Critical section
        }
    }
    ```
  - **Il modello di programmazione asincrono**: Utilizzo di async e await per la programmazione asincrona.
    ```csharp
    public async Task MyAsyncMethod()
    {
        await Task.Delay(1000);
        Console.WriteLine("Async method completed");
    }
    ```

- **Dependency Injection, Logging, Xunit**
  - **Dependency Injection**: Iniezione di dipendenze con il framework di DI di .NET Core.
    ```csharp
    public interface ILogger
    {
        void Log(string message);
    }

    public class ConsoleLogger : ILogger
    {
        public void Log(string message)
        {
            Console.WriteLine(message);
        }
    }

    public class OrderService
    {
        private readonly ILogger _logger;

        public OrderService(ILogger logger)
        {
            _logger = logger;
        }

        public void ProcessOrder()
        {
            _logger.Log("Order processed");
        }
    }
    ```
  - **Logging**: Utilizzo di ILogger per il logging delle applicazioni.
    ```csharp
    public class OrderService
    {
        private readonly ILogger<OrderService> _logger;

        public OrderService(ILogger<OrderService> logger)
        {
            _logger = logger;
        }

        public void ProcessOrder()
        {
            _logger.LogInformation("Order processed");
        }
    }
    ```
  - **Xunit**: Creazione di test unitari con Xunit.
    ```csharp
    public class OrderServiceTests
    {
        [Fact]
        public void ProcessOrder_ShouldLogMessage()
        {
            // Arrange
            var loggerMock = new Mock<ILogger<OrderService>>();
            var orderService = new OrderService(loggerMock.Object);

            // Act
            orderService.ProcessOrder();

            // Assert
            loggerMock.Verify(x => x.Log(It.IsAny<LogLevel>(), It.IsAny<EventId>(), It.IsAny<object>(), It.IsAny<Exception>(), It.IsAny<Func<object, Exception, string>>()), Times.Once);
        }
    }
    ```

- **Database SQL e NoSQL, JSON, CSV**
  - **I Database**: Introduzione ai database relazionali e NoSQL.
  - **I DBMS**: Utilizzo di sistemi di gestione dei database come SQL Server e MongoDB.
  - **Progettazione Concettuale**: Progettazione del modello concettuale del database.
  - **Progettazione Logica**: Progettazione del modello logico del database.
  - **Progettazione Fisica (Implementazione della base dati per uno specifico DBMS)**: Implementazione del database in un DBMS specifico.
  - **Relazioni, Chiavi interne ed esterne**: Definizione di relazioni e chiavi nel database.
  - **La normalizzazione e vincoli di integrità**: Normalizzazione del database e definizione di vincoli di integrità.
  - **Installazione, connessione e creazione di un DB con il DBMS SQL Server**: Configurazione di SQL Server e creazione di un database.
    ```sql
    CREATE DATABASE MyDatabase;
    ```
  - **Il linguaggio SQL**: Esecuzione di query SQL per la gestione dei dati.
    ```sql
    SELECT * FROM Users;
    ```
  - **Operatori logici**: Utilizzo di operatori logici nelle query SQL.
    ```sql
    SELECT * FROM Users WHERE Age > 18 AND Country = 'USA';
    ```
  - **La clausola di ordinamento ORDER BY**: Ordinamento dei risultati delle query con ORDER BY.
    ```sql
    SELECT * FROM Users ORDER BY Age DESC;
    ```
  - **La clausola JOIN**: Utilizzo di JOIN per combinare tabelle.
    ```sql
    SELECT Users.Name, Orders.OrderDate
    FROM Users
    INNER JOIN Orders ON Users.Id = Orders.UserId;
    ```
  - **La clausola di raggruppamento GROUP BY**: Raggruppamento dei risultati delle query con GROUP BY.
    ```sql
    SELECT Country, COUNT(*)
    FROM Users
    GROUP BY Country;
    ```

- **ADO.NET**
  - **Operazioni CRUD con ADO.NET**: Esecuzione di operazioni CRUD (Create, Read, Update, Delete) con ADO.NET.
    ```csharp
    using (SqlConnection connection = new SqlConnection(connectionString))
    {
        connection.Open();
        string query = "INSERT INTO Users (Name, Age) VALUES (@Name, @Age)";
        using (SqlCommand command = new SqlCommand(query, connection))
        {
            command.Parameters.AddWithValue("@Name", "John");
            command.Parameters.AddWithValue("@Age", 30);
            command.ExecuteNonQuery();
        }
    }
    ```
  - **Providers di ADO.NET**: Utilizzo di provider di dati ADO.NET.
    ```csharp
    using (SqlConnection connection = new SqlConnection(connectionString))
    {
        connection.Open();
        // Use the connection
    }
    ```
  - **Il Repository Pattern (o DAO)**: Implementazione del pattern Repository per l'accesso ai dati.
    ```csharp
    public interface IUserRepository
    {
        Task<User> GetUserByIdAsync(int id);
        Task AddUserAsync(User user);
        Task UpdateUserAsync(User user);
        Task DeleteUserAsync(int id);
    }

    public class UserRepository : IUserRepository
    {
        private readonly string _connectionString;

        public UserRepository(string connectionString)
        {
            _connectionString = connectionString;
        }

        public async Task<User> GetUserByIdAsync(int id)
        {
            using (SqlConnection connection = new SqlConnection(_connectionString))
            {
                await connection.OpenAsync();
                string query = "SELECT * FROM Users WHERE Id = @Id";
                using (SqlCommand command = new SqlCommand(query, connection))
                {
                    command.Parameters.AddWithValue("@Id", id);
                    using (SqlDataReader reader = await command.ExecuteReaderAsync())
                    {
                        if (await reader.ReadAsync())
                        {
                            return new User
                            {
                                Id = reader.GetInt32(reader.GetOrdinal("Id")),
                                Name = reader.GetString(reader.GetOrdinal("Name")),
                                Age = reader.GetInt32(reader.GetOrdinal("Age"))
                            };
                        }
                    }
                }
            }
            return null;
        }

        public async Task AddUserAsync(User user)
        {
            using (SqlConnection connection = new SqlConnection(_connectionString))
            {
                await connection.OpenAsync();
                string query = "INSERT INTO Users (Name, Age) VALUES (@Name, @Age)";
                using (SqlCommand command = new SqlCommand(query, connection))
                {
                    command.Parameters.AddWithValue("@Name", user.Name);
                    command.Parameters.AddWithValue("@Age", user.Age);
                    await command.ExecuteNonQueryAsync();
                }
            }
        }

        public async Task UpdateUserAsync(User user)
        {
            using (SqlConnection connection = new SqlConnection(_connectionString))
            {
                await connection.OpenAsync();
                string query = "UPDATE Users SET Name = @Name, Age = @Age WHERE Id = @Id";
                using (SqlCommand command = new SqlCommand(query, connection))
                {
                    command.Parameters.AddWithValue("@Name", user.Name);
                    command.Parameters.AddWithValue("@Age", user.Age);
                    command.Parameters.AddWithValue("@Id", user.Id);
                    await command.ExecuteNonQueryAsync();
                }
            }
        }

        public async Task DeleteUserAsync(int id)
        {
            using (SqlConnection connection = new SqlConnection(_connectionString))
            {
                await connection.OpenAsync();
                string query = "DELETE FROM Users WHERE Id = @Id";
                using (SqlCommand command = new SqlCommand(query, connection))
                {
                    command.Parameters.AddWithValue("@Id", id);
                    await command.ExecuteNonQueryAsync();
                }
            }
        }
    }
    ```
  - **Object Relational Mapping**: Mappatura di oggetti a tabelle di database.

- **Entity Framework Core, LINQ**
  - **Entity Framework Core**: Introduzione a Entity Framework Core per l'accesso ai dati.
  - **Le entità**: Definizione di entità per rappresentare le tabelle del database.
    ```csharp
    public class User
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
    ```
  - **La classe DbContext e i DbSet**: Utilizzo di DbContext e DbSet per gestire le entità.
    ```csharp
    public class AppDbContext : DbContext
    {
        public DbSet<User> Users { get; set; }

        protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
        {
            optionsBuilder.UseSqlServer("YourConnectionString");
        }
    }
    ```
  - **Approccio Code First**: Creazione del database a partire dal codice.
    ```csharp
    public class AppDbContext : DbContext
    {
        public DbSet<User> Users { get; set; }

        protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
        {
            optionsBuilder.UseSqlServer("YourConnectionString");
        }
    }
    ```
  - **Mapping mediante attributi**: Mappatura delle entità con attributi.
    ```csharp
    [Table("Users")]
    public class User
    {
        [Key]
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
    ```
  - **Mapping mediante fluent API**: Mappatura delle entità con la fluent API.
    ```csharp
    public class AppDbContext : DbContext
    {
        public DbSet<User> Users { get; set; }

        protected override void OnModelCreating(ModelBuilder modelBuilder)
        {
            modelBuilder.Entity<User>()
                .ToTable("Users")
                .HasKey(u => u.Id);
        }
    }
    ```
  - **Approccio Database First**: Creazione del codice a partire dal database esistente.
    ```bash
    Scaffold-DbContext "YourConnectionString" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models
    ```
  - **Ciclo di vita delle Entità (Entity State)**: Gestione dello stato delle entità.
    ```csharp
    var user = new User { Name = "John", Age = 30 };
    context.Users.Add(user);
    context.SaveChanges();
    ```
  - **Interrogare, aggiungere, modificare ed eliminare gli elementi di un DbSet**: Esecuzione di operazioni CRUD con Entity Framework Core.
    ```csharp
    var user = context.Users.Find(1);
    user.Name = "Jane";
    context.SaveChanges();
    ```
  - **Lazy Loading ed Eager Loading delle entità correlate**: Caricamento delle entità correlate con lazy loading e eager loading.
    ```csharp
    var user = context.Users.Include(u => u.Orders).FirstOrDefault(u => u.Id == 1);
    ```
  - **Entity Framework Core e LINQ**: Esecuzione di query LINQ con Entity Framework Core.
    ```csharp
    var users = context.Users.Where(u => u.Age > 18).ToList();
    ```
  - **L’interfaccia IQueryable**: Utilizzo di IQueryable per eseguire query LINQ.
    ```csharp
    IQueryable<User> query = context.Users.Where(u => u.Age > 18);
    ```
  - **LINQ providers**: Utilizzo di provider LINQ per eseguire query.
    ```csharp
    var users = context.Users.Where(u => u.Age > 18).ToList();
    ```
  - **La deferred execution**: Esecuzione differita delle query LINQ.
    ```csharp
    IQueryable<User> query = context.Users.Where(u => u.Age > 18);
    var users = query.ToList(); // Query is executed here
    ```

- **Retrospective**

**Week 5**

- **Sprint**

- **Protocolli di rete**
  - **Il protocollo HTTPS**: Utilizzo del protocollo HTTPS per la comunicazione sicura.
  - **Protocollo FTP**: Utilizzo del protocollo FTP per il trasferimento di file.
  - **Web Server**: Configurazione di web server come IIS e Apache.

- **Web Apps ed HTML5, JSON, TypeScript**
  - **Panoramica sullo sviluppo frontend per il web**: Introduzione allo sviluppo frontend.
  - **Lo stack HTML/CSS/JS**: Utilizzo di HTML, CSS e JavaScript per lo sviluppo web.
  - **Il framework Bootstrap**: Utilizzo di Bootstrap per il design responsivo.
  - **Il linguaggio TypeScript**: Utilizzo di TypeScript per lo sviluppo di applicazioni web.
    ```typescript
    class Person {
        name: string;
        age: number;

        constructor(name: string, age: number) {
            this.name = name;
            this.age = age;
        }

        greet() {
            console.log(`Hello, ${this.name}`);
        }
    }

    let person = new Person("John", 30);
    person.greet();
    ```
  - **Esercitazioni sullo sviluppo frontend**: Esercitazioni pratiche sullo sviluppo frontend.
  - **Panoramica dello sviluppo web**: Introduzione allo sviluppo web.
  - **Il Web Server IIS (Internet Information Server)**: Configurazione di IIS per ospitare applicazioni web.
  - **Il processo di Deploy**: Distribuzione delle applicazioni web su server di produzione.

- **API Restful, Minimal API**
  - **Servizi ed API**: Introduzione ai servizi web e alle API.
  - **Sviluppo di Web Services con ASP.NET Core Web API**: Creazione di API RESTful con ASP.NET Core.
  - **L’architettura REST**: Introduzione all'architettura REST.
  - **I Verbi HTTP**: Utilizzo dei verbi HTTP (GET, POST, PUT, DELETE) per le operazioni CRUD.
  - **Le risorse**: Definizione delle risorse esposte dall'API.

  **Esempio di codice per API RESTful:**
  ```csharp
  [ApiController]
  [Route("api/[controller]")]
  public class ProductsController : ControllerBase
  {
      private readonly IProductService _productService;

      public ProductsController(IProductService productService)
      {
          _productService = productService;
      }

      [HttpGet]
      public async Task<ActionResult<IEnumerable<Product>>> GetProducts()
      {
          var products = await _productService.GetAllProductsAsync();
          return Ok(products);
      }

      [HttpGet("{id}")]
      public async Task<ActionResult<Product>> GetProduct(int id)
      {
          var product = await _productService.GetProductByIdAsync(id);
          if (product == null)
          {
              return NotFound();
          }
          return Ok(product);
      }

      [HttpPost]
      public async Task<ActionResult<Product>> CreateProduct(Product product)
      {
          await _productService.AddProductAsync(product);
          return CreatedAtAction(nameof(GetProduct), new { id = product.Id }, product);
      }

      [HttpPut("{id}")]
      public async Task<IActionResult> UpdateProduct(int id, Product product)
      {
          if (id != product.Id)
          {
              return BadRequest();
          }
          await _productService.UpdateProductAsync(product);
          return NoContent();
      }

      [HttpDelete("{id}")]
      public async Task<IActionResult> DeleteProduct(int id)
      {
          await _productService.DeleteProductAsync(id);
          return NoContent();
      }
  }
  ```

Certamente! Ecco una versione dettagliata delle sezioni richieste, con casi d'uso ed esempi di codice.

---

### App MVC ed API

**Sviluppo di Web Apps con ASP.NET Core MVC**: Creazione di applicazioni web con ASP.NET Core MVC.
- **Caso d'uso**: Creazione di un'applicazione web per la gestione di una biblioteca, dove gli utenti possono cercare, aggiungere e rimuovere libri.
  ```csharp
  public class Startup
  {
      public void ConfigureServices(IServiceCollection services)
      {
          services.AddControllersWithViews();
      }

      public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
      {
          if (env.IsDevelopment())
          {
              app.UseDeveloperExceptionPage();
          }
          else
          {
              app.UseExceptionHandler("/Home/Error");
              app.UseHsts();
          }
          app.UseHttpsRedirection();
          app.UseStaticFiles();

          app.UseRouting();

          app.UseAuthorization();

          app.UseEndpoints(endpoints =>
          {
              endpoints.MapControllerRoute(
                  name: "default",
                  pattern: "{controller=Home}/{action=Index}/{id?}");
          });
      }
  }
  ```

**Il design pattern MVC**: Introduzione al pattern Model-View-Controller.
- **Caso d'uso**: Separazione delle responsabilità in un'applicazione web per la gestione di un blog, dove il modello gestisce i dati, la vista gestisce l'interfaccia utente e il controller gestisce la logica di business.
  ```csharp
  // Model
  public class BlogPost
  {
      public int Id { get; set; }
      public string Title { get; set; }
      public string Content { get; set; }
      public DateTime CreatedDate { get; set; }
  }

  // View (Razor Page)
  @model IEnumerable<BlogPost>
  @foreach (var post in Model)
  {
      <div>
          <h2>@post.Title</h2>
          <p>@post.Content</p>
          <p>@post.CreatedDate</p>
      </div>
  }

  // Controller
  public class BlogController : Controller
  {
      private readonly IBlogService _blogService;

      public BlogController(IBlogService blogService)
      {
          _blogService = blogService;
      }

      public IActionResult Index()
      {
          var posts = _blogService.GetAllPosts();
          return View(posts);
      }
  }
  ```

**Pagine Razor (.cshtml)**: Creazione di pagine Razor per le viste.
- **Caso d'uso**: Creazione di una pagina Razor per visualizzare una lista di prodotti in un negozio online.
  ```csharp
  @model IEnumerable<Product>
  @foreach (var product in Model)
  {
      <div>
          <h2>@product.Name</h2>
          <p>@product.Description</p>
          <p>Price: @product.Price</p>
      </div>
  }
  ```

**Action Methods**: Definizione di action methods nei controller.
- **Caso d'uso**: Definizione di action methods per gestire le operazioni CRUD (Create, Read, Update, Delete) su una lista di contatti.
  ```csharp
  public class ContactsController : Controller
  {
      private readonly IContactService _contactService;

      public ContactsController(IContactService contactService)
      {
          _contactService = contactService;
      }

      public IActionResult Index()
      {
          var contacts = _contactService.GetAllContacts();
          return View(contacts);
      }

      public IActionResult Create()
      {
          return View();
      }

      [HttpPost]
      public IActionResult Create(Contact contact)
      {
          if (ModelState.IsValid)
          {
              _contactService.AddContact(contact);
              return RedirectToAction("Index");
          }
          return View(contact);
      }

      public IActionResult Edit(int id)
      {
          var contact = _contactService.GetContactById(id);
          if (contact == null)
          {
              return NotFound();
          }
          return View(contact);
      }

      [HttpPost]
      public IActionResult Edit(int id, Contact contact)
      {
          if (id != contact.Id)
          {
              return NotFound();
          }

          if (ModelState.IsValid)
          {
              _contactService.UpdateContact(contact);
              return RedirectToAction("Index");
          }
          return View(contact);
      }

      public IActionResult Delete(int id)
      {
          var contact = _contactService.GetContactById(id);
          if (contact == null)
          {
              return NotFound();
          }
          return View(contact);
      }

      [HttpPost, ActionName("Delete")]
      public IActionResult DeleteConfirmed(int id)
      {
          _contactService.DeleteContact(id);
          return RedirectToAction("Index");
      }
  }
  ```

**Routing**: Configurazione del routing per le applicazioni web.
- **Caso d'uso**: Configurazione del routing per un'applicazione web di e-commerce, dove le URL sono mappate a specifici controller e action methods.
  ```csharp
  public class Startup
  {
      public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
      {
          app.UseRouting();

          app.UseEndpoints(endpoints =>
          {
              endpoints.MapControllerRoute(
                  name: "default",
                  pattern: "{controller=Home}/{action=Index}/{id?}");

              endpoints.MapControllerRoute(
                  name: "products",
                  pattern: "products/{category}/{id?}",
                  defaults: new { controller = "Products", action = "Index" });
          });
      }
  }
  ```

**Validazione del model**: Validazione dei dati del modello.
- **Caso d'uso**: Validazione dei dati di un modulo di registrazione utente per garantire che tutti i campi obbligatori siano compilati e che le password corrispondano.
  ```csharp
  public class RegisterViewModel
  {
      [Required]
      [EmailAddress]
      public string Email { get; set; }

      [Required]
      [MinLength(6)]
      public string Password { get; set; }

      [Required]
      [Compare("Password")]
      public string ConfirmPassword { get; set; }
  }

  public class AccountController : Controller
  {
      [HttpGet]
      public IActionResult Register()
      {
          return View();
      }

      [HttpPost]
      public IActionResult Register(RegisterViewModel model)
      {
          if (ModelState.IsValid)
          {
              // Logica per registrare l'utente
              return RedirectToAction("Index", "Home");
          }
          return View(model);
      }
  }
  ```

**Attributi di validazione**: Utilizzo di attributi di validazione per i modelli.
- **Caso d'uso**: Utilizzo di attributi di validazione per garantire che i dati di un modulo di contatto siano validi prima di inviarli.
  ```csharp
  public class ContactViewModel
  {
      [Required]
      [StringLength(100, ErrorMessage = "The {0} value cannot exceed {1} characters.")]
      public string Name { get; set; }

      [Required]
      [EmailAddress]
      public string Email { get; set; }

      [Required]
      [Phone]
      public string PhoneNumber { get; set; }

      [Required]
      [StringLength(500, ErrorMessage = "The {0} value cannot exceed {1} characters.")]
      public string Message { get; set; }
  }

  public class ContactController : Controller
  {
      [HttpGet]
      public IActionResult Index()
      {
          return View();
      }

      [HttpPost]
      public IActionResult Index(ContactViewModel model)
      {
          if (ModelState.IsValid)
          {
              // Logica per inviare il messaggio di contatto
              return RedirectToAction("Success");
          }
          return View(model);
      }

      public IActionResult Success()
      {
          return View();
      }
  }
  ```

**Sicurezza in applicazioni ASP.NET Core**: Implementazione di misure di sicurezza per proteggere le applicazioni web.
- **Caso d'uso**: Implementazione dell'autenticazione e autorizzazione per un'applicazione web di gestione delle risorse umane, dove solo gli utenti autorizzati possono accedere a determinate funzionalità.
  ```csharp
  public class Startup
  {
      public void ConfigureServices(IServiceCollection services)
      {
          services.AddControllersWithViews();
          services.AddAuthentication(CookieAuthenticationDefaults.AuthenticationScheme)
              .AddCookie(options =>
              {
                  options.LoginPath = "/Account/Login";
              });
          services.AddAuthorization(options =>
          {
              options.AddPolicy("AdminPolicy", policy => policy.RequireRole("Admin"));
          });
      }

      public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
      {
          app.UseRouting();

          app.UseAuthentication();
          app.UseAuthorization();

          app.UseEndpoints(endpoints =>
          {
              endpoints.MapControllerRoute(
                  name: "default",
                  pattern: "{controller=Home}/{action=Index}/{id?}");
          });
      }
  }

  public class AccountController : Controller
  {
      [HttpGet]
      public IActionResult Login()
      {
          return View();
      }

      [HttpPost]
      public async Task<IActionResult> Login(LoginViewModel model)
      {
          if (ModelState.IsValid)
          {
              // Logica per autenticare l'utente
              var claims = new List<Claim>
              {
                  new Claim(ClaimTypes.Name, model.Username),
                  new Claim(ClaimTypes.Role, "Admin")
              };
              var claimsIdentity = new ClaimsIdentity(claims, CookieAuthenticationDefaults.AuthenticationScheme);
              await HttpContext.SignInAsync(CookieAuthenticationDefaults.AuthenticationScheme, new ClaimsPrincipal(claimsIdentity));
              return RedirectToAction("Index", "Home");
          }
          return View(model);
      }

      [Authorize(Policy = "AdminPolicy")]
      public IActionResult Admin()
      {
          return View();
      }
  }
  ```

Spero che queste spiegazioni dettagliate e gli esempi di codice ti siano utili! Se hai bisogno di ulteriori chiarimenti o modifiche, fammi sapere.


- **Retrospective**

**Week 6**

- **Sprint**

- **Azure e RBAC**

- **Containers**

- **Shell vs Portal**

- **Sicurezza in CLOUD, configurazione, vault**

- **Retrospective**

- **Terminazione progetto e rilascio**

### Esempi specifici per ciascuno dei principi SOLID

1. **Single Responsibility Principle (SRP)**:
   - **Esempio**: Una classe `OrderProcessor` dovrebbe avere una sola responsabilità, come elaborare gli ordini, e non dovrebbe gestire anche la notifica degli utenti.
   ```csharp
   public class OrderProcessor
   {
       public void ProcessOrder(Order order)
       {
           // Logica per elaborare l'ordine
       }
   }

   public class NotificationService
   {
       public void NotifyUser(User user, string message)
       {
           // Logica per notificare l'utente
       }
   }
   ```

2. **Open/Closed Principle (OCP)**:
   - **Esempio**: Una classe dovrebbe essere aperta per l'estensione ma chiusa per la modifica. Utilizzo di interfacce per estendere il comportamento.
   ```csharp
   public interface IDiscountStrategy
   {
       decimal ApplyDiscount(decimal amount);
   }

   public class FixedDiscount : IDiscountStrategy
   {
       public decimal ApplyDiscount(decimal amount)
       {
           return amount * 0.9m; // 10% di sconto
       }
   }

   public class Order
   {
       private readonly IDiscountStrategy _discountStrategy;

       public Order(IDiscountStrategy discountStrategy)
       {
           _discountStrategy = discountStrategy;
       }

       public decimal CalculateTotal(decimal amount)
       {
           return _discountStrategy.ApplyDiscount(amount);
       }
   }
   ```

3. **Liskov Substitution Principle (LSP)**:
   - **Esempio**: Le sottoclassi devono essere sostituibili con le loro classi base senza alterare il comportamento del programma.
   ```csharp
   public class Bird
   {
       public virtual void Fly()
       {
           Console.WriteLine("Flying");
       }
   }

   public class Sparrow : Bird
   {
       public override void Fly()
       {
           Console.WriteLine("Sparrow is flying");
       }
   }

   public class Ostrich : Bird
   {
       public override void Fly()
       {
           throw new NotSupportedException("Ostriches can't fly");
       }
   }
   ```

4. **Interface Segregation Principle (ISP)**:
   - **Esempio**: Le interfacce dovrebbero essere specifiche per il client. Non forzare i client a implementare metodi che non usano.
   ```csharp
   public interface IWorker
   {
       void Work();
   }

   public interface IEater
   {
       void Eat();
   }

   public class Worker : IWorker, IEater
   {
       public void Work()
       {
           // Logica per lavorare
       }

       public void Eat()
       {
           // Logica per mangiare
       }
   }

   public class Robot : IWorker
   {
       public void Work()
       {
           // Logica per lavorare
       }
   }
   ```

5. **Dependency Inversion Principle (DIP)**:
   - **Esempio**: Dipendere dalle astrazioni, non dalle implementazioni concrete.
   ```csharp
   public interface ILogger
   {
       void Log(string message);
   }

   public class ConsoleLogger : ILogger
   {
       public void Log(string message)
       {
           Console.WriteLine(message);
       }
   }

   public class FileLogger : ILogger
   {
       public void Log(string message)
       {
           // Logica per scrivere su file
       }
   }

   public class OrderService
   {
       private readonly ILogger _logger;

       public OrderService(ILogger logger)
       {
           _logger = logger;
       }

       public void ProcessOrder()
       {
           // Logica per elaborare l'ordine
           _logger.Log("Order processed");
       }
   }
  ```
