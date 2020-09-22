---
title: Тип ресурса Оффершифтрекуест
description: Представляет тип запроса на смену для предоставления смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021275"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="18576-103">Тип ресурса Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="18576-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="18576-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18576-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18576-105">Представляет тип запроса на смену для предоставления смены другому пользователю в команде.</span><span class="sxs-lookup"><span data-stu-id="18576-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="18576-106">Методы</span><span class="sxs-lookup"><span data-stu-id="18576-106">Methods</span></span>

| <span data-ttu-id="18576-107">Метод</span><span class="sxs-lookup"><span data-stu-id="18576-107">Method</span></span>       | <span data-ttu-id="18576-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18576-108">Return Type</span></span> | <span data-ttu-id="18576-109">Описание</span><span class="sxs-lookup"><span data-stu-id="18576-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="18576-110">Создание</span><span class="sxs-lookup"><span data-stu-id="18576-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="18576-111">оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="18576-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="18576-112">Создайте экземпляр объекта Оффершифтрекуест.</span><span class="sxs-lookup"><span data-stu-id="18576-112">Create an instance of an offerShiftRequest object.</span></span> |
| <span data-ttu-id="18576-113">[получение](../api/offershiftrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="18576-113">[Get](../api/offershiftrequest-get.md)</span></span> | [<span data-ttu-id="18576-114">оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="18576-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="18576-115">Чтение свойств и связей объекта Оффершифтрекуест.</span><span class="sxs-lookup"><span data-stu-id="18576-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="18576-116">List</span><span class="sxs-lookup"><span data-stu-id="18576-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="18576-117">Коллекция [оффершифтрекуест](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="18576-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="18576-118">Чтение свойств и связей всех объектов Оффершифтрекуест в команде.</span><span class="sxs-lookup"><span data-stu-id="18576-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="18576-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="18576-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="18576-120">Нет</span><span class="sxs-lookup"><span data-stu-id="18576-120">None</span></span>|<span data-ttu-id="18576-121">Утверждение Оффершифтрекуест.</span><span class="sxs-lookup"><span data-stu-id="18576-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="18576-122">Отклоня</span><span class="sxs-lookup"><span data-stu-id="18576-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="18576-123">Нет</span><span class="sxs-lookup"><span data-stu-id="18576-123">None</span></span>|<span data-ttu-id="18576-124">Отклонить Оффершифтрекуест.</span><span class="sxs-lookup"><span data-stu-id="18576-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="18576-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="18576-125">Properties</span></span>

| <span data-ttu-id="18576-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="18576-126">Property</span></span>     | <span data-ttu-id="18576-127">Тип</span><span class="sxs-lookup"><span data-stu-id="18576-127">Type</span></span>        | <span data-ttu-id="18576-128">Описание</span><span class="sxs-lookup"><span data-stu-id="18576-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18576-129">реЦипиентактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="18576-129">recipientActionDateTime</span></span>|<span data-ttu-id="18576-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18576-130">DateTimeOffset</span></span>|<span data-ttu-id="18576-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="18576-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="18576-133">реЦипиентактионмессаже</span><span class="sxs-lookup"><span data-stu-id="18576-133">recipientActionMessage</span></span>|<span data-ttu-id="18576-134">String</span><span class="sxs-lookup"><span data-stu-id="18576-134">String</span></span>| <span data-ttu-id="18576-135">Настраиваемое сообщение, отправленное получателем запроса на смену предложением.</span><span class="sxs-lookup"><span data-stu-id="18576-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="18576-136">реЦипиентусерид</span><span class="sxs-lookup"><span data-stu-id="18576-136">recipientUserId</span></span>|<span data-ttu-id="18576-137">String</span><span class="sxs-lookup"><span data-stu-id="18576-137">String</span></span>| <span data-ttu-id="18576-138">Идентификатор пользователя, который является получателем запроса на смену.</span><span class="sxs-lookup"><span data-stu-id="18576-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="18576-139">сендершифтид</span><span class="sxs-lookup"><span data-stu-id="18576-139">senderShiftId</span></span>|<span data-ttu-id="18576-140">String</span><span class="sxs-lookup"><span data-stu-id="18576-140">String</span></span>| <span data-ttu-id="18576-141">Идентификатор пользователя отправителя запроса на смену.</span><span class="sxs-lookup"><span data-stu-id="18576-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18576-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="18576-142">Relationships</span></span>

<span data-ttu-id="18576-143">Нет</span><span class="sxs-lookup"><span data-stu-id="18576-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18576-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18576-144">JSON representation</span></span>

<span data-ttu-id="18576-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18576-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
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


