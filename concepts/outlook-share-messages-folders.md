# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="c9265-101">Получение сообщений Outlook в общей или делегированной папке</span><span class="sxs-lookup"><span data-stu-id="c9265-101">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="c9265-102">Outlook позволяет пользователям совместно использовать почтовые папки друг с другом и предоставляет  отдельным папкам доступ для «чтения», «создания», «изменения» или «удаления».</span><span class="sxs-lookup"><span data-stu-id="c9265-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="c9265-103">Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента и получать доступ к определенным почтовым папкам или ко всему почтовому ящику клиента; этот процесс Outlook также известен под названием «делегирование».</span><span class="sxs-lookup"><span data-stu-id="c9265-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="c9265-104">Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="c9265-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="c9265-105">Поддержка также применяется к папкам, которые были делегированны.</span><span class="sxs-lookup"><span data-stu-id="c9265-105">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="c9265-106">Допустим, Гарт предоставил Джону доступ на чтение своей папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="c9265-106">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="c9265-107">Если Джон войдет в ваше приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получить доступ к почте и папке "Входящие" Гарта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="c9265-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="c9265-108">Получение сообщения из общей папки</span><span class="sxs-lookup"><span data-stu-id="c9265-108">Get a message in the shared folder</span></span>

<span data-ttu-id="c9265-109">Так вы можете получить определенное сообщение из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="c9265-109">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="c9265-110">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](../api-reference/v1.0/resources/message.md), указанный параметром `{id}`, из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="c9265-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="c9265-111">Получение всех сообщений из общей папки</span><span class="sxs-lookup"><span data-stu-id="c9265-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="c9265-112">Получение всех сообщений из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="c9265-112">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="c9265-113">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](../api-reference/v1.0/resources/message.md) из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="c9265-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="c9265-114">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="c9265-114">Get the shared folder</span></span>

<span data-ttu-id="c9265-115">Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.</span><span class="sxs-lookup"><span data-stu-id="c9265-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="c9265-116">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](../api-reference/v1.0/resources/mailfolder.md), представляющий папку "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="c9265-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="c9265-117">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="c9265-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="c9265-118">Если Гарт не поделился своим календарем с Иваном и не делегировал свой почтовый ящик этому пользователю, указав идентификатор или имя участника-пользователя  Гарта в операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="c9265-118">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="c9265-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c9265-119">Next steps</span></span>

<span data-ttu-id="c9265-120">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="c9265-120">Find out more about:</span></span>

- [<span data-ttu-id="c9265-121">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="c9265-121">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="c9265-122">[Использование API почты](../api-reference/v1.0/resources/mail_api_overview.md) и [варианты использования](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="c9265-122">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>