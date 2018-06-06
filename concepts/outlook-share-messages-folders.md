# <a name="share-outlook-message-folders-between-users"></a>Совместный доступ пользователей к папкам сообщений Outlook

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Пользователи Outlook могут делиться папками и предоставлять права на чтение, создание и изменение отдельных папок или всего почтового ящика. В Outlook это также называют делегированием.

Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.

Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие". Если Иван войдет в приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.

## <a name="get-a-message-in-the-shared-folder"></a>Получение сообщения из общей папки

Так вы можете получить определенное сообщение из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](../api-reference/v1.0/resources/message.md), указанный параметром `{id}`, из папки "Входящие" Григория.

## <a name="get-all-messages-in-the-shared-folder"></a>Получение всех сообщений из общей папки

Получение всех сообщений из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](../api-reference/v1.0/resources/message.md) из папки "Входящие" Григория.

## <a name="get-the-shared-folder"></a>Получение общей папки

Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](../api-reference/v1.0/resources/mailfolder.md), представляющий папку "Входящие" Григория.

Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.

Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка. 


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование API почты](../api-reference/v1.0/resources/mail_api_overview.md) и [варианты использования](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) в Microsoft Graph 1.0.