---
title: Получение неизменяемых идентификаторов для ресурсов Outlook
description: 'Элементы Outlook (сообщения, события, контакты, задачи) ведут себя довольно интересно, и вы этого либо никогда не замечали, либо это вызывало серьезные затруднения: их идентификаторы изменяются. Это происходит нечасто (только при перемещении элемента), но может привести к серьезным проблемам для приложений, сохраняющих идентификаторы в автономном режиме для дальнейшего использования. Неизменяемые идентификаторы позволяют вашему приложению получить идентификатор, который не изменяется в течение всего времени существования элемента.'
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e0ddee215b7574e152fa5ffc574d218d5a2f811a
ms.sourcegitcommit: bbe42a15dad4ffe037a6934ab6001b585b7574c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2019
ms.locfileid: "31904093"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="7373d-105">Получение неизменяемых идентификаторов для ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="7373d-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="7373d-106">Элементы Outlook (сообщения, события, контакты, задачи) ведут себя довольно интересно, и вы этого либо никогда не замечали, либо это вызывало серьезные затруднения: их идентификаторы изменяются.</span><span class="sxs-lookup"><span data-stu-id="7373d-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="7373d-107">Это происходит нечасто (только при перемещении элемента), но может привести к серьезным проблемам для приложений, сохраняющих идентификаторы в автономном режиме для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="7373d-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="7373d-108">Неизменяемые идентификаторы позволяют вашему приложению получить идентификатор, который не изменяется в течение всего времени существования элемента.</span><span class="sxs-lookup"><span data-stu-id="7373d-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="7373d-109">**Важно!** Неизменяемые идентификаторы доступны в Microsoft Graph только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="7373d-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="7373d-110">Принципы работы</span><span class="sxs-lookup"><span data-stu-id="7373d-110">How it works</span></span>

<span data-ttu-id="7373d-111">Неизменяемый идентификатор — это необязательная функция для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7373d-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="7373d-112">Чтобы согласиться на ее использование, ваше приложение должно отправить дополнительный заголовок HTTP в запросах API:</span><span class="sxs-lookup"><span data-stu-id="7373d-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="7373d-113">Этот заголовок относится только к запросу, в который он входит.</span><span class="sxs-lookup"><span data-stu-id="7373d-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="7373d-114">Если вы хотите всегда использовать неизменяемые идентификаторы, необходимо включать этот заголовок в каждый запрос API.</span><span class="sxs-lookup"><span data-stu-id="7373d-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="7373d-115">Время существования неизменяемых идентификаторов</span><span class="sxs-lookup"><span data-stu-id="7373d-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="7373d-116">Неизменяемый идентификатор элемента не изменится до тех пор, пока элемент остается в том же почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7373d-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="7373d-117">Это означает, что неизменяемый идентификатор НЕ изменится, если элемент перемещается в другую папку почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7373d-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="7373d-118">Однако неизменяемый идентификатор изменится, если:</span><span class="sxs-lookup"><span data-stu-id="7373d-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="7373d-119">пользователь перемещает элемент в архивный почтовый ящик;</span><span class="sxs-lookup"><span data-stu-id="7373d-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="7373d-120">пользователь экспортирует элемент (в PST-файл, в виде MSG-файла и т. д.) и повторно импортирует его в свой почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="7373d-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="7373d-121">Элементы, поддерживающие неизменяемый идентификатор</span><span class="sxs-lookup"><span data-stu-id="7373d-121">Items that support immutable ID</span></span>

<span data-ttu-id="7373d-122">Приведенные ниже элементы поддерживают неизменяемые идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="7373d-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="7373d-123">Тип ресурса message</span><span class="sxs-lookup"><span data-stu-id="7373d-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="7373d-124">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="7373d-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="7373d-125">Тип ресурса event</span><span class="sxs-lookup"><span data-stu-id="7373d-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="7373d-126">Тип ресурса eventMessage</span><span class="sxs-lookup"><span data-stu-id="7373d-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="7373d-127">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="7373d-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="7373d-128">Тип ресурса outlookTask</span><span class="sxs-lookup"><span data-stu-id="7373d-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="7373d-129">Типы контейнеров (mailFolder, calendar и т. д.) не поддерживают неизменяемый идентификатор, но их обычные идентификаторы являются постоянными.</span><span class="sxs-lookup"><span data-stu-id="7373d-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="7373d-130">Неизменяемый идентификатор с уведомлением об изменениях</span><span class="sxs-lookup"><span data-stu-id="7373d-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="7373d-131">Можно запросить, чтобы Microsoft Graph отправлял неизменяемые идентификаторы в уведомлениях об изменениях путем включения заголовка `Prefer: IdType="ImmutableId"` при [создании подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="7373d-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="7373d-132">Существующие подписки, созданные без заголовка, продолжат использовать формат идентификатора по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7373d-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="7373d-133">Чтобы переключить существующие подписки на использование неизменяемых идентификаторов, их нужно удалить и заново создать с использованием заголовка.</span><span class="sxs-lookup"><span data-stu-id="7373d-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="7373d-134">Неизменяемый идентификатор с запросом изменений</span><span class="sxs-lookup"><span data-stu-id="7373d-134">Immutable ID with delta query</span></span>

<span data-ttu-id="7373d-135">Можно запросить, чтобы Microsoft Graph возвращал неизменяемые идентификаторы в [ответах на запросы изменений](delta-query-overview.md) для поддерживаемых типов ресурсов путем включения заголовка `Prefer: IdType="ImmutableId"`.</span><span class="sxs-lookup"><span data-stu-id="7373d-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="7373d-136">Значения `nextLink` и `deltaLink`, возвращаемые запросами изменений, совместимы с обоими форматами идентификаторов, поэтому вашему приложению не требуется повторно выполнять синхронизацию, чтобы воспользоваться преимуществами неизменяемого идентификатора.</span><span class="sxs-lookup"><span data-stu-id="7373d-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="7373d-137">С помощью заголовка можно получить неизменяемые идентификаторы в дальнейшем и можно отдельно [обновить хранилище вашего приложения](#updating-existing-data).</span><span class="sxs-lookup"><span data-stu-id="7373d-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="7373d-138">Обновление существующих данных</span><span class="sxs-lookup"><span data-stu-id="7373d-138">Updating existing data</span></span>

<span data-ttu-id="7373d-139">Если уже имеется база данных, заполненная тысячами обычных идентификаторов, можно перенести эти идентификаторы в неизменяемый формат с помощью функции [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="7373d-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="7373d-140">Вы можете обеспечить массив для перевода в нужный формат с количеством идентификаторов до 1000.</span><span class="sxs-lookup"><span data-stu-id="7373d-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="7373d-141">**Примечание.** Можно также можете использовать `translateExchangeIds` для переноса приложений веб-служб Exchange в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7373d-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="7373d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="7373d-142">Example</span></span>

<span data-ttu-id="7373d-143">В приведенном ниже примере обычный идентификатор Graph преобразуется в неизменяемый идентификатор Graph.</span><span class="sxs-lookup"><span data-stu-id="7373d-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="7373d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7373d-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="7373d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7373d-145">Response</span></span>

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```
