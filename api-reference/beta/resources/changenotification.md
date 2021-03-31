---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправленного абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: bc015317d755444a7b52e43b9c107bd0c4ef7acc
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469393"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="2e090-103">Тип ресурса changeNotification</span><span class="sxs-lookup"><span data-stu-id="2e090-103">changeNotification resource type</span></span>

<span data-ttu-id="2e090-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e090-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e090-105">Представляет уведомление, отправленные абоненту.</span><span class="sxs-lookup"><span data-stu-id="2e090-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="2e090-106">Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="2e090-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2e090-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2e090-107">Methods</span></span>

<span data-ttu-id="2e090-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e090-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2e090-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e090-109">Properties</span></span>

| <span data-ttu-id="2e090-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e090-110">Property</span></span> | <span data-ttu-id="2e090-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2e090-111">Type</span></span> | <span data-ttu-id="2e090-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2e090-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2e090-113">changeType</span><span class="sxs-lookup"><span data-stu-id="2e090-113">changeType</span></span> | <span data-ttu-id="2e090-114">string</span><span class="sxs-lookup"><span data-stu-id="2e090-114">string</span></span> | <span data-ttu-id="2e090-115">Указывает тип изменения, которое поднимет уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="2e090-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="2e090-116">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="2e090-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="2e090-117">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2e090-117">Required.</span></span> |
| <span data-ttu-id="2e090-118">clientState</span><span class="sxs-lookup"><span data-stu-id="2e090-118">clientState</span></span> | <span data-ttu-id="2e090-119">string</span><span class="sxs-lookup"><span data-stu-id="2e090-119">string</span></span> | <span data-ttu-id="2e090-120">Значение свойства **clientState,** отправленного в запросе подписки (если таково).</span><span class="sxs-lookup"><span data-stu-id="2e090-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="2e090-121">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="2e090-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="2e090-122">Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значения свойства **clientState.**</span><span class="sxs-lookup"><span data-stu-id="2e090-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="2e090-123">Значение свойства **clientState,** отправленного с подпиской, сравнивается со значением свойства **clientState,** полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="2e090-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="2e090-124">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2e090-124">Optional.</span></span> |
| <span data-ttu-id="2e090-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="2e090-125">encryptedContent</span></span> | [<span data-ttu-id="2e090-126">microsoft.graph.changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="2e090-126">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="2e090-127">(Предварительный просмотр) Зашифрованное содержимое, прикрепленное с уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="2e090-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="2e090-128">Только если **шифрованиеCertificate** и **includeResourceData** было определено во время запроса подписки и если ресурс поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="2e090-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="2e090-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2e090-129">Optional.</span></span> |
| <span data-ttu-id="2e090-130">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="2e090-130">lifecycleEvent</span></span> | <span data-ttu-id="2e090-131">Строка</span><span class="sxs-lookup"><span data-stu-id="2e090-131">string</span></span> | <span data-ttu-id="2e090-132">Тип уведомления жизненного цикла, если текущее уведомление является уведомлением жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="2e090-132">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="2e090-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2e090-133">Optional.</span></span> <span data-ttu-id="2e090-134">Поддерживаемые значения `missed` : `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="2e090-134">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="2e090-135">id</span><span class="sxs-lookup"><span data-stu-id="2e090-135">id</span></span> | <span data-ttu-id="2e090-136">string</span><span class="sxs-lookup"><span data-stu-id="2e090-136">string</span></span> | <span data-ttu-id="2e090-137">Уникальный ID для уведомления.</span><span class="sxs-lookup"><span data-stu-id="2e090-137">Unique ID for the notification.</span></span> <span data-ttu-id="2e090-138">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2e090-138">Optional.</span></span> |
| <span data-ttu-id="2e090-139">resource</span><span class="sxs-lookup"><span data-stu-id="2e090-139">resource</span></span> | <span data-ttu-id="2e090-140">string</span><span class="sxs-lookup"><span data-stu-id="2e090-140">string</span></span> | <span data-ttu-id="2e090-141">URI ресурса, излучающего уведомление об изменении относительно `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="2e090-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="2e090-142">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2e090-142">Required.</span></span> |
| <span data-ttu-id="2e090-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="2e090-143">resourceData</span></span> | [<span data-ttu-id="2e090-144">microsoft.graph.resourceData</span><span class="sxs-lookup"><span data-stu-id="2e090-144">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="2e090-145">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="2e090-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="2e090-146">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2e090-146">Required.</span></span> |
| <span data-ttu-id="2e090-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2e090-147">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="2e090-148">дата и время</span><span class="sxs-lookup"><span data-stu-id="2e090-148">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="2e090-149">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="2e090-149">The expiration time for the subscription.</span></span> <span data-ttu-id="2e090-150">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2e090-150">Required.</span></span> |
| <span data-ttu-id="2e090-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="2e090-151">subscriptionId</span></span> | <span data-ttu-id="2e090-152">строка</span><span class="sxs-lookup"><span data-stu-id="2e090-152">string</span></span> | <span data-ttu-id="2e090-153">Уникальный идентификатор подписки, которая породила уведомление.</span><span class="sxs-lookup"><span data-stu-id="2e090-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="2e090-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="2e090-154">tenantId</span></span> | <span data-ttu-id="2e090-155">guid</span><span class="sxs-lookup"><span data-stu-id="2e090-155">guid</span></span> | <span data-ttu-id="2e090-156">Уникальный идентификатор клиента, из которого возникло уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="2e090-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e090-157">Связи</span><span class="sxs-lookup"><span data-stu-id="2e090-157">Relationships</span></span>

<span data-ttu-id="2e090-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2e090-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e090-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e090-159">JSON representation</span></span>

<span data-ttu-id="2e090-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e090-160">The following is a JSON representation of the resource.</span></span>

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


