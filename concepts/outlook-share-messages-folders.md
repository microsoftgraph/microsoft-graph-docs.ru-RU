# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Получение сообщений Outlook в общей или делегированной папке

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Outlook позволяет пользователям совместно использовать почтовые папки друг с другом и предоставляет  отдельным папкам доступ для «чтения», «создания», «изменения» или «удаления». Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента и получать доступ к определенным почтовым папкам или ко всему почтовому ящику клиента; этот процесс Outlook также известен под названием «делегирование».

Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок. Поддержка также применяется к папкам, которые были делегированны.

Допустим, Гарт предоставил Джону доступ на чтение своей папки "Входящие". Если Джон войдет в ваше приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получить доступ к почте и папке "Входящие" Гарта, как показано ниже.

## <a name="get-a-message-in-the-shared-folder"></a>Получение сообщения из общей папки

Так вы можете получить определенное сообщение из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](../api-reference/v1.0/resources/message.md), указанный параметром `{id}`, из папки "Входящие" Григория.

## <a name="get-all-messages-in-the-shared-folder"></a>Получение всех сообщений из общей папки

Получение всех сообщений из папки "Входящие" Григория:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](../api-reference/v1.0/resources/message.md) из папки "Входящие" Григория.

## <a name="get-the-shared-folder"></a>Получение общей папки

Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](../api-reference/v1.0/resources/mailfolder.md), представляющий папку "Входящие" Григория.

Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.

Если Гарт не поделился своим календарем с Иваном и не делегировал свой почтовый ящик этому пользователю, указав идентификатор или имя участника-пользователя  Гарта в операциях GET, будет возвращена ошибка. 


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование API почты](../api-reference/v1.0/resources/mail_api_overview.md) и [варианты использования](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) в Microsoft Graph 1.0.