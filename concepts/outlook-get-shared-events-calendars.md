---
title: Получение событий Outlook из общего или делегированного календаря
description: В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.
author: angelgolfer-ms
ms.openlocfilehash: 8ceb6a49b971c5ad01f27b53c0f3cd3cf047865d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346566"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="b9a35-104">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="b9a35-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="b9a35-105">В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="b9a35-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="b9a35-106">Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.</span><span class="sxs-lookup"><span data-stu-id="b9a35-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="b9a35-107">Что касается программного кода, Microsoft Graph поддерживает получение событий из календарей, доступ к которым был предоставлен другими пользователями, а также получение самих общих календарей.</span><span class="sxs-lookup"><span data-stu-id="b9a35-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="b9a35-108">Поддержка также относится к делегированным календарям.</span><span class="sxs-lookup"><span data-stu-id="b9a35-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="b9a35-109">Допустим, Григорий поделился с Иваном своим стандартным календарем и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="b9a35-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="b9a35-110">Если Иван войдет в приложение и предоставит делегированные разрешения (Calendars.Read.Shared или Calendars.ReadWrite.Shared), то приложение сможет получать доступ к стандартному календарю Григория и событиям из него, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b9a35-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="b9a35-111">Получение события из общего календаря</span><span class="sxs-lookup"><span data-stu-id="b9a35-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="b9a35-112">Можно получить определенное события из общего стандартного календаря Григория:</span><span class="sxs-lookup"><span data-stu-id="b9a35-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="b9a35-113">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [event](/graph/api/resources/event?view=graph-rest-1.0), указанный параметром `{id}`, из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="b9a35-113">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="b9a35-114">Получение всех событий из общего календаря</span><span class="sxs-lookup"><span data-stu-id="b9a35-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="b9a35-115">Получение всех событий из стандартного календаря, которым Григорий поделился с Иваном:</span><span class="sxs-lookup"><span data-stu-id="b9a35-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="b9a35-116">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [event](/graph/api/resources/event?view=graph-rest-1.0) из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="b9a35-116">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="b9a35-117">Получение общего календаря</span><span class="sxs-lookup"><span data-stu-id="b9a35-117">Get the shared calendar</span></span>

<span data-ttu-id="b9a35-118">Получение стандартного календаря, которым Григорий поделился с Иваном.</span><span class="sxs-lookup"><span data-stu-id="b9a35-118">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="b9a35-119">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [calendar](/graph/api/resources/calendar?view=graph-rest-1.0), представляющий стандартный календарь Григория.</span><span class="sxs-lookup"><span data-stu-id="b9a35-119">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="b9a35-120">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своему стандартному календарю или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b9a35-120">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="b9a35-121">Если Григорий не поделился своим стандартным календарем с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Ивана в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="b9a35-121">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="b9a35-122">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b9a35-122">Next steps</span></span>

<span data-ttu-id="b9a35-123">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="b9a35-123">Find out more about:</span></span>

- [<span data-ttu-id="b9a35-124">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="b9a35-124">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="b9a35-125">[API календаря](/graph/api/resources/calendar?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="b9a35-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>