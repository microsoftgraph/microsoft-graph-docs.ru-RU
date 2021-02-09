---
title: Тип ресурса offerShiftRequest
description: Представляет тип запроса на смену для предложения смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d1b26d7801a3eb4570104ff68b9037fd9c553a68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156716"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="553ec-103">Тип ресурса offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="553ec-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="553ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="553ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="553ec-105">Представляет тип запроса на смену для предложения смены другому пользователю в команде.</span><span class="sxs-lookup"><span data-stu-id="553ec-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="553ec-106">Методы</span><span class="sxs-lookup"><span data-stu-id="553ec-106">Methods</span></span>

| <span data-ttu-id="553ec-107">Метод</span><span class="sxs-lookup"><span data-stu-id="553ec-107">Method</span></span>       | <span data-ttu-id="553ec-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="553ec-108">Return Type</span></span> | <span data-ttu-id="553ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="553ec-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="553ec-110">Создание</span><span class="sxs-lookup"><span data-stu-id="553ec-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="553ec-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="553ec-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="553ec-112">Создание экземпляра объекта offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="553ec-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="553ec-113">Получение</span><span class="sxs-lookup"><span data-stu-id="553ec-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="553ec-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="553ec-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="553ec-115">Чтение свойств и связей объекта offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="553ec-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="553ec-116">Список</span><span class="sxs-lookup"><span data-stu-id="553ec-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="553ec-117">Коллекция [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="553ec-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="553ec-118">Чтение свойств и связей всех объектов offerShiftRequest в команде.</span><span class="sxs-lookup"><span data-stu-id="553ec-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="553ec-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="553ec-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="553ec-120">Нет</span><span class="sxs-lookup"><span data-stu-id="553ec-120">None</span></span>|<span data-ttu-id="553ec-121">Утверждение offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="553ec-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="553ec-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="553ec-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="553ec-123">Нет</span><span class="sxs-lookup"><span data-stu-id="553ec-123">None</span></span>|<span data-ttu-id="553ec-124">Отклонение предложенияShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="553ec-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="553ec-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="553ec-125">Properties</span></span>

| <span data-ttu-id="553ec-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="553ec-126">Property</span></span>     | <span data-ttu-id="553ec-127">Тип</span><span class="sxs-lookup"><span data-stu-id="553ec-127">Type</span></span>        | <span data-ttu-id="553ec-128">Описание</span><span class="sxs-lookup"><span data-stu-id="553ec-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="553ec-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="553ec-129">recipientActionDateTime</span></span>|<span data-ttu-id="553ec-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="553ec-130">DateTimeOffset</span></span>|<span data-ttu-id="553ec-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="553ec-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="553ec-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="553ec-133">recipientActionMessage</span></span>|<span data-ttu-id="553ec-134">String</span><span class="sxs-lookup"><span data-stu-id="553ec-134">String</span></span>| <span data-ttu-id="553ec-135">Настраиваемые сообщения, отправленные получателем запроса на смену предложения.</span><span class="sxs-lookup"><span data-stu-id="553ec-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="553ec-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="553ec-136">recipientUserId</span></span>|<span data-ttu-id="553ec-137">String</span><span class="sxs-lookup"><span data-stu-id="553ec-137">String</span></span>| <span data-ttu-id="553ec-138">ИД пользователя получателя запроса на смену предложения.</span><span class="sxs-lookup"><span data-stu-id="553ec-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="553ec-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="553ec-139">senderShiftId</span></span>|<span data-ttu-id="553ec-140">String</span><span class="sxs-lookup"><span data-stu-id="553ec-140">String</span></span>| <span data-ttu-id="553ec-141">ИД отправитель запроса на смену предложения.</span><span class="sxs-lookup"><span data-stu-id="553ec-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="553ec-142">Связи</span><span class="sxs-lookup"><span data-stu-id="553ec-142">Relationships</span></span>

<span data-ttu-id="553ec-143">Нет</span><span class="sxs-lookup"><span data-stu-id="553ec-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="553ec-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="553ec-144">JSON representation</span></span>

<span data-ttu-id="553ec-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="553ec-145">The following is a JSON representation of the resource.</span></span>

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


