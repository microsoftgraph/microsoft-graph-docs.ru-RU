# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="a5f07-101">Получение событий Outlook в общем или делегированном календаре</span><span class="sxs-lookup"><span data-stu-id="a5f07-101">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="a5f07-102">В Outlook пользователи могут предоставить общий доступ к календарю другим пользователям и позволить им просматривать или изменять события в календаре.</span><span class="sxs-lookup"><span data-stu-id="a5f07-102">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="a5f07-103">Пользователи также могут предоставлять делегата с  правом действовать от их имени, чтобы получать или отвечать на приглашения на собрания, или создавать или изменять элементы в календаре.</span><span class="sxs-lookup"><span data-stu-id="a5f07-103">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="a5f07-104">Программным способом Microsoft Graph поддерживает получение событий в календарях, общие с другими пользователями, а также получение самих общих о календарей.</span><span class="sxs-lookup"><span data-stu-id="a5f07-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="a5f07-105">Поддержка также применяется к календарям, которые были делегированны.</span><span class="sxs-lookup"><span data-stu-id="a5f07-105">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="a5f07-106">Например, Гарт совместно использует календарь по умолчанию и с Джоном и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="a5f07-106">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="a5f07-107">Если Джон вошел в ваше приложение и предоставил делегированные разрешения (Calendars.Read.Shared or Calendars.ReadWrite.Shared), то ваше приложение сможет получить доступ к календарю и событиям по умолчанию Гарта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="a5f07-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="a5f07-108">Получение событий в общем календаре</span><span class="sxs-lookup"><span data-stu-id="a5f07-108">Get an event in the shared calendar</span></span>

<span data-ttu-id="a5f07-109">Вы сможете получить  определенные события в общем календаре  по умолчанию пользователя Гарта:</span><span class="sxs-lookup"><span data-stu-id="a5f07-109">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="a5f07-110">При успешном завершении, вы получите HTTP 200 OK и экземпляр [события](../api-reference/v1.0/resources/event.md), определяемого `{id}` из календаря по умолчанию Гарта.</span><span class="sxs-lookup"><span data-stu-id="a5f07-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/event.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="a5f07-111">Получение всех событий в общем календаре</span><span class="sxs-lookup"><span data-stu-id="a5f07-111">Get all the events in the shared calendar</span></span>

<span data-ttu-id="a5f07-112">Получение всех событий в календаре по умолчанию, который Гарт совместно использует с Джоном:</span><span class="sxs-lookup"><span data-stu-id="a5f07-112">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="a5f07-113">При успешном завершении, вы получите HTTP 200 OK и коллекцию экземпляров [события](../api-reference/v1.0/resources/event.md) в календаре по умолчанию Гарта.</span><span class="sxs-lookup"><span data-stu-id="a5f07-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/event.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="a5f07-114">Получение общего календаря</span><span class="sxs-lookup"><span data-stu-id="a5f07-114">Get the shared folder</span></span>

<span data-ttu-id="a5f07-115">Получите календаря по умолчанию, который Гарт совместно использует с Джоном.</span><span class="sxs-lookup"><span data-stu-id="a5f07-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="a5f07-116">При успешном завершении, вы получите HTTP 200 OK и экземпляра [календаря](../api-reference/v1.0/resources/calendar.md), который представляется папкой по умолчанию Гарта.</span><span class="sxs-lookup"><span data-stu-id="a5f07-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/calendar.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="a5f07-117">Такие же возможности для запросов GET будут доступны, если Гарт делегирует Джону дополнительные права доступа к своему календарю по умолчанию или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="a5f07-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="a5f07-118">Если Гарт не предоставил доступ к своему календарю по умолчанию и не делегировал свой почтовый ящик Джону, указав идентификатор или имя участника-пользователя  Гарта в операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="a5f07-118">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="a5f07-119">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="a5f07-119">Next steps</span></span>

<span data-ttu-id="a5f07-120">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="a5f07-120">Find out more about:</span></span>

- [<span data-ttu-id="a5f07-121">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="a5f07-121">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="a5f07-122"> [Календарь API](../api-reference/v1.0/resources/calendar.md) в Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="a5f07-122">The [calendar API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1.0.</span></span>