# <a name="share-outlook-message-folders-between-users"></a><span data-ttu-id="83a95-101">Совместный доступ пользователей к папкам сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="83a95-101">Share Outlook message folders between users</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="83a95-102">Пользователи Outlook могут делиться папками и предоставлять права на чтение, создание и изменение отдельных папок или всего почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="83a95-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="83a95-103">В Outlook это также называют делегированием.</span><span class="sxs-lookup"><span data-stu-id="83a95-103">This is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="83a95-104">Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="83a95-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span>

<span data-ttu-id="83a95-105">Допустим, Григорий предоставил Ивану доступ на чтение своей папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="83a95-105">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="83a95-106">Если Иван войдет в приложение и предоставит делегированные разрешения (Mail.Read.Shared или Mail.ReadWrite.Shared), то приложение сможет получать доступ к почте и папке "Входящие" Григория, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="83a95-106">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="83a95-107">Получение сообщения из общей папки</span><span class="sxs-lookup"><span data-stu-id="83a95-107">Get a message in the shared folder</span></span>

<span data-ttu-id="83a95-108">Так вы можете получить определенное сообщение из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="83a95-108">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="83a95-109">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [message](../api-reference/v1.0/resources/message.md), указанный параметром `{id}`, из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="83a95-109">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="83a95-110">Получение всех сообщений из общей папки</span><span class="sxs-lookup"><span data-stu-id="83a95-110">Get all messages in the shared folder</span></span>

<span data-ttu-id="83a95-111">Получение всех сообщений из папки "Входящие" Григория:</span><span class="sxs-lookup"><span data-stu-id="83a95-111">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="83a95-112">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [message](../api-reference/v1.0/resources/message.md) из папки "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="83a95-112">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="83a95-113">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="83a95-113">Get the shared folder</span></span>

<span data-ttu-id="83a95-114">Получение папки ("Входящие"), доступ к которой Григорий предоставил Ивану.</span><span class="sxs-lookup"><span data-stu-id="83a95-114">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="83a95-115">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [mailFolder](../api-reference/v1.0/resources/mailfolder.md), представляющий папку "Входящие" Григория.</span><span class="sxs-lookup"><span data-stu-id="83a95-115">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="83a95-116">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своей папке "Входящие" или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="83a95-116">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="83a95-117">Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="83a95-117">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="83a95-118">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="83a95-118">Next steps</span></span>

<span data-ttu-id="83a95-119">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="83a95-119">Find out more about:</span></span>

- [<span data-ttu-id="83a95-120">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="83a95-120">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="83a95-121">[Использование API почты](../api-reference/v1.0/resources/mail_api_overview.md) и [варианты использования](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) в Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="83a95-121">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>