---
title: Тип ресурса Теамсасинкоператион
description: 'Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9c604d8823de4f48e4338b9637861e8a09505b78
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033756"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="d1086-103">Тип ресурса Теамсасинкоператион</span><span class="sxs-lookup"><span data-stu-id="d1086-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="d1086-104">Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API.</span><span class="sxs-lookup"><span data-stu-id="d1086-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="d1086-105">Эти операции долго выполняются или слишком дороги для завершения в течение периода действия исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="d1086-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="d1086-106">При запуске асинхронной операции метод возвращает код ответа, принятый в 202.</span><span class="sxs-lookup"><span data-stu-id="d1086-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="d1086-107">В ответе также будет содержаться заголовок Location, который содержит расположение Теамсасинкоператион.</span><span class="sxs-lookup"><span data-stu-id="d1086-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="d1086-108">Периодически проверяйте состояние операции, выполнив запрос GET к этому расположению; Подождите >30 секунд между чеками.</span><span class="sxs-lookup"><span data-stu-id="d1086-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="d1086-109">После успешного выполнения запроса состояние будет "выполнено успешно", а Таржетресаурцелокатион будет указывать на ресурс "создано/изменено".</span><span class="sxs-lookup"><span data-stu-id="d1086-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d1086-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1086-110">Properties</span></span>

| <span data-ttu-id="d1086-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1086-111">Property</span></span> | <span data-ttu-id="d1086-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d1086-112">Type</span></span>   | <span data-ttu-id="d1086-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d1086-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d1086-114">id</span><span class="sxs-lookup"><span data-stu-id="d1086-114">id</span></span>|<span data-ttu-id="d1086-115">string</span><span class="sxs-lookup"><span data-stu-id="d1086-115">string</span></span> |<span data-ttu-id="d1086-116">Уникальный идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-116">Unique operation id.</span></span>|
|<span data-ttu-id="d1086-117">Оператионтипе</span><span class="sxs-lookup"><span data-stu-id="d1086-117">operationType</span></span>|[<span data-ttu-id="d1086-118">Объекта teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="d1086-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="d1086-119">Указывает, какие типы операций описаны.</span><span class="sxs-lookup"><span data-stu-id="d1086-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="d1086-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1086-120">createdDateTime</span></span>|<span data-ttu-id="d1086-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1086-121">DateTimeOffset</span></span> |<span data-ttu-id="d1086-122">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="d1086-123">status</span><span class="sxs-lookup"><span data-stu-id="d1086-123">status</span></span>|[<span data-ttu-id="d1086-124">Теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="d1086-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="d1086-125">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-125">Operation status.</span></span>|
|<span data-ttu-id="d1086-126">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d1086-126">lastActionDateTime</span></span>|<span data-ttu-id="d1086-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1086-127">DateTimeOffset</span></span> |<span data-ttu-id="d1086-128">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="d1086-129">Аттемптскаунт</span><span class="sxs-lookup"><span data-stu-id="d1086-129">attemptsCount</span></span>|<span data-ttu-id="d1086-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d1086-130">Int32</span></span>|<span data-ttu-id="d1086-131">Сколько раз была предпринята попытка выполнения операции до ее пометки как успешной или неудачной.</span><span class="sxs-lookup"><span data-stu-id="d1086-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="d1086-132">Таржетресаурцеид</span><span class="sxs-lookup"><span data-stu-id="d1086-132">targetResourceId</span></span>|<span data-ttu-id="d1086-133">кодом</span><span class="sxs-lookup"><span data-stu-id="d1086-133">guid</span></span> |<span data-ttu-id="d1086-134">Идентификатор объекта, созданного или измененного в результате асинхронной операции, как правило, [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d1086-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="d1086-135">Таржетресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="d1086-135">targetResourceLocation</span></span>|<span data-ttu-id="d1086-136">string</span><span class="sxs-lookup"><span data-stu-id="d1086-136">string</span></span>|<span data-ttu-id="d1086-137">Расположение объекта, созданного или измененного в результате асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="d1086-138">Этот URL-адрес должен считаться непрозрачным значением и не был проанализирован в пути к его компонентам.</span><span class="sxs-lookup"><span data-stu-id="d1086-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="d1086-139">error</span><span class="sxs-lookup"><span data-stu-id="d1086-139">error</span></span>|[<span data-ttu-id="d1086-140">Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="d1086-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="d1086-141">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d1086-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1086-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1086-142">JSON representation</span></span>

<span data-ttu-id="d1086-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1086-143">The following is a JSON representation of the resource.</span></span>

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
