---
title: тип ресурса offerShiftRequest
description: Представляет тип запроса на смену, чтобы предложить переход другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f80e8578422aa00d6af1d2df22a0dfb7472c8c8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721483"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="c98b0-103">тип ресурса offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="c98b0-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="c98b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c98b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98b0-105">Представляет тип запроса на смену, чтобы предложить переход другому пользователю в команде.</span><span class="sxs-lookup"><span data-stu-id="c98b0-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="c98b0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c98b0-106">Methods</span></span>

| <span data-ttu-id="c98b0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c98b0-107">Method</span></span>       | <span data-ttu-id="c98b0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c98b0-108">Return Type</span></span> | <span data-ttu-id="c98b0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c98b0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c98b0-110">Создание</span><span class="sxs-lookup"><span data-stu-id="c98b0-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="c98b0-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="c98b0-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="c98b0-112">Создание экземпляра объекта offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="c98b0-112">Create an instance of an offerShiftRequest object.</span></span> |
| <span data-ttu-id="c98b0-113">[получение](../api/offershiftrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="c98b0-113">[Get](../api/offershiftrequest-get.md)</span></span> | [<span data-ttu-id="c98b0-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="c98b0-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="c98b0-115">Чтение свойств и связей объекта offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="c98b0-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="c98b0-116">List</span><span class="sxs-lookup"><span data-stu-id="c98b0-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="c98b0-117">Коллекция [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c98b0-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="c98b0-118">Чтение свойств и связей всех объектов offerShiftRequest в команде.</span><span class="sxs-lookup"><span data-stu-id="c98b0-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="c98b0-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="c98b0-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="c98b0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c98b0-120">None</span></span>|<span data-ttu-id="c98b0-121">Утверждение предложенияShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="c98b0-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="c98b0-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="c98b0-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="c98b0-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c98b0-123">None</span></span>|<span data-ttu-id="c98b0-124">Отклонение предложенияShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="c98b0-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="c98b0-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="c98b0-125">Properties</span></span>

| <span data-ttu-id="c98b0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c98b0-126">Property</span></span>     | <span data-ttu-id="c98b0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c98b0-127">Type</span></span>        | <span data-ttu-id="c98b0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c98b0-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c98b0-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c98b0-129">recipientActionDateTime</span></span>|<span data-ttu-id="c98b0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c98b0-130">DateTimeOffset</span></span>|<span data-ttu-id="c98b0-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c98b0-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c98b0-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c98b0-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c98b0-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="c98b0-133">recipientActionMessage</span></span>|<span data-ttu-id="c98b0-134">String</span><span class="sxs-lookup"><span data-stu-id="c98b0-134">String</span></span>| <span data-ttu-id="c98b0-135">Настраиваемые сообщения, отправленные получателем запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="c98b0-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="c98b0-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="c98b0-136">recipientUserId</span></span>|<span data-ttu-id="c98b0-137">String</span><span class="sxs-lookup"><span data-stu-id="c98b0-137">String</span></span>| <span data-ttu-id="c98b0-138">Пользовательский id получателя запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="c98b0-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="c98b0-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="c98b0-139">senderShiftId</span></span>|<span data-ttu-id="c98b0-140">String</span><span class="sxs-lookup"><span data-stu-id="c98b0-140">String</span></span>| <span data-ttu-id="c98b0-141">Пользовательский id отправитель запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="c98b0-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c98b0-142">Связи</span><span class="sxs-lookup"><span data-stu-id="c98b0-142">Relationships</span></span>

<span data-ttu-id="c98b0-143">Нет</span><span class="sxs-lookup"><span data-stu-id="c98b0-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c98b0-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c98b0-144">JSON representation</span></span>

<span data-ttu-id="c98b0-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c98b0-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


