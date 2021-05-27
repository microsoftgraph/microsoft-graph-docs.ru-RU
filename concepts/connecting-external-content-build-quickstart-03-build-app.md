<!-- markdownlint-disable MD002 MD025 MD041 -->

На этом этапе будет создаваться консольное приложение .NET Core. После этого создадим новое подключение, зарегистрируйте схему и синхронизируйте элементы.

## <a name="create-a-net-core-console-app"></a>Создание консольного приложения .NET Core

1. Запуск Visual Studio 2019 г. и перейдите в **файл**  >  **New**  >  **Project.**
2. Выберите шаблон **Консоли App (.NET Core)** и выберите **Далее**.
3. Введите **Project** имя : "PartsInventoryConnector" и выберите почтовый ящик для **"Место** решения и проекта в том же каталоге" и выберите **Создать,** как показано на следующем изображении.

![Снимок экрана раздела "Настройка нового проекта"](images/connectors-images/build7.png)

## <a name="add-nuget-packages"></a>Добавление пакетов NuGet

Чтобы добавить NuGet пакеты, сначала щелкните правой кнопкой **мыши Project решение** и выберите Открыть в **терминале**.

![Снимок экрана, показывающий параметр Открыть терминал](images/connectors-images/build8.png)

Затем запустите следующие команды CLI в командной подсказке разработчика.

```dotnetcli
dotnet add package CsvHelper --version 12.1.2
dotnet add package Microsoft.EntityFrameworkCore.Design --version 3.1.3
dotnet add package Microsoft.EntityFrameworkCore.Sqlite --version 3.1.3
dotnet add package Microsoft.Extensions.Configuration.UserSecrets --version 3.1.3
dotnet add package Microsoft.Graph.Beta --version 0.17.0-preview
dotnet add package Microsoft.Identity.Client --version 4.13.0
```

## <a name="add-azure-ad-authentication"></a>Добавление проверки подлинности с помощью Azure AD

Эта проверка подлинности необходима для получения необходимого маркера доступа OAuth для вызова API соединителов.

1. Создайте новый каталог с именем **Authentication** в **каталоге PartsInventoryConnector.**
2. Создайте новый файл в каталоге **проверки** подлинности clientCredentialAuthProvider.cs и поместите следующий код в этот файл:

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Microsoft.Identity.Client;
using System;
using System.Net.Http;
using System.Net.Http.Headers;
using System.Threading.Tasks;

namespace PartsInventoryConnector.Authentication
{
    public class ClientCredentialAuthProvider : IAuthenticationProvider
    {
        private IConfidentialClientApplication _msalClient;
        private int _maxRetries = 3;

        public ClientCredentialAuthProvider(string appId, string tenantId, string secret)
        {
            _msalClient = ConfidentialClientApplicationBuilder
                .Create(appId)
                .WithTenantId(tenantId)
                .WithClientSecret(secret)
                .Build();
        }

        public async Task AuthenticateRequestAsync(HttpRequestMessage request)
        {
            int retryCount = 0;

            do
            {
                try
                {
                    var result = await _msalClient
                        .AcquireTokenForClient(new[] { "https://graph.microsoft.com/.default" })
                        .ExecuteAsync();

                    if (!string.IsNullOrEmpty(result.AccessToken))
                    {
                        request.Headers.Authorization =
                            new AuthenticationHeaderValue("bearer", result.AccessToken);
                        break;
                    }
                }
                catch (MsalServiceException serviceException)
                {
                    if (serviceException.ErrorCode == "temporarily_unavailable")
                    {
                        await Task.Delay(10000);
                    }
                    else
                    {
                        throw serviceException;
                    }
                }
                catch (Exception exception)
                {
                    throw exception;
                }

                retryCount++;
            } while (retryCount < _maxRetries);
        }
    }
}
```

## <a name="add-user-experience"></a>Добавление пользовательского интерфейса

1. Создайте новый каталог в **каталоге PartsInventoryConnector с** именем **Консоль.**
2. Создайте новый файл в **каталоге Консоли** с именем MenuChoice.cs и поместите следующий код в этот файл:

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.

namespace PartsInventoryConnector.Console
{
    public enum MenuChoice
    {
        Invalid = 0,
        CreateConnection,
        RegisterSchema,
        PushAllItems,
        Exit
    }
}
```

