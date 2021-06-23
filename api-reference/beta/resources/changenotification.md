---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправленного абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 43933d31b8ac12f77331887c0421c3b6fc50b66b
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082379"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="a3512-103">Тип ресурса changeNotification</span><span class="sxs-lookup"><span data-stu-id="a3512-103">changeNotification resource type</span></span>

<span data-ttu-id="a3512-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3512-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3512-105">Представляет уведомление, отправленные абоненту.</span><span class="sxs-lookup"><span data-stu-id="a3512-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="a3512-106">Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="a3512-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a3512-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3512-107">Methods</span></span>

<span data-ttu-id="a3512-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="a3512-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="a3512-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3512-109">Properties</span></span>

| <span data-ttu-id="a3512-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3512-110">Property</span></span> | <span data-ttu-id="a3512-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a3512-111">Type</span></span> | <span data-ttu-id="a3512-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a3512-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a3512-113">changeType</span><span class="sxs-lookup"><span data-stu-id="a3512-113">changeType</span></span> | <span data-ttu-id="a3512-114">changeType</span><span class="sxs-lookup"><span data-stu-id="a3512-114">changeType</span></span> | <span data-ttu-id="a3512-115">Указывает тип изменения, которое поднимет уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="a3512-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="a3512-116">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="a3512-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="a3512-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3512-117">Required.</span></span> |
| <span data-ttu-id="a3512-118">clientState</span><span class="sxs-lookup"><span data-stu-id="a3512-118">clientState</span></span> | <span data-ttu-id="a3512-119">string</span><span class="sxs-lookup"><span data-stu-id="a3512-119">string</span></span> | <span data-ttu-id="a3512-120">Значение свойства **clientState,** отправленного в запросе подписки (если таково).</span><span class="sxs-lookup"><span data-stu-id="a3512-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="a3512-121">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="a3512-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="a3512-122">Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значения свойства **clientState.**</span><span class="sxs-lookup"><span data-stu-id="a3512-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="a3512-123">Значение свойства **clientState,** отправленного с подпиской, сравнивается со значением свойства **clientState,** полученного с каждым уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="a3512-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="a3512-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a3512-124">Optional.</span></span> |
| <span data-ttu-id="a3512-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="a3512-125">encryptedContent</span></span> | [<span data-ttu-id="a3512-126">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="a3512-126">changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="a3512-127">(Предварительный просмотр) Зашифрованное содержимое, прикрепленное с уведомлением об изменении.</span><span class="sxs-lookup"><span data-stu-id="a3512-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="a3512-128">Только если **шифрованиеCertificate** и **includeResourceData** было определено во время запроса подписки и если ресурс поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="a3512-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="a3512-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a3512-129">Optional.</span></span> |
| <span data-ttu-id="a3512-130">id</span><span class="sxs-lookup"><span data-stu-id="a3512-130">id</span></span> | <span data-ttu-id="a3512-131">string</span><span class="sxs-lookup"><span data-stu-id="a3512-131">string</span></span> | <span data-ttu-id="a3512-132">Уникальный ID для уведомления.</span><span class="sxs-lookup"><span data-stu-id="a3512-132">Unique ID for the notification.</span></span> <span data-ttu-id="a3512-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a3512-133">Optional.</span></span> |
| <span data-ttu-id="a3512-134">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="a3512-134">lifecycleEvent</span></span> | <span data-ttu-id="a3512-135">lifecycleEventType</span><span class="sxs-lookup"><span data-stu-id="a3512-135">lifecycleEventType</span></span> | <span data-ttu-id="a3512-136">Тип уведомления жизненного цикла, если текущее уведомление является уведомлением жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="a3512-136">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="a3512-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a3512-137">Optional.</span></span> <span data-ttu-id="a3512-138">Поддерживаемые значения `missed` : `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="a3512-138">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="a3512-139">resource</span><span class="sxs-lookup"><span data-stu-id="a3512-139">resource</span></span> | <span data-ttu-id="a3512-140">string</span><span class="sxs-lookup"><span data-stu-id="a3512-140">string</span></span> | <span data-ttu-id="a3512-141">URI ресурса, излучающего уведомление об изменении относительно `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="a3512-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="a3512-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3512-142">Required.</span></span> |
| <span data-ttu-id="a3512-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="a3512-143">resourceData</span></span> | [<span data-ttu-id="a3512-144">resourceData</span><span class="sxs-lookup"><span data-stu-id="a3512-144">resourceData</span></span>](resourcedata.md) | <span data-ttu-id="a3512-145">Содержимое этого свойства зависит от типа связанного с ним ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3512-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="a3512-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3512-146">Required.</span></span> |
| <span data-ttu-id="a3512-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a3512-147">subscriptionExpirationDateTime</span></span> | <span data-ttu-id="a3512-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3512-148">DateTimeOffset</span></span> | <span data-ttu-id="a3512-149">Время окончания срока действия подписки.</span><span class="sxs-lookup"><span data-stu-id="a3512-149">The expiration time for the subscription.</span></span> <span data-ttu-id="a3512-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3512-150">Required.</span></span> |
| <span data-ttu-id="a3512-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="a3512-151">subscriptionId</span></span> | <span data-ttu-id="a3512-152">GUID</span><span class="sxs-lookup"><span data-stu-id="a3512-152">GUID</span></span> | <span data-ttu-id="a3512-153">Уникальный идентификатор подписки, которая породила уведомление.</span><span class="sxs-lookup"><span data-stu-id="a3512-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="a3512-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="a3512-154">tenantId</span></span> | <span data-ttu-id="a3512-155">GUID</span><span class="sxs-lookup"><span data-stu-id="a3512-155">GUID</span></span> | <span data-ttu-id="a3512-156">Уникальный идентификатор клиента, из которого возникло уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="a3512-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3512-157">Связи</span><span class="sxs-lookup"><span data-stu-id="a3512-157">Relationships</span></span>

<span data-ttu-id="a3512-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a3512-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3512-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3512-159">JSON representation</span></span>

<span data-ttu-id="a3512-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3512-160">The following is a JSON representation of the resource.</span></span>

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


