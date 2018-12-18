---
title: Тип ресурса teamsAsyncOperation
description: 'Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API. '
author: nkramer
ms.openlocfilehash: fd64f99c20505a8e670c865faa039e9db3174ed6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320610"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="bf2df-103">Тип ресурса teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="bf2df-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="bf2df-104">Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API.</span><span class="sxs-lookup"><span data-stu-id="bf2df-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="bf2df-105">Эти операции выполняются длительным или слишком дорого для выполнения в рамках интервала времени их исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="bf2df-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="bf2df-106">При запуске асинхронной операции, метод возвращает 202 код ответа принято.</span><span class="sxs-lookup"><span data-stu-id="bf2df-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="bf2df-107">Ответ также будет содержать заголовок расположения, который содержит расположение teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="bf2df-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="bf2df-108">Периодически проверяйте состояние операции, сделав запрос GET по этому адресу; Подождите > 30 секунд между проверок.</span><span class="sxs-lookup"><span data-stu-id="bf2df-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="bf2df-109">После успешного завершения запроса состояния будет иметь «выполнена успешно» и targetResourceLocation будет указывать на ресурс созданные или измененные.</span><span class="sxs-lookup"><span data-stu-id="bf2df-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="bf2df-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf2df-110">Properties</span></span>

| <span data-ttu-id="bf2df-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf2df-111">Property</span></span> | <span data-ttu-id="bf2df-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2df-112">Type</span></span>   | <span data-ttu-id="bf2df-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2df-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2df-114">id</span><span class="sxs-lookup"><span data-stu-id="bf2df-114">id</span></span>|<span data-ttu-id="bf2df-115">строка</span><span class="sxs-lookup"><span data-stu-id="bf2df-115">string</span></span> |<span data-ttu-id="bf2df-116">Операция уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bf2df-116">Unique operation id.</span></span>|
|<span data-ttu-id="bf2df-117">operationType</span><span class="sxs-lookup"><span data-stu-id="bf2df-117">operationType</span></span>|[<span data-ttu-id="bf2df-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="bf2df-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="bf2df-119">Указывает, какой тип операции, описанного.</span><span class="sxs-lookup"><span data-stu-id="bf2df-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="bf2df-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf2df-120">createdDateTime</span></span>|<span data-ttu-id="bf2df-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf2df-121">DateTimeOffset</span></span> |<span data-ttu-id="bf2df-122">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="bf2df-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="bf2df-123">status</span><span class="sxs-lookup"><span data-stu-id="bf2df-123">status</span></span>|[<span data-ttu-id="bf2df-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="bf2df-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="bf2df-125">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="bf2df-125">Operation status.</span></span>|
|<span data-ttu-id="bf2df-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="bf2df-126">lastActionDateTime</span></span>|<span data-ttu-id="bf2df-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf2df-127">DateTimeOffset</span></span> |<span data-ttu-id="bf2df-128">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="bf2df-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="bf2df-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="bf2df-129">attemptsCount</span></span>|<span data-ttu-id="bf2df-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bf2df-130">Int32</span></span>|<span data-ttu-id="bf2df-131">Количество раз, когда операция перед помечаются как успешные и неудачные.</span><span class="sxs-lookup"><span data-stu-id="bf2df-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="bf2df-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="bf2df-132">targetResourceId</span></span>|<span data-ttu-id="bf2df-133">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="bf2df-133">guid</span></span> |<span data-ttu-id="bf2df-134">Идентификатор объекта, который создал или изменены в результате этой асинхронной операции, обычно [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bf2df-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="bf2df-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="bf2df-135">targetResourceLocation</span></span>|<span data-ttu-id="bf2df-136">string</span><span class="sxs-lookup"><span data-stu-id="bf2df-136">string</span></span>|<span data-ttu-id="bf2df-137">Расположение объекта, который создал или изменил как результат этой асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="bf2df-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="bf2df-138">Этот URL-адрес следует рассматривать как Непрозрачное значение и не синтаксический анализ в его компонента пути.</span><span class="sxs-lookup"><span data-stu-id="bf2df-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="bf2df-139">error</span><span class="sxs-lookup"><span data-stu-id="bf2df-139">error</span></span>|[<span data-ttu-id="bf2df-140">operationError</span><span class="sxs-lookup"><span data-stu-id="bf2df-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="bf2df-141">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="bf2df-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf2df-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf2df-142">JSON representation</span></span>

<span data-ttu-id="bf2df-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf2df-143">The following is a JSON representation of the resource.</span></span>

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
