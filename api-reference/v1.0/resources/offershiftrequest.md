---
title: тип ресурса offerShiftRequest
description: Представляет запрос на предложение о переходе другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 508f8c79606ef6e9e0d3778899cb04789b9defde
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720804"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="1a5dd-103">тип ресурса offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1a5dd-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="1a5dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a5dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a5dd-105">Представляет запрос на предложение о переходе другому пользователю в команде.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-105">Represents a request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="1a5dd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1a5dd-106">Methods</span></span>

| <span data-ttu-id="1a5dd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1a5dd-107">Method</span></span>       | <span data-ttu-id="1a5dd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a5dd-108">Return Type</span></span> | <span data-ttu-id="1a5dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a5dd-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1a5dd-110">Список</span><span class="sxs-lookup"><span data-stu-id="1a5dd-110">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="1a5dd-111">Коллекция [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1a5dd-111">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="1a5dd-112">Ознакомьтесь с свойствами и отношениями всех **объектов offerShiftRequest** в команде.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-112">Read the properties and relationships of all **offerShiftRequest** objects in a team.</span></span> |
| [<span data-ttu-id="1a5dd-113">Создание</span><span class="sxs-lookup"><span data-stu-id="1a5dd-113">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="1a5dd-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1a5dd-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="1a5dd-115">Создание экземпляра объекта **offerShiftRequest.**</span><span class="sxs-lookup"><span data-stu-id="1a5dd-115">Create an instance of an **offerShiftRequest** object.</span></span> |
| <span data-ttu-id="1a5dd-116">[получение](../api/offershiftrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="1a5dd-116">[Get](../api/offershiftrequest-get.md)</span></span> | [<span data-ttu-id="1a5dd-117">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1a5dd-117">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="1a5dd-118">Ознакомьтесь с свойствами и отношениями объекта **offerShiftRequest.**</span><span class="sxs-lookup"><span data-stu-id="1a5dd-118">Read the properties and relationships of an **offerShiftRequest** object.</span></span> |
|[<span data-ttu-id="1a5dd-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="1a5dd-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="1a5dd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1a5dd-120">None</span></span>|<span data-ttu-id="1a5dd-121">Утверждение **предложенияShiftRequest**.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-121">Approve an **offerShiftRequest**.</span></span> |
|[<span data-ttu-id="1a5dd-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="1a5dd-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="1a5dd-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1a5dd-123">None</span></span>|<span data-ttu-id="1a5dd-124">Отклонение **предложенияShiftRequest**.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-124">Decline an **offerShiftRequest**.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a5dd-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a5dd-125">Properties</span></span>

| <span data-ttu-id="1a5dd-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a5dd-126">Property</span></span>     | <span data-ttu-id="1a5dd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1a5dd-127">Type</span></span>        | <span data-ttu-id="1a5dd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1a5dd-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a5dd-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1a5dd-129">recipientActionDateTime</span></span>|<span data-ttu-id="1a5dd-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a5dd-130">DateTimeOffset</span></span>|<span data-ttu-id="1a5dd-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1a5dd-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1a5dd-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1a5dd-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="1a5dd-133">recipientActionMessage</span></span>|<span data-ttu-id="1a5dd-134">String</span><span class="sxs-lookup"><span data-stu-id="1a5dd-134">String</span></span>| <span data-ttu-id="1a5dd-135">Настраиваемые сообщения, отправленные получателем запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="1a5dd-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="1a5dd-136">recipientUserId</span></span>|<span data-ttu-id="1a5dd-137">String</span><span class="sxs-lookup"><span data-stu-id="1a5dd-137">String</span></span>| <span data-ttu-id="1a5dd-138">Пользовательский ID получателя запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-138">User ID of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="1a5dd-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="1a5dd-139">senderShiftId</span></span>|<span data-ttu-id="1a5dd-140">String</span><span class="sxs-lookup"><span data-stu-id="1a5dd-140">String</span></span>| <span data-ttu-id="1a5dd-141">Пользовательский ID отправитель запроса на перенос предложения.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-141">User ID of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a5dd-142">Связи</span><span class="sxs-lookup"><span data-stu-id="1a5dd-142">Relationships</span></span>

<span data-ttu-id="1a5dd-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a5dd-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a5dd-144">JSON representation</span></span>

<span data-ttu-id="1a5dd-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a5dd-145">The following is a JSON representation of the resource.</span></span>

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

