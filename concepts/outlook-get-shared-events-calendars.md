---
title: Получение событий Outlook из общего или делегированного календаря
description: В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.
author: angelgolfer-ms
ms.openlocfilehash: ef4de6cedeeb9a5688f250652eef0cd6cd5f5183
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413150"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="cc120-104">Получение событий Outlook из общего или делегированного календаря</span><span class="sxs-lookup"><span data-stu-id="cc120-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="cc120-105">В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре.</span><span class="sxs-lookup"><span data-stu-id="cc120-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="cc120-106">Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc120-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="cc120-107">Что касается программного кода, Microsoft Graph поддерживает получение событий из календарей, доступ к которым был предоставлен другими пользователями, а также получение самих общих календарей.</span><span class="sxs-lookup"><span data-stu-id="cc120-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="cc120-108">Поддержка также относится к делегированным календарям.</span><span class="sxs-lookup"><span data-stu-id="cc120-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="cc120-109">Допустим, Григорий поделился с Иваном своим стандартным календарем и предоставил ему доступ на чтение.</span><span class="sxs-lookup"><span data-stu-id="cc120-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="cc120-110">Если Иван войдет в приложение и предоставит делегированные разрешения (Calendars.Read.Shared или Calendars.ReadWrite.Shared), то приложение сможет получать доступ к стандартному календарю Григория и событиям из него, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="cc120-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

> <span data-ttu-id="cc120-111">**Примечание.** Разрешения совместного доступа (Calendars.Read.Shared или Calendars.ReadWrite.Shared) позволяют читать или записывать события в общем или делегированном календаре.</span><span class="sxs-lookup"><span data-stu-id="cc120-111">**Note** The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="cc120-112">Они не поддерживают [подписку на уведомления об изменениях](webhooks.md) элементов в таких папках.</span><span class="sxs-lookup"><span data-stu-id="cc120-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="cc120-113">Чтобы настроить подписки на уведомления об изменениях событий в общем, делегированном или любом другом календаре пользователя или ресурса в клиенте, используйте разрешение приложения Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="cc120-113">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="cc120-114">Получение события из общего календаря</span><span class="sxs-lookup"><span data-stu-id="cc120-114">Get an event in the shared calendar</span></span>

<span data-ttu-id="cc120-115">Можно получить определенное события из общего стандартного календаря Григория:</span><span class="sxs-lookup"><span data-stu-id="cc120-115">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="cc120-116">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [event](/graph/api/resources/event?view=graph-rest-1.0), указанный параметром `{id}`, из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="cc120-116">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="cc120-117">Получение всех событий из общего календаря</span><span class="sxs-lookup"><span data-stu-id="cc120-117">Get all the events in the shared calendar</span></span>

<span data-ttu-id="cc120-118">Получение всех событий из стандартного календаря, которым Григорий поделился с Иваном:</span><span class="sxs-lookup"><span data-stu-id="cc120-118">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="cc120-119">В случае успешного выполнения вы получите отклик HTTP 200 OK и коллекцию экземпляров объекта [event](/graph/api/resources/event?view=graph-rest-1.0) из стандартного календаря Григория.</span><span class="sxs-lookup"><span data-stu-id="cc120-119">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="cc120-120">Получение общего календаря</span><span class="sxs-lookup"><span data-stu-id="cc120-120">Get the shared calendar</span></span>

<span data-ttu-id="cc120-121">Получение стандартного календаря, которым Григорий поделился с Иваном.</span><span class="sxs-lookup"><span data-stu-id="cc120-121">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="cc120-122">В случае успешного выполнения вы получите отклик HTTP 200 OK и экземпляр объекта [calendar](/graph/api/resources/calendar?view=graph-rest-1.0), представляющий стандартный календарь Григория.</span><span class="sxs-lookup"><span data-stu-id="cc120-122">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="cc120-123">Такие же возможности для запросов GET будут доступны, если Григорий делегирует Ивану дополнительные права доступа к своему стандартному календарю или всему почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cc120-123">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="cc120-124">Если Григорий не поделился своим стандартным календарем с Иваном и не делегировал ему свой почтовый ящик, то при указании идентификатора пользователя или имени участника-пользователя Ивана в этих операциях GET будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="cc120-124">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="cc120-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="cc120-125">Next steps</span></span>

<span data-ttu-id="cc120-126">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="cc120-126">Find out more about:</span></span>

- [<span data-ttu-id="cc120-127">Зачем выполнять интеграцию с Календарем Outlook?</span><span class="sxs-lookup"><span data-stu-id="cc120-127">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="cc120-128">[API календаря](/graph/api/resources/calendar?view=graph-rest-1.0) в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="cc120-128">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>