## <a name="set-up-data-model"></a>Настройка модели данных

1. Создание нового каталога в **каталоге PartsInventoryConnector с** именем **Models**.
2. Создайте новый файл в **каталоге Models** с именем AppliancePart.cs и поместите в этот файл следующий код:


```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Newtonsoft.Json;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;

namespace PartsInventoryConnector.Models
{
    public class AppliancePart
    {
        [Key]
        public int PartNumber { get; set; }
        public string Name { get; set; }
        public string Description { get; set; }
        public double Price { get; set; }
        public int Inventory { get; set; }
        [JsonProperty("appliances@odata.type")]
        private const string AppliancesODataType = "Collection(String)";
        public List<string> Appliances { get; set; }

        public Properties AsExternalItemProperties()
        {
            var properties = new Properties
            {
                AdditionalData = new Dictionary<string, object>
                {
                    { "partNumber", PartNumber },
                    { "name", Name },
                    { "description", Description },
                    { "price", Price },
                    { "inventory", Inventory },
                    { "appliances@odata.type", "Collection(String)" },
                    { "appliances", Appliances }
                }
            };

            return properties;
        }
    }
}
```



3. Создайте новый файл в **каталоге Models** с именем ApplianceDbContext.cs и поместите следующий код в этот файл:

```c
using Microsoft.Data.Sqlite;
using Microsoft.EntityFrameworkCore;
using Microsoft.EntityFrameworkCore.ChangeTracking;
using Newtonsoft.Json;
using System;
using System.Collections.Generic;
using System.Linq;

namespace PartsInventoryConnector.Models
{
    public class ApplianceDbContext : DbContext
    {
        public DbSet<AppliancePart> Parts { get; set; }

        protected override void OnConfiguring(DbContextOptionsBuilder options)
        {
            options.UseSqlite("Data Source=parts.db");
        }

        protected override void OnModelCreating(ModelBuilder modelBuilder)
        {
            // EF Core can't store lists, so add a converter for the Appliances
            // property to serialize as a JSON string on save to DB
            modelBuilder.Entity<AppliancePart>()
                .Property(ap => ap.Appliances)
                .HasConversion(
                    v => JsonConvert.SerializeObject(v),
                    v => JsonConvert.DeserializeObject<List<string>>(v)
                );

            // Add LastUpdated and IsDeleted shadow properties
            modelBuilder.Entity<AppliancePart>()
                .Property<DateTime>("LastUpdated")
                .HasDefaultValueSql("datetime()")
                .ValueGeneratedOnAddOrUpdate();
            modelBuilder.Entity<AppliancePart>()
                .Property<bool>("IsDeleted")
                .IsRequired()
                .HasDefaultValue(false);

            // Exclude any soft-deleted items (IsDeleted = 1) from
            // the default query sets
            modelBuilder.Entity<AppliancePart>()
                .HasQueryFilter(a => !EF.Property<bool>(a, "IsDeleted"));
        }

        public override int SaveChanges()
        {
            // Prevent deletes of data, instead mark the item as deleted
            // by setting IsDeleted = true.
            foreach(var entry in ChangeTracker.Entries()
              .Where(e => e.State == EntityState.Deleted))
            {
                if (entry.Entity.GetType() == typeof(AppliancePart))
                {
                    SoftDelete(entry);
                }

            }

            return base.SaveChanges();
        }

        private void SoftDelete(EntityEntry entry)
        {
            var partNumber = new SqliteParameter("@partNumber",
                entry.OriginalValues["PartNumber"]);

            Database.ExecuteSqlRaw(
                "UPDATE Parts SET IsDeleted = 1 WHERE PartNumber = @partNumber",
                partNumber);

            entry.State = EntityState.Detached;
        }
    }
}
```

4. Создание нового каталога с именем **Data** в **каталоге PartsInventoryConnector.**
5. Создайте новый файл в **каталоге данных** CsvDataLoader.cs и поместите в этот файл следующий код:

