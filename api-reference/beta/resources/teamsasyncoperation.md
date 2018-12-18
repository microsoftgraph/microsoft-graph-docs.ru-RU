---
title: Тип ресурса teamsAsyncOperation
description: 'Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. '
author: nkramer
ms.openlocfilehash: f88f5eba32fbd0629bf66a61dca963a7815988fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305560"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="60b26-103">Тип ресурса teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="60b26-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="60b26-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="60b26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60b26-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b26-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60b26-106">Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API.</span><span class="sxs-lookup"><span data-stu-id="60b26-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="60b26-107">Эти операции выполняются длительным или слишком дорого для выполнения в рамках интервала времени их исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="60b26-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="60b26-108">При запуске асинхронной операции, метод возвращает 202 код ответа принято.</span><span class="sxs-lookup"><span data-stu-id="60b26-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="60b26-109">Ответ также будет содержать заголовок расположения, который содержит расположение teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="60b26-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="60b26-110">Периодически проверяйте состояние операции, сделав запрос GET по этому адресу; Подождите > 30 секунд между проверок.</span><span class="sxs-lookup"><span data-stu-id="60b26-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="60b26-111">После успешного завершения запроса состояния будет иметь «выполнена успешно» и targetResourceLocation будет указывать на ресурс созданные или измененные.</span><span class="sxs-lookup"><span data-stu-id="60b26-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="60b26-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="60b26-112">Properties</span></span>

| <span data-ttu-id="60b26-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="60b26-113">Property</span></span> | <span data-ttu-id="60b26-114">Тип</span><span class="sxs-lookup"><span data-stu-id="60b26-114">Type</span></span>   | <span data-ttu-id="60b26-115">Описание</span><span class="sxs-lookup"><span data-stu-id="60b26-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="60b26-116">id</span><span class="sxs-lookup"><span data-stu-id="60b26-116">id</span></span>|<span data-ttu-id="60b26-117">строка</span><span class="sxs-lookup"><span data-stu-id="60b26-117">string</span></span> |<span data-ttu-id="60b26-118">Операция уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="60b26-118">Unique operation id.</span></span>|
|<span data-ttu-id="60b26-119">operationType</span><span class="sxs-lookup"><span data-stu-id="60b26-119">operationType</span></span>|[<span data-ttu-id="60b26-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="60b26-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="60b26-121">Указывает, какой тип операции, описанного.</span><span class="sxs-lookup"><span data-stu-id="60b26-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="60b26-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60b26-122">createdDateTime</span></span>|<span data-ttu-id="60b26-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b26-123">DateTimeOffset</span></span> |<span data-ttu-id="60b26-124">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="60b26-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="60b26-125">status</span><span class="sxs-lookup"><span data-stu-id="60b26-125">status</span></span>|[<span data-ttu-id="60b26-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="60b26-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="60b26-127">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="60b26-127">Operation status.</span></span>|
|<span data-ttu-id="60b26-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="60b26-128">lastActionDateTime</span></span>|<span data-ttu-id="60b26-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b26-129">DateTimeOffset</span></span> |<span data-ttu-id="60b26-130">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="60b26-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="60b26-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="60b26-131">attemptsCount</span></span>|<span data-ttu-id="60b26-132">Int32</span><span class="sxs-lookup"><span data-stu-id="60b26-132">Int32</span></span>|<span data-ttu-id="60b26-133">Количество раз, когда операция перед помечаются как успешные и неудачные.</span><span class="sxs-lookup"><span data-stu-id="60b26-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="60b26-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="60b26-134">targetResourceId</span></span>|<span data-ttu-id="60b26-135">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="60b26-135">guid</span></span> |<span data-ttu-id="60b26-136">Идентификатор объекта, который создал или изменены в результате этой асинхронной операции, обычно [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="60b26-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="60b26-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="60b26-137">targetResourceLocation</span></span>|<span data-ttu-id="60b26-138">string</span><span class="sxs-lookup"><span data-stu-id="60b26-138">string</span></span>|<span data-ttu-id="60b26-139">Расположение объекта, который создал или изменил как результат этой асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="60b26-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="60b26-140">Этот URL-адрес следует рассматривать как Непрозрачное значение и не синтаксический анализ в его компонента пути.</span><span class="sxs-lookup"><span data-stu-id="60b26-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="60b26-141">error</span><span class="sxs-lookup"><span data-stu-id="60b26-141">error</span></span>|[<span data-ttu-id="60b26-142">operationError</span><span class="sxs-lookup"><span data-stu-id="60b26-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="60b26-143">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="60b26-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60b26-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60b26-144">JSON representation</span></span>

<span data-ttu-id="60b26-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60b26-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
