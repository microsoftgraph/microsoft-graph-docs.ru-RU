---
title: тип ресурса teamsAsyncOperation
description: 'Операция Microsoft Teams async — это операция, которая выходит за рамки срока службы одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9239e9543b77348b4524dc76be8fee64e1b9919a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030840"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="4a1b2-103">тип ресурса teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4a1b2-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="4a1b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a1b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a1b2-105">Операция Microsoft Teams async — это операция, которая выходит за рамки срока службы одного запроса API.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="4a1b2-106">Эти операции являются длительными или слишком дорогими для выполнения в период времени, зарожаемого запросом.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="4a1b2-107">При инициировании операции async метод возвращает код ответа 202 Accepted.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="4a1b2-108">В ответе также будет содержаться загон расположения, который содержит расположение teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="4a1b2-109">Периодически проверяйте состояние операции, делая запрос GET в этом расположении; подождите >30 секунд между проверками.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="4a1b2-110">После успешного завершения запроса состояние будет "успешным", а целевое значениеResourceLocation будет указать на созданный или измененный ресурс.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="methods"></a><span data-ttu-id="4a1b2-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4a1b2-111">Methods</span></span>

|  <span data-ttu-id="4a1b2-112">Метод</span><span class="sxs-lookup"><span data-stu-id="4a1b2-112">Method</span></span>                                                                   |  <span data-ttu-id="4a1b2-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4a1b2-113">Return Type</span></span>                                                                     | <span data-ttu-id="4a1b2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4a1b2-114">Description</span></span>                                                       | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :---------------------------------------------------------------- |
| [<span data-ttu-id="4a1b2-115">Список операций в чате</span><span class="sxs-lookup"><span data-stu-id="4a1b2-115">List operations on a chat</span></span>](../api/chat-list-operations.md)               | <span data-ttu-id="4a1b2-116">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="4a1b2-116">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="4a1b2-117">Список операций async, которые запускались или запускались в определенном чате.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-117">List async operations that ran or are running on a specific chat.</span></span> |
| [<span data-ttu-id="4a1b2-118">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="4a1b2-118">Get operation</span></span>](../api/teamsasyncoperation-get.md)                   | <span data-ttu-id="4a1b2-119">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="4a1b2-119">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="4a1b2-120">Получите операцию async, которая запущена или запущена на определенном ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-120">Get an async operation that ran or is running on a specific resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a1b2-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a1b2-121">Properties</span></span>

| <span data-ttu-id="4a1b2-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a1b2-122">Property</span></span> | <span data-ttu-id="4a1b2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4a1b2-123">Type</span></span>   | <span data-ttu-id="4a1b2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4a1b2-124">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a1b2-125">id</span><span class="sxs-lookup"><span data-stu-id="4a1b2-125">id</span></span>|<span data-ttu-id="4a1b2-126">string</span><span class="sxs-lookup"><span data-stu-id="4a1b2-126">string</span></span> |<span data-ttu-id="4a1b2-127">Уникальный id операции.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-127">Unique operation id.</span></span>|
|<span data-ttu-id="4a1b2-128">operationType</span><span class="sxs-lookup"><span data-stu-id="4a1b2-128">operationType</span></span>|[<span data-ttu-id="4a1b2-129">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="4a1b2-129">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="4a1b2-130">Обозначает, какой тип операции описывается.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-130">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="4a1b2-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a1b2-131">createdDateTime</span></span>|<span data-ttu-id="4a1b2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a1b2-132">DateTimeOffset</span></span> |<span data-ttu-id="4a1b2-133">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-133">Time when the operation was created.</span></span>|
|<span data-ttu-id="4a1b2-134">status</span><span class="sxs-lookup"><span data-stu-id="4a1b2-134">status</span></span>|[<span data-ttu-id="4a1b2-135">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="4a1b2-135">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="4a1b2-136">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-136">Operation status.</span></span>|
|<span data-ttu-id="4a1b2-137">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4a1b2-137">lastActionDateTime</span></span>|<span data-ttu-id="4a1b2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a1b2-138">DateTimeOffset</span></span> |<span data-ttu-id="4a1b2-139">Время последнего обновления операции async.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-139">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="4a1b2-140">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="4a1b2-140">attemptsCount</span></span>|<span data-ttu-id="4a1b2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4a1b2-141">Int32</span></span>|<span data-ttu-id="4a1b2-142">Количество попыток операции, прежде чем она была отмечена успешной или неудачной.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-142">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="4a1b2-143">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="4a1b2-143">targetResourceId</span></span>|<span data-ttu-id="4a1b2-144">guid</span><span class="sxs-lookup"><span data-stu-id="4a1b2-144">guid</span></span> |<span data-ttu-id="4a1b2-145">ID объекта, созданного или измененного в результате этой операции async, как правило, [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4a1b2-145">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="4a1b2-146">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="4a1b2-146">targetResourceLocation</span></span>|<span data-ttu-id="4a1b2-147">Строка</span><span class="sxs-lookup"><span data-stu-id="4a1b2-147">string</span></span>|<span data-ttu-id="4a1b2-148">Расположение объекта, созданного или измененного в результате этой операции async.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-148">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="4a1b2-149">Этот URL-адрес должен рассматриваться как непрозрачная величина, а не разрезать его пути компонентов.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-149">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="4a1b2-150">error</span><span class="sxs-lookup"><span data-stu-id="4a1b2-150">error</span></span>|[<span data-ttu-id="4a1b2-151">operationError</span><span class="sxs-lookup"><span data-stu-id="4a1b2-151">operationError</span></span>](operationerror.md)|<span data-ttu-id="4a1b2-152">Любая ошибка, которая вызывает сбой операции async.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-152">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a1b2-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a1b2-153">JSON representation</span></span>

<span data-ttu-id="4a1b2-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a1b2-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


