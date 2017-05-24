# <a name="traverse-microsoft-graph"></a>Просмотр ресурсов в Microsoft Graph

Помимо чтения и записи данных с помощью API Microsoft Graph, вы можете использовать шаблоны запросов для просмотра ресурсов в Microsoft Graph. Документ метаданных поможет вам разобраться в модели данных ресурсов и отношений в Microsoft Graph.

## <a name="microsoft-graph-api-metadata"></a>Метаданные API Microsoft Graph

Документ метаданных ($metadata) публикуется в корневом каталоге службы. По указанным ниже URL-адресам можно просмотреть сервисный документ для версии 1.0 и бета-версии API Microsoft Graph.

**Метаданные API `v1.0` Microsoft Graph**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Метаданные API `beta` Microsoft Graph**

```
    https://graph.microsoft.com/beta/$metadata
```

Метаданные позволяют разобраться в модели данных Microsoft Graph, в том числе типах объектов, сложных типах и перечислениях, из которых состоят ресурсы, представленные в пакетах запросов и ответов.

С помощью метаданных можно узнать об отношениях между сущностями в Microsoft Graph и создать URL-адреса для перехода между ними.

Имена ресурсов URL-адреса пути, параметры запросов, а также параметры и значения действий указываются без учета регистра. Однако назначаемые значения, идентификаторы объектов и другие значения в кодировке base64 указываются с учетом регистра.

## <a name="view-a-specific-resource-from-a-collection-by-id"></a>Просмотр ресурса из коллекции по идентификатору

Чтобы просмотреть сведения о пользователе, получите коллекцию всех пользователей и используйте HTTPS-запрос GET для поиска пользователя по идентификатору. Для объекта `User` в качестве идентификатора можно использовать свойство `id` или `userPrincipalName`. В следующем примере запроса в качестве идентификатора используется значение `userPrincipalName`. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном выполнении действия будет получен ответ 200 OK, содержащий полезные данные с представлением ресурса user, как показано ниже.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```

## <a name="read-specific-properties-of-a-resource"></a>Чтение определенных свойств ресурса
Чтобы получить только биографические данные пользователя, например предоставленное им описание в разделе _Обо мне_ и набор квалификационных навыков, в предыдущий запрос можно добавить параметр [$select](query_parameters.md), как показано в следующем примере. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются полезные данные и состояние 200 OK, как показано ниже.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
Здесь возвращаются не наборы свойств для объекта `user`, а только базовые свойства `aboutMe`, `displayName` и `skills`.

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>Чтение отдельных свойств ресурсов в коллекции
Вы можете не только просматривать отдельные свойства одного ресурса, но и получить все ее ресурсы только с указанными свойствами, применив к коллекции аналогичный параметр запроса [$select](query_parameters.md). Например, чтобы запросить имена элементов на диске вошедшего пользователя, можно отправить следующий HTTPS-запрос GET.

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются код состояния 200 OK и полезные данные, содержащие только имена общих файлов, как показано в следующем примере.

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>Переход от одного ресурса к другому с помощью отношения
Руководитель состоит в отношении `directReports` со своими подчиненными. Чтобы запросить список подчиненных пользователя, можно использовать приведенный ниже HTTPS-запрос GET для перехода к целевому объекту с помощью отношения. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются полезные данные и состояние 200 OK, как показано ниже.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

Аналогичным образом можно переходить к связанным ресурсам с помощью отношений. Например, отношение `user => messages` позволяет перейти от пользователя Azure Active Directory (AD) к набору сообщений Outlook. В приведенном ниже примере показано, как это сделать в вызове REST API.


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
При успешном ответе возвращаются полезные данные и состояние 200 OK, как показано ниже.


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```
Чтобы просмотреть все отношения для ресурса, откройте метаданные, найдите нужный EntityType и просмотрите все его свойства NavigationProperties.

## <a name="call-functions"></a>Вызов функций
Microsoft Graph также поддерживает _функции_ для выполнения с ресурсами действий, отличных от простых операций CRUD (создание, чтение, обновление и удаление). Они часто имеют форму HTTPS-запросов POST, принимающих аргументы. Например, с помощью указанной ниже функции вошедший пользователь (`me`) может отправить сообщение электронной почты.

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

Вы можете просмотреть все доступные функции в метаданных. Они отображаются как функции или действия.

## <a name="use-the-microsoft-graph-sdks"></a>Использование пакетов SDK Microsoft Graph

Вам нравятся возможности и удобство пакетов SDK? Вы всегда можете вызывать Microsoft Graph с помощью REST API, но мы также предоставляем пакеты SDK для многих популярных платформ. Обзор доступных пакетов SDK см. в разделе [Примеры кода и пакеты SDK](https://graph.microsoft.io/en-us/code-samples-and-sdks).

## <a name="see-also"></a>См. также

- [Использование API Microsoft Graph](use_the_api.md)
- [Получение токенов аутентификации](auth_overview.md)