```c
using CsvHelper;
using CsvHelper.Configuration;
using CsvHelper.TypeConversion;
using PartsInventoryConnector.Models;
using System.Collections.Generic;
using System.IO;
using System.Linq;

namespace PartsInventoryConnector.Data
{
    public static class CsvDataLoader
    {
        public static List<AppliancePart> LoadPartsFromCsv(string filePath)
        {
            using (var reader = new StreamReader(filePath))
            using (var csv = new CsvReader(reader))
            {
                csv.Configuration.RegisterClassMap<AppliancePartMap>();
                return new List<AppliancePart>(csv.GetRecords<AppliancePart>());
            }
        }
    }

    public class ApplianceListConverter : DefaultTypeConverter
    {
        public override object ConvertFromString(string text, IReaderRow row, MemberMapData memberMapData)
        {
            var appliances = text.Split(';');
            return new List<string>(appliances);
        }
    }

    public class AppliancePartMap : ClassMap<AppliancePart>
    {
        public AppliancePartMap()
        {
            Map(m => m.PartNumber);
            Map(m => m.Name);
            Map(m => m.Description);
            Map(m => m.Price);
            Map(m => m.Inventory);
            Map(m => m.Appliances).TypeConverter<ApplianceListConverter>();
        }
    }
}
```

## <a name="write-the-microsoft-graph-helper-service"></a>Напишите службу Graph Майкрософт

1. Создайте новый каталог с именем **MicrosoftGraph** в **каталоге PartsInventoryConnector.**
2. Создайте новый файл в **каталоге MicrosoftGraph** с именем CustomSerializer.cs и поместите следующий код в этот файл:

```c
using Microsoft.Graph;
using Newtonsoft.Json;
using Newtonsoft.Json.Converters;
using Newtonsoft.Json.Serialization;
using System;
using System.IO;

namespace PartsInventoryConnector.Graph
{
    // The Microsoft Graph SDK serializes enumerations in camelCase.
    // The Microsoft Graph service currently requires the PropertyType enum
    // to be PascalCase. This will override the Microsoft Graph serialization
    // If the Microsoft Graph service changes to accept camelCase this will no
    // longer be necessary.
    class CustomContractResolver : DefaultContractResolver
    {
        protected override JsonConverter ResolveContractConverter(Type objectType)
        {
            if (typeof(PropertyType).IsAssignableFrom(objectType))
            {
                // This default converter uses PascalCase
                return new StringEnumConverter();
            }
            return base.ResolveContractConverter(objectType);
        }
    }

    // In order to hook up the custom contract resolver for
    // PropertyType, we need to implement a custom serializer to
    // pass to the MicrosoftGraphServiceClient.
    public class CustomSerializer : ISerializer
    {

        private Serializer _microsoftGraphSerializer;
        private JsonSerializerSettings _jsonSerializerSettings;

        public CustomSerializer()
        {
            _microsoftGraphSerializer = new Serializer();

            _jsonSerializerSettings = new JsonSerializerSettings
            {
                ContractResolver = new CustomContractResolver()
            };
        }

        // For deserialize, just pass through to the default
        // Microsoft Graph SDK serializer
        public T DeserializeObject<T>(Stream stream)
        {
            return _microsoftGraphSerializer.DeserializeObject<T>(stream);
        }

        // For deserialize, just pass through to the default
        // Microsoft Graph SDK serializer
        public T DeserializeObject<T>(string inputString)
        {
            return _microsoftGraphSerializer.DeserializeObject<T>(inputString);
        }

        public string SerializeObject(object serializeableObject)
        {
            // If a Schema object is being serialized, do the conversion
            // ourselves
            if (serializeableObject is Schema)
            {
                var foo = JsonConvert.SerializeObject(serializeableObject, _jsonSerializerSettings);
                return foo;
            }

            // Otherwise, just pass through to the default Microsoft Graph SDK serializer
            return _microsoftGraphSerializer.SerializeObject(serializeableObject);
        }
    }
}
```

3. Создайте новый файл в **каталоге Microsoft Graph** MicrosoftGraphHelper.cs и поместите код ниже в этом файле.

Следующий код содержит методы, которые используют **MicrosoftGraphServiceClient** для создания и отправки вызовов в службу Microsoft Graph и обработки ответа.

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Newtonsoft.Json;
using System.Net.Http;
using System.Threading.Tasks;

