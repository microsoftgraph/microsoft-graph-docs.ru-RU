---
title: Получение событий Outlook из общего или делегированного календаря
description: В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092637"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="0798b-104">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="0798b-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="0798b-105">В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="0798b-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="0798b-106">Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.</span><span class="sxs-lookup"><span data-stu-id="0798b-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="0798b-107">Что касается программного кода, Microsoft Graph поддерживает получение событий из календарей, доступ к которым был предоставлен другими пользователями, а также получение самих общих календарей.</span><span class="sxs-lookup"><span data-stu-id="0798b-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="0798b-108">Поддержка также относится к делегированным календарям.</span><span class="sxs-lookup"><span data-stu-id="0798b-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="0798b-109">Допустим, Григорий поделился с Иваном своим стандартным календарем и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="0798b-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="0798b-110">Если Иван войдет в приложение и предоставит делегированные разрешения (Calendars.Read.Shared или Calendars.ReadWrite.Shared), то приложение сможет получать доступ к стандартному календарю Григория и событиям из него, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="0798b-110">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="0798b-111">Получение события из общего календаря</span><span class="sxs-lookup"><span data-stu-id="0798b-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="0798b-112">Можно получить определенное события из общего стандартного календаря Григория:</span><span class="sxs-lookup"><span data-stu-id="0798b-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="0798b-113">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [event](/graph/api/resources/event?view=graph-rest-1.0), указанный параметром `{id}`, из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="0798b-113">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="0798b-114">Получение всех событий из общего календаря</span><span class="sxs-lookup"><span data-stu-id="0798b-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="0798b-115">Получение всех событий из стандартного календаря, которым Григорий поделился с Иваном:</span><span class="sxs-lookup"><span data-stu-id="0798b-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="0798b-116">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [event](/graph/api/resources/event?view=graph-rest-1.0) из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="0798b-116">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="0798b-117">Получение общего календаря</span><span class="sxs-lookup"><span data-stu-id="0798b-117">Get the shared folder</span></span>

<span data-ttu-id="0798b-118">Получение стандартного календаря, которым Григорий поделился с Иваном.</span><span class="sxs-lookup"><span data-stu-id="0798b-118">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="0798b-119">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [calendar](/graph/api/resources/calendar?view=graph-rest-1.0), представляющий стандартный календарь Григория.</span><span class="sxs-lookup"><span data-stu-id="0798b-119">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="0798b-120">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своему стандартному календарю или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="0798b-120">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="0798b-121">Если Григорий не поделился своим стандартным календарем с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Ивана в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="0798b-121">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="0798b-122">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0798b-122">Next steps</span></span>

<span data-ttu-id="0798b-123">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="0798b-123">Find out more about:</span></span>

- [<span data-ttu-id="0798b-124">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="0798b-124">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="0798b-125">[API календаря](/graph/api/resources/calendar?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="0798b-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>