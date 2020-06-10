---
title: Тип ресурса Чанженотификатион
description: Представляет уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1bb5f8d5177e294a969fb48d335bd4a3061f1bb1
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681762"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="e097b-103">Тип ресурса Чанженотификатион</span><span class="sxs-lookup"><span data-stu-id="e097b-103">changeNotification resource type</span></span>

<span data-ttu-id="e097b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e097b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e097b-105">Представляет уведомление, отправленное подписчику.</span><span class="sxs-lookup"><span data-stu-id="e097b-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="e097b-106">Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="e097b-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e097b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e097b-107">Methods</span></span>

<span data-ttu-id="e097b-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e097b-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="e097b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e097b-109">Properties</span></span>

| <span data-ttu-id="e097b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e097b-110">Property</span></span> | <span data-ttu-id="e097b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e097b-111">Type</span></span> | <span data-ttu-id="e097b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e097b-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e097b-113">changeType</span><span class="sxs-lookup"><span data-stu-id="e097b-113">changeType</span></span> | <span data-ttu-id="e097b-114">string</span><span class="sxs-lookup"><span data-stu-id="e097b-114">string</span></span> | <span data-ttu-id="e097b-115">Указывает тип изменения, которое вызовет уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="e097b-115">Indicates the type of change that will raised the change notification.</span></span> <span data-ttu-id="e097b-116">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e097b-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="e097b-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e097b-117">Required.</span></span> |
| <span data-ttu-id="e097b-118">clientState</span><span class="sxs-lookup"><span data-stu-id="e097b-118">clientState</span></span> | <span data-ttu-id="e097b-119">string</span><span class="sxs-lookup"><span data-stu-id="e097b-119">string</span></span> | <span data-ttu-id="e097b-120">Значение свойства **clientState** , указанное в запросе на подписку (при наличии).</span><span class="sxs-lookup"><span data-stu-id="e097b-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="e097b-121">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="e097b-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="e097b-122">Клиент может проверить, что уведомление об изменении поступило из службы, сравнив значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="e097b-122">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="e097b-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e097b-123">Optional.</span></span> |
| <span data-ttu-id="e097b-124">енкриптедконтент</span><span class="sxs-lookup"><span data-stu-id="e097b-124">encryptedContent</span></span> | [<span data-ttu-id="e097b-125">Microsoft. Graph. Чанженотификатионенкриптедконтент</span><span class="sxs-lookup"><span data-stu-id="e097b-125">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="e097b-126">Просмотреть Зашифрованное содержимое, связанное с уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="e097b-126">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="e097b-127">Предоставляется только в том случае, если **енкриптионцертификате** и **инклудересаурцедата** определены во время запроса на подписку, и если он поддерживается ресурсом.</span><span class="sxs-lookup"><span data-stu-id="e097b-127">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="e097b-128">Необязательный</span><span class="sxs-lookup"><span data-stu-id="e097b-128">Optional</span></span> |
| <span data-ttu-id="e097b-129">лифецикливент</span><span class="sxs-lookup"><span data-stu-id="e097b-129">lifecycleEvent</span></span> | <span data-ttu-id="e097b-130">string</span><span class="sxs-lookup"><span data-stu-id="e097b-130">string</span></span> | <span data-ttu-id="e097b-131">Тип уведомления о жизненном цикле, если текущее уведомление является уведомлением жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="e097b-131">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="e097b-132">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e097b-132">Optional.</span></span> <span data-ttu-id="e097b-133">Поддерживаемые значения: `missed` , `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="e097b-133">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="e097b-134">id</span><span class="sxs-lookup"><span data-stu-id="e097b-134">id</span></span> | <span data-ttu-id="e097b-135">строка</span><span class="sxs-lookup"><span data-stu-id="e097b-135">string</span></span> | <span data-ttu-id="e097b-136">Уникальный идентификатор уведомления.</span><span class="sxs-lookup"><span data-stu-id="e097b-136">Unique ID for the notification.</span></span> <span data-ttu-id="e097b-137">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e097b-137">Optional.</span></span> |
| <span data-ttu-id="e097b-138">resource</span><span class="sxs-lookup"><span data-stu-id="e097b-138">resource</span></span> | <span data-ttu-id="e097b-139">string</span><span class="sxs-lookup"><span data-stu-id="e097b-139">string</span></span> | <span data-ttu-id="e097b-140">URI ресурса, который выдал уведомление об изменении относительно `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="e097b-140">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="e097b-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e097b-141">Required.</span></span> |
| <span data-ttu-id="e097b-142">resourceData</span><span class="sxs-lookup"><span data-stu-id="e097b-142">resourceData</span></span> | [<span data-ttu-id="e097b-143">Microsoft. Graph. resourceData</span><span class="sxs-lookup"><span data-stu-id="e097b-143">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="e097b-144">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="e097b-144">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="e097b-145">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e097b-145">Required.</span></span> |
| <span data-ttu-id="e097b-146">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="e097b-146">sequenceNumber</span></span> | <span data-ttu-id="e097b-147">int</span><span class="sxs-lookup"><span data-stu-id="e097b-147">int</span></span> | <span data-ttu-id="e097b-148">Число в последовательности для уведомления, помогающее клиентскому приложению определить, находятся ли уведомления в последовательности, или если уведомление отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e097b-148">A number in sequence for a notification, to help the client app identify if notifications are in sequence or if a notification is missing.</span></span> <span data-ttu-id="e097b-149">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e097b-149">Optional.</span></span> |
| <span data-ttu-id="e097b-150">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e097b-150">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="e097b-151">дата и время</span><span class="sxs-lookup"><span data-stu-id="e097b-151">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="e097b-152">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="e097b-152">The expiration time for the subscription.</span></span> <span data-ttu-id="e097b-153">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e097b-153">Required.</span></span> |
| <span data-ttu-id="e097b-154">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="e097b-154">subscriptionId</span></span> | <span data-ttu-id="e097b-155">string</span><span class="sxs-lookup"><span data-stu-id="e097b-155">string</span></span> | <span data-ttu-id="e097b-156">Уникальный идентификатор подписки, создавшей уведомление.</span><span class="sxs-lookup"><span data-stu-id="e097b-156">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="e097b-157">tenantId</span><span class="sxs-lookup"><span data-stu-id="e097b-157">tenantId</span></span> | <span data-ttu-id="e097b-158">кодом</span><span class="sxs-lookup"><span data-stu-id="e097b-158">guid</span></span> | <span data-ttu-id="e097b-159">Уникальный идентификатор клиента, с которого поступило уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="e097b-159">The unique identified of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e097b-160">Связи</span><span class="sxs-lookup"><span data-stu-id="e097b-160">Relationships</span></span>

<span data-ttu-id="e097b-161">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e097b-161">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e097b-162">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e097b-162">JSON representation</span></span>

<span data-ttu-id="e097b-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e097b-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "sequenceNumber": 20,
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