namespace PartsInventoryConnector.Graph
{
    public class MicrosoftGraphHelper
    {
        private MicrosoftGraphServiceClient _microsoftGraphClient;

        public MicrosoftGraphHelper(IAuthenticationProvider authProvider)
        {
            // Configure a default HttpProvider with our
            // custom serializer to handle the PropertyType serialization
            var serializer = new CustomSerializer();
            var httpProvider = new HttpProvider(serializer);

            // Initialize the Microsoft Graph client
            _microsoftGraphClient = new MicrosoftGraphServiceClient(authProvider, httpProvider);
        }
    }
}
```

## <a name="initialize-the-microsoft-graph-helper-service"></a>Инициализация службы Graph майкрософт

Откройте Program.cs и замените весь контент следующим кодом:

```c
using Microsoft.EntityFrameworkCore;
using Microsoft.Extensions.Configuration;
using Microsoft.Graph;
using PartsInventoryConnector.Authentication;
using PartsInventoryConnector.Console;
using PartsInventoryConnector.Data;
using PartsInventoryConnector.Graph;
using PartsInventoryConnector.Models;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading.Tasks;

namespace PartsInventoryConnector
{
    class Program
    {
        private static MicrosoftGraphHelper _microsoftGraphHelper;

        private static ExternalConnection _currentConnection;

        private static string _tenantId;

        static async Task Main(string[] args)
        {
            try
            {
                // Load configuration from appsettings.json
                var appConfig = LoadAppSettings();
                if (appConfig == null)
                {
                    return;
                }

                // Save tenant ID for setting ACL on items
                _tenantId = appConfig["tenantId"];

                // Initialize the auth provider
                var authProvider = new ClientCredentialAuthProvider(
                    appConfig["appId"],
                    appConfig["tenantId"],
                    appConfig["appSecret"]
                );

                // Check if the database is empty
                using (var db = new ApplianceDbContext())
                {
                    if (db.Parts.IgnoreQueryFilters().Count() <= 0)
                    {
                        ImportCsvToDatabase(db, "ApplianceParts.csv");
                    }
                }

                _microsoftGraphHelper = new MicrosoftGraphHelper(authProvider);

                do
                {
                    var userChoice = DoMenuPrompt();

                    switch (userChoice)
                    {
                        case MenuChoice.CreateConnection:
                            await CreateConnectionAsync();
                            break;
                        case MenuChoice.RegisterSchema:
                            await RegisterSchemaAsync();
                            break;
                        case MenuChoice.PushAllItems:
                            await UpdateItemsFromDatabase();
                            break;
                        case MenuChoice.Exit:
                            // Exit the program
                            return;
                        case MenuChoice.Invalid:
                        default:
                            break;
                    }

                } while (true);
            }
            catch (Exception ex)
            {
                System.Console.WriteLine(ex.Message);
            }
        }

        private static void ImportCsvToDatabase(ApplianceDbContext db, string partsFilePath)
        {
            var parts = CsvDataLoader.LoadPartsFromCsv(partsFilePath);
            db.AddRange(parts);
            db.SaveChanges();
        }

        private static MenuChoice DoMenuPrompt()
        {
            System.Console.WriteLine($"Current connection: {(_currentConnection == null ? "NONE" : _currentConnection.Name)}");
            System.Console.WriteLine("Please choose one of the following options:");

            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.CreateConnection)}. Create a connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.RegisterSchema)}. Register schema for current connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.PushAllItems)}. Push ALL items to current connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.Exit)}. Exit");

            try
            {
                var choice = int.Parse(System.Console.ReadLine());
                return (MenuChoice)choice;
            }
            catch (FormatException)
            {
                return MenuChoice.Invalid;
            }
        }
        private static string PromptForInput(string prompt, bool valueRequired)
        {
            string response = null;

            do
            {
                System.Console.WriteLine($"{prompt}:");
                response = System.Console.ReadLine();
                if (valueRequired && string.IsNullOrEmpty(response))
                {
                    System.Console.WriteLine("You must provide a value");
                }
            } while (valueRequired && string.IsNullOrEmpty(response));

            return response;
        }

        private static IConfigurationRoot LoadAppSettings()
        {
            var appConfig = new ConfigurationBuilder()
                .AddUserSecrets<Program>()
                .Build();

            // Check for required settings
            if (string.IsNullOrEmpty(appConfig["appId"]) ||
                string.IsNullOrEmpty(appConfig["appSecret"]) ||
                string.IsNullOrEmpty(appConfig["tenantId"]))
            {
                return null;
            }

            return appConfig;
        }
    }
}
```

## <a name="create-the-connection"></a>Создание подключения

1. В **Graph** Microsoft откройте файл MicrosoftGraphHelper.cs и добавьте следующий код после метода **конструктора.**

```c
#region Connections

        public async Task<ExternalConnection> CreateConnectionAsync(string id, string name, string description)
        {
            var newConnection = new ExternalConnection
            {
                // Need to set to null, service returns 400
                // if @odata.type property is sent
                ODataType = null,
                Id = id,
                Name = name,
                Description = description
            };

            return await _microsoftGraphClient.External.Connections.Request().AddAsync(newConnection);
        }

#endregion
```

2. Откройте файл Program.cs и добавьте следующий код после **основного** метода:


```c
private static async Task CreateConnectionAsync()
        {
            var connectionId = PromptForInput("Enter a unique ID for the new connection", true);
            var connectionName = PromptForInput("Enter a name for the new connection", true);
            var connectionDescription = PromptForInput("Enter a description for the new connection", false);

            try
            {
                // Create the connection
                _currentConnection = await _microsoftGraphHelper.CreateConnectionAsync(connectionId, connectionName, connectionDescription);
          System.Console.WriteLine("New connection created");
                System.Console.WriteLine(Newtonsoft.Json.JsonConvert.SerializeObject(_currentConnection, Newtonsoft.Json.Formatting.Indented));
            }
            catch (ServiceException serviceException)
            {
                System.Console.WriteLine(serviceException.Message);
                return;
            }
      }
```

## <a name="register-schema"></a>Схема регистрации

1. В **Graph** Microsoft откройте файл MicrosoftGraphHelper.cs и добавьте следующий код после метода **конструктора.**

```c
#region Schema

        public async Task RegisterSchemaAsync(string connectionId, Schema schema)
        {
            // Need access to the HTTP response here since we are doing an
            // async request. The new schema object isn't returned, we need
            // the Location header from the response
            var asyncNewSchemaRequest = _microsoftGraphClient.External.Connections[connectionId].Schema
                .Request()
                .Header("Prefer", "respond-async")
                .GetHttpRequestMessage();

            asyncNewSchemaRequest.Method = HttpMethod.Post;
            asyncNewSchemaRequest.Content = _microsoftGraphClient.HttpProvider.Serializer.SerializeAsJsonContent(schema);

            var response = await _microsoftGraphClient.HttpProvider.SendAsync(asyncNewSchemaRequest);

            if (response.IsSuccessStatusCode)
            {
                // Get the operation ID from the Location header
                var operationId = ExtractOperationId(response.Headers.Location);
                await CheckSchemaStatusAsync(connectionId, operationId);
            }
            else
            {
                throw new ServiceException(
                    new Error
                    {
                        Code = response.StatusCode.ToString(),
                        Message = "Registering schema failed"
                    }
                );
            }
        }

        private string ExtractOperationId(System.Uri uri)
        {
            int numSegments = uri.Segments.Length;
            return uri.Segments[numSegments - 1];
        }

        public async Task CheckSchemaStatusAsync(string connectionId, string operationId)
        {
            do
            {
                var operation = await _microsoftGraphClient.External.Connections[connectionId]
                    .Operations[operationId]
                    .Request()
                    .GetAsync();

                if (operation.Status == ConnectionOperationStatus.Completed)
                {
                    return;
                }
                else if (operation.Status == ConnectionOperationStatus.Failed)
                {
                    throw new ServiceException(
                        new Error
                        {
                            Code = operation.Error.ErrorCode,
                            Message = operation.Error.Message
                        }
                    );
                }

                await Task.Delay(3000);
            } while (true);
        }

