---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 6a39d156849236a40268064cb234e6015c9424f3
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598546"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="ee5a6-103">Тип ресурса changeNotification</span><span class="sxs-lookup"><span data-stu-id="ee5a6-103">changeNotification resource type</span></span>

<span data-ttu-id="ee5a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee5a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee5a6-105">Представляет уведомление, отправленное подписчику.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="ee5a6-106">Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="ee5a6-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ee5a6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ee5a6-107">Methods</span></span>

<span data-ttu-id="ee5a6-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="ee5a6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee5a6-109">Properties</span></span>

| <span data-ttu-id="ee5a6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee5a6-110">Property</span></span> | <span data-ttu-id="ee5a6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ee5a6-111">Type</span></span> | <span data-ttu-id="ee5a6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ee5a6-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ee5a6-113">changeType</span><span class="sxs-lookup"><span data-stu-id="ee5a6-113">changeType</span></span> | <span data-ttu-id="ee5a6-114">string</span><span class="sxs-lookup"><span data-stu-id="ee5a6-114">string</span></span> | <span data-ttu-id="ee5a6-115">Указывает тип изменения, которое вызывает уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="ee5a6-116">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="ee5a6-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-117">Required.</span></span> |
| <span data-ttu-id="ee5a6-118">clientState</span><span class="sxs-lookup"><span data-stu-id="ee5a6-118">clientState</span></span> | <span data-ttu-id="ee5a6-119">string</span><span class="sxs-lookup"><span data-stu-id="ee5a6-119">string</span></span> | <span data-ttu-id="ee5a6-120">Значение свойства **clientState** , указанное в запросе на подписку (при наличии).</span><span class="sxs-lookup"><span data-stu-id="ee5a6-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="ee5a6-121">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="ee5a6-122">Клиент может проверить, поступило ли уведомление об изменении из службы, сравнив значения свойства **clientState** .</span><span class="sxs-lookup"><span data-stu-id="ee5a6-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="ee5a6-123">Значение свойства **clientState** , отправляемого с подпиской, сравнивается со значением свойства **clientState** , полученного при каждом уведомлении об изменении.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="ee5a6-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-124">Optional.</span></span> |
| <span data-ttu-id="ee5a6-125">енкриптедконтент</span><span class="sxs-lookup"><span data-stu-id="ee5a6-125">encryptedContent</span></span> | [<span data-ttu-id="ee5a6-126">Microsoft. Graph. Чанженотификатионенкриптедконтент</span><span class="sxs-lookup"><span data-stu-id="ee5a6-126">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="ee5a6-127">Просмотреть Зашифрованное содержимое, связанное с уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="ee5a6-128">Предоставляется только в том случае, если **енкриптионцертификате** и **инклудересаурцедата** определены во время запроса на подписку, и если он поддерживается ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="ee5a6-129">Необязательна</span><span class="sxs-lookup"><span data-stu-id="ee5a6-129">Optional</span></span> |
| <span data-ttu-id="ee5a6-130">лифецикливент</span><span class="sxs-lookup"><span data-stu-id="ee5a6-130">lifecycleEvent</span></span> | <span data-ttu-id="ee5a6-131">string</span><span class="sxs-lookup"><span data-stu-id="ee5a6-131">string</span></span> | <span data-ttu-id="ee5a6-132">Тип уведомления о жизненном цикле, если текущее уведомление является уведомлением жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-132">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="ee5a6-133">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-133">Optional.</span></span> <span data-ttu-id="ee5a6-134">Поддерживаемые значения: `missed` , `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="ee5a6-134">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="ee5a6-135">id</span><span class="sxs-lookup"><span data-stu-id="ee5a6-135">id</span></span> | <span data-ttu-id="ee5a6-136">string</span><span class="sxs-lookup"><span data-stu-id="ee5a6-136">string</span></span> | <span data-ttu-id="ee5a6-137">Уникальный идентификатор уведомления.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-137">Unique ID for the notification.</span></span> <span data-ttu-id="ee5a6-138">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-138">Optional.</span></span> |
| <span data-ttu-id="ee5a6-139">resource</span><span class="sxs-lookup"><span data-stu-id="ee5a6-139">resource</span></span> | <span data-ttu-id="ee5a6-140">string</span><span class="sxs-lookup"><span data-stu-id="ee5a6-140">string</span></span> | <span data-ttu-id="ee5a6-141">URI ресурса, который выдал уведомление об изменении относительно `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="ee5a6-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="ee5a6-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-142">Required.</span></span> |
| <span data-ttu-id="ee5a6-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="ee5a6-143">resourceData</span></span> | [<span data-ttu-id="ee5a6-144">Microsoft. Graph. resourceData</span><span class="sxs-lookup"><span data-stu-id="ee5a6-144">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="ee5a6-145">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="ee5a6-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-146">Required.</span></span> |
| <span data-ttu-id="ee5a6-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee5a6-147">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="ee5a6-148">дата и время</span><span class="sxs-lookup"><span data-stu-id="ee5a6-148">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="ee5a6-149">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-149">The expiration time for the subscription.</span></span> <span data-ttu-id="ee5a6-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-150">Required.</span></span> |
| <span data-ttu-id="ee5a6-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="ee5a6-151">subscriptionId</span></span> | <span data-ttu-id="ee5a6-152">строка</span><span class="sxs-lookup"><span data-stu-id="ee5a6-152">string</span></span> | <span data-ttu-id="ee5a6-153">Уникальный идентификатор подписки, создавшей уведомление.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="ee5a6-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="ee5a6-154">tenantId</span></span> | <span data-ttu-id="ee5a6-155">кодом</span><span class="sxs-lookup"><span data-stu-id="ee5a6-155">guid</span></span> | <span data-ttu-id="ee5a6-156">Уникальный идентификатор клиента, с которого поступило уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ee5a6-157">Связи</span><span class="sxs-lookup"><span data-stu-id="ee5a6-157">Relationships</span></span>

<span data-ttu-id="ee5a6-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee5a6-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ee5a6-159">JSON representation</span></span>

<span data-ttu-id="ee5a6-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee5a6-160">The following is a JSON representation of the resource.</span></span>

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
