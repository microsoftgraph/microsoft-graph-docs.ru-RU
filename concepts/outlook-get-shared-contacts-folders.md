# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="03b0c-101">Получение контактов Outlook в общей папке</span><span class="sxs-lookup"><span data-stu-id="03b0c-101">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="03b0c-102">Outlook позволяет пользователям совместно использовать почтовые папки друг с другом и предоставляет отдельным папкам доступ для «чтения», «создания», «изменения» или «удаления».</span><span class="sxs-lookup"><span data-stu-id="03b0c-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="03b0c-103">Outlook также позволяет клиенту делегировать другому пользователю действовать от имени клиента и получать доступ к определенным почтовым папкам или ко всему почтовому ящику клиента; этот процесс Outlook также известен под названием «делегирование».</span><span class="sxs-lookup"><span data-stu-id="03b0c-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="03b0c-104">Что касается программного кода, Microsoft Graph поддерживает получение сообщений из почтовых папок, доступ к которым был предоставлен другими пользователями, а также получение самих общих папок.</span><span class="sxs-lookup"><span data-stu-id="03b0c-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="03b0c-105">Поддержка также применяется к папкам в делегированном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="03b0c-105">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="03b0c-106">Допустим, Гарт поделился с Джоном  настраиваемой папкой  контактов и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="03b0c-106">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="03b0c-107">Если Джон войдет в ваше приложение и предоставит делегированные разрешения (Contacts.Read.Shared или Contacts.ReadWrite.Shared), то  ваше приложение сможет получить доступ к контактам в настраиваемой папке контактов Гарта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="03b0c-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="03b0c-108">Получение контакта в общей папке</span><span class="sxs-lookup"><span data-stu-id="03b0c-108">Get a message in the shared folder</span></span>

<span data-ttu-id="03b0c-109">Вы сможете получить конкретный контакт в настраиваемой папке контактов, которую Гарт разделил совместно с Джоном:</span><span class="sxs-lookup"><span data-stu-id="03b0c-109">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="03b0c-110">При успешном завершении, вы получите HTTP 200 OK и экземпляр [contact](../api-reference/v1.0/resources/contact.md), определяемого `{id}` из общей папки контактов Гарта.</span><span class="sxs-lookup"><span data-stu-id="03b0c-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/contact.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="03b0c-111">Получение всех контактов в общей папке</span><span class="sxs-lookup"><span data-stu-id="03b0c-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="03b0c-112">Получение всех контактов в общей папке контактов Гарта:</span><span class="sxs-lookup"><span data-stu-id="03b0c-112">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="03b0c-113">При успешном завершении, вы получите HTTP 200 OK и коллекцию экземпляров [contact](../api-reference/v1.0/resources/contact.md)в общей папке контактов Гарта.</span><span class="sxs-lookup"><span data-stu-id="03b0c-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/contact.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="03b0c-114">Получение общей папки</span><span class="sxs-lookup"><span data-stu-id="03b0c-114">Get the shared folder</span></span>

<span data-ttu-id="03b0c-115">Получение папки контактов, которую Гарт разделил совместно с  Джоном.</span><span class="sxs-lookup"><span data-stu-id="03b0c-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="03b0c-116">При успешном завершении вы получите HTTP 200 OK и экземпляр [contactFolder](../api-reference/v1.0/resources/contactfolder.md), который предоставляется общей папкой контактов Гарта.</span><span class="sxs-lookup"><span data-stu-id="03b0c-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/contactfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="03b0c-117">Те же возможности GET применяются, если Гарт делегировал Джону весь свой почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="03b0c-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="03b0c-118">Если Гарт не поделился своей папкой контактов с Джоном и не делегировал ему свой почтовый ящик, указав идентификатор или имя участника-пользователя Гарта в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="03b0c-118">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="03b0c-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="03b0c-119">Next steps</span></span>

<span data-ttu-id="03b0c-120">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="03b0c-120">Find out more about:</span></span>

- [<span data-ttu-id="03b0c-121">Для чего необходимо выполнять интеграцию с личными контактами Outlook?</span><span class="sxs-lookup"><span data-stu-id="03b0c-121">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="03b0c-122"> [Контакты API](../api-reference/v1.0/resources/contact.md) в Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="03b0c-122">The [contacts API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1.0.</span></span>