#endregion
```

2. Откройте файл Program.cs и добавьте следующий код после **метода Main.**

```c
private static async Task RegisterSchemaAsync()
        {
            if (_currentConnection == null)
            {
                System.Console.WriteLine("No connection selected. Please create a new connection or select an existing connection.");
                return;
            }

            System.Console.WriteLine("Registering schema, this may take a moment...");

            try
            {
                // Register the schema
                var schema = new Schema
                {
                    // Need to set to null, service returns 400
                    // if @odata.type property is sent
                    ODataType = null,
                    BaseType = "microsoft.graph.externalItem",
                    Properties = new List<Property>
                    {
                        new Property { Name = "partNumber", Type = PropertyType.Int64, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "name", Type = PropertyType.String, IsQueryable = true, IsSearchable = true, IsRetrievable = true },
                        new Property { Name = "description", Type = PropertyType.String, IsQueryable = false, IsSearchable = true, IsRetrievable = true },
                        new Property { Name = "price", Type = PropertyType.Double, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "inventory", Type = PropertyType.Int64, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "appliances", Type = PropertyType.StringCollection, IsQueryable = true, IsSearchable = true, IsRetrievable = true }
                    }
                };

                await _microsoftGraphHelper.RegisterSchemaAsync(_currentConnection.Id, schema);
                System.Console.WriteLine("Schema registered");
            }
            catch (ServiceException serviceException)
            {
                System.Console.WriteLine($"{serviceException.StatusCode} error registering schema:");
                System.Console.WriteLine(serviceException.Message);
                return;
            }
        }
```

## <a name="sync-items"></a>Элементы синхронизации

1. В **Graph** Microsoft откройте файл MicrosoftGraphHelper.cs и добавьте следующий код после метода **Конструктора.**

```c
#region PushData   

        public async Task AddOrUpdateItem(string connectionId, ExternalItem item)
        {
            // The SDK's auto-generated request builder uses POST here,
            // which isn't correct. For now, get the HTTP request and change it
            // to PUT manually.
            var putItemRequest = _microsoftGraphClient.External.Connections[connectionId]
                .Items[item.Id].Request().GetHttpRequestMessage();

            putItemRequest.Method = HttpMethod.Put;
            putItemRequest.Content = _microsoftGraphClient.HttpProvider.Serializer.SerializeAsJsonContent(item);

            var response = await _microsoftGraphClient.HttpProvider.SendAsync(putItemRequest);
            if (!response.IsSuccessStatusCode)
            {
                throw new ServiceException(
                    new Error
                    {
                        Code = response.StatusCode.ToString(),
                        Message = "Error indexing item."
                    }
                );
            }
        }

        #endregion
```

2. Откройте файл Program.cs и добавьте следующий код после **метода Main.**

```c
private static async Task UpdateItemsFromDatabase()
        {
            if (_currentConnection == null)
            {
                System.Console.WriteLine("No connection selected. Please create a new connection or select an existing connection.");
                return;
            }

            List<AppliancePart> partsToUpload = null;

            using (var db = new ApplianceDbContext())
            {
                partsToUpload = db.Parts
                    .ToList();
            }

            System.Console.WriteLine($"Processing {partsToUpload.Count()} add/updates");

            foreach (var part in partsToUpload)
            {
                var newItem = new ExternalItem
                {
                    Id = part.PartNumber.ToString(),
                    Content = new ExternalItemContent
                    {
                        // Need to set to null, service returns 400
                        // if @odata.type property is sent
                        ODataType = null,
                        Type = ExternalItemContentType.Text,
                        Value = part.Description
                    },
                    Acl = new List<Acl>
                    {
                        new Acl {
                            AccessType = AccessType.Grant,
                            Type = AclType.Everyone,
                            Value = _tenantId,
                            IdentitySource = "Azure Active Directory"
                        }
                    },
                    Properties = part.AsExternalItemProperties()
                };

                try
                {
                    System.Console.Write($"Uploading part number {part.PartNumber}...");
                    await _microsoftGraphHelper.AddOrUpdateItem(_currentConnection.Id, newItem);
                    System.Console.WriteLine("DONE");
                }
                catch (ServiceException serviceException)
                {
                    System.Console.WriteLine("FAILED");
                    System.Console.WriteLine($"{serviceException.StatusCode} error adding or updating part {part.PartNumber}");
                    System.Console.WriteLine(serviceException.Message);
                }
            }
        }
```
