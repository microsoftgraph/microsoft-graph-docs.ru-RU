---
title: Получение неизменяемых идентификаторов для ресурсов Outlook
description: Неизменяемые идентификаторы позволяют вашему приложению получить идентификатор для элемента Outlook, который не изменяется в течение всего времени существования элемента.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 572804950148e0cf2b5dcbb35842195123698c49
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473660"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="04756-103">Получение неизменяемых идентификаторов для ресурсов Outlook</span><span class="sxs-lookup"><span data-stu-id="04756-103">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="04756-104">Элементы Outlook (сообщения, события, контакты, задачи) ведут себя довольно интересно, и вы этого либо никогда не замечали, либо это вызывало серьезные затруднения: их идентификаторы изменяются.</span><span class="sxs-lookup"><span data-stu-id="04756-104">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="04756-105">Это происходит нечасто (только при перемещении элемента), но может привести к серьезным проблемам для приложений, сохраняющих идентификаторы в автономном режиме для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="04756-105">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="04756-106">Неизменяемые идентификаторы позволяют вашему приложению получить идентификатор, который не изменяется в течение всего времени существования элемента.</span><span class="sxs-lookup"><span data-stu-id="04756-106">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> [!NOTE]
> <span data-ttu-id="04756-107">В неизменяемых идентификаторах, как и во всех других идентификаторах в Microsoft Graph, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="04756-107">Immutable identifiers, like all identifiers in Microsoft Graph, are case-sensitive.</span></span> <span data-ttu-id="04756-108">Об этом следует помнить при сравнении идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="04756-108">Keep this in mind if you are comparing IDs.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="04756-109">Принципы работы</span><span class="sxs-lookup"><span data-stu-id="04756-109">How it works</span></span>

<span data-ttu-id="04756-110">Неизменяемый идентификатор — это необязательная функция для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04756-110">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="04756-111">Чтобы согласиться на ее использование, ваше приложение должно отправить дополнительный заголовок HTTP в запросах API:</span><span class="sxs-lookup"><span data-stu-id="04756-111">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="04756-112">Этот заголовок относится только к запросу, в который он входит.</span><span class="sxs-lookup"><span data-stu-id="04756-112">This header only applies to the request it is included with.</span></span> <span data-ttu-id="04756-113">Если вы хотите всегда использовать неизменяемые идентификаторы, необходимо включать этот заголовок в каждый запрос API.</span><span class="sxs-lookup"><span data-stu-id="04756-113">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="04756-114">Время существования неизменяемых идентификаторов</span><span class="sxs-lookup"><span data-stu-id="04756-114">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="04756-115">Неизменяемый идентификатор элемента не изменится до тех пор, пока элемент остается в том же почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="04756-115">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="04756-116">Это означает, что неизменяемый идентификатор НЕ изменится, если элемент перемещается в другую папку почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="04756-116">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="04756-117">Однако неизменяемый идентификатор изменится, если:</span><span class="sxs-lookup"><span data-stu-id="04756-117">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="04756-118">пользователь перемещает элемент в архивный почтовый ящик;</span><span class="sxs-lookup"><span data-stu-id="04756-118">The user moves the item to an archive mailbox.</span></span>
- <span data-ttu-id="04756-119">пользователь экспортирует элемент (в PST-файл, в виде MSG-файла и т. д.) и повторно импортирует его в свой почтовый ящик;</span><span class="sxs-lookup"><span data-stu-id="04756-119">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox.</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="04756-120">Элементы, поддерживающие неизменяемый идентификатор</span><span class="sxs-lookup"><span data-stu-id="04756-120">Items that support immutable ID</span></span>

<span data-ttu-id="04756-121">Приведенные ниже элементы поддерживают неизменяемые идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="04756-121">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="04756-122">Тип ресурса message</span><span class="sxs-lookup"><span data-stu-id="04756-122">message resource type</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="04756-123">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="04756-123">attachment resource type</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="04756-124">Тип ресурса event</span><span class="sxs-lookup"><span data-stu-id="04756-124">event resource type</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="04756-125">Тип ресурса eventMessage</span><span class="sxs-lookup"><span data-stu-id="04756-125">eventMessage resource type</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="04756-126">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="04756-126">contact resource type</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="04756-127">Тип ресурса outlookTask</span><span class="sxs-lookup"><span data-stu-id="04756-127">outlookTask resource type</span></span>](/graph/api/resources/outlooktask)

<span data-ttu-id="04756-128">Типы контейнеров (mailFolder, calendar и т. д.) не поддерживают неизменяемый идентификатор, но их обычные идентификаторы являются постоянными.</span><span class="sxs-lookup"><span data-stu-id="04756-128">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-sending-mail"></a><span data-ttu-id="04756-129">Неизменяемый идентификатор с отправляемой почтой</span><span class="sxs-lookup"><span data-stu-id="04756-129">Immutable ID with sending mail</span></span>

<span data-ttu-id="04756-130">Вы можете использовать неизменяемые идентификаторы для поиска сообщения в папке "Отправленные" после его отправки с помощью следующих действий:</span><span class="sxs-lookup"><span data-stu-id="04756-130">You can use immutable IDs to find a message in the Sent Items folder after it has been sent, using the following steps:</span></span>

1. <span data-ttu-id="04756-131">[Создайте черновик сообщения](/graph/api/user-post-messages), используя заголовок `Prefer: IdType="ImmutableId"`, и сохраните свойство `id` сообщения в отклике.</span><span class="sxs-lookup"><span data-stu-id="04756-131">[Create a draft message](/graph/api/user-post-messages) using the `Prefer: IdType="ImmutableId"` header and save the `id` property of the message in the response.</span></span>
1. <span data-ttu-id="04756-132">[Отправьте сообщение](/graph/api/message-send), используя идентификатор из предыдущего действия.</span><span class="sxs-lookup"><span data-stu-id="04756-132">[Send the message](/graph/api/message-send) using the ID from the previous step.</span></span>
1. <span data-ttu-id="04756-133">[Получите сообщение](/graph/api/message-get), используя идентификатор из первого действия.</span><span class="sxs-lookup"><span data-stu-id="04756-133">[Get the message](/graph/api/message-get) using the ID from the first step.</span></span> <span data-ttu-id="04756-134">Это копия из папки "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="04756-134">This is the copy in Sent Items.</span></span>

> [!NOTE]
> <span data-ttu-id="04756-135">Получение сообщения из папки "Отправленные" сразу после отправки сообщения может завершиться неудачей.</span><span class="sxs-lookup"><span data-stu-id="04756-135">Getting the message in Sent Items may not succeed immediately after sending the message.</span></span> <span data-ttu-id="04756-136">Копия сообщения не создается, пока сообщение не будет успешно отправлено, что может занять некоторое время.</span><span class="sxs-lookup"><span data-stu-id="04756-136">The copy of the message is not created until the message successfully sends, which may take time.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="04756-137">Неизменяемый идентификатор с уведомлением об изменениях</span><span class="sxs-lookup"><span data-stu-id="04756-137">Immutable ID with change notifications</span></span>

<span data-ttu-id="04756-138">Можно запросить, чтобы Microsoft Graph отправлял неизменяемые идентификаторы в уведомлениях об изменениях путем включения заголовка `Prefer: IdType="ImmutableId"` при [создании подписки](/graph/api/subscription-post-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="04756-138">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions).</span></span> <span data-ttu-id="04756-139">Существующие подписки, созданные без заголовка, продолжат использовать формат идентификатора по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="04756-139">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="04756-140">Чтобы переключить существующие подписки на использование неизменяемых идентификаторов, их нужно удалить и заново создать с использованием заголовка.</span><span class="sxs-lookup"><span data-stu-id="04756-140">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="04756-141">Неизменяемый идентификатор с запросом изменений</span><span class="sxs-lookup"><span data-stu-id="04756-141">Immutable ID with delta query</span></span>

<span data-ttu-id="04756-142">Можно запросить, чтобы Microsoft Graph возвращал неизменяемые идентификаторы в [ответах на запросы изменений](delta-query-overview.md) для поддерживаемых типов ресурсов путем включения заголовка `Prefer: IdType="ImmutableId"`.</span><span class="sxs-lookup"><span data-stu-id="04756-142">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="04756-143">Значения `nextLink` и `deltaLink`, возвращаемые запросами изменений, совместимы с обоими форматами идентификаторов, поэтому вашему приложению не требуется повторно выполнять синхронизацию, чтобы воспользоваться преимуществами неизменяемого идентификатора.</span><span class="sxs-lookup"><span data-stu-id="04756-143">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="04756-144">С помощью заголовка можно получить неизменяемые идентификаторы в дальнейшем и можно отдельно [обновить хранилище вашего приложения](#updating-existing-data).</span><span class="sxs-lookup"><span data-stu-id="04756-144">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="04756-145">Обновление существующих данных</span><span class="sxs-lookup"><span data-stu-id="04756-145">Updating existing data</span></span>

<span data-ttu-id="04756-146">Если уже имеется база данных, заполненная тысячами обычных идентификаторов, можно перенести эти идентификаторы в неизменяемый формат с помощью функции [translateExchangeIds](/graph/api/user-translateexchangeids).</span><span class="sxs-lookup"><span data-stu-id="04756-146">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids) function.</span></span> <span data-ttu-id="04756-147">Вы можете обеспечить массив для перевода в нужный формат с количеством идентификаторов до 1000.</span><span class="sxs-lookup"><span data-stu-id="04756-147">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> [!NOTE]
> <span data-ttu-id="04756-148">Можно также использовать `translateExchangeIds` для переноса приложений веб-служб Exchange в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04756-148">You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="04756-149">Пример</span><span class="sxs-lookup"><span data-stu-id="04756-149">Example</span></span>

<span data-ttu-id="04756-150">В приведенном ниже примере обычный идентификатор Graph преобразуется в неизменяемый идентификатор Graph.</span><span class="sxs-lookup"><span data-stu-id="04756-150">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="04756-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="04756-151">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="04756-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="04756-152">Response</span></span>

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
