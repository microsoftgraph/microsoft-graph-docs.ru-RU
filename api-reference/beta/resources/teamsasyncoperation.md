---
title: Тип ресурса Теамсасинкоператион
description: 'Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 691a2843918707ab05ce798b6c191ea04aa2e42e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519906"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="d8d92-103">Тип ресурса Теамсасинкоператион</span><span class="sxs-lookup"><span data-stu-id="d8d92-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="d8d92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d92-105">Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API.</span><span class="sxs-lookup"><span data-stu-id="d8d92-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="d8d92-106">Эти операции долго выполняются или слишком дороги для завершения в течение периода действия исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="d8d92-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="d8d92-107">При запуске асинхронной операции метод возвращает код ответа, принятый в 202.</span><span class="sxs-lookup"><span data-stu-id="d8d92-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="d8d92-108">В ответе также будет содержаться заголовок Location, который содержит расположение Теамсасинкоператион.</span><span class="sxs-lookup"><span data-stu-id="d8d92-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="d8d92-109">Периодически проверяйте состояние операции, выполнив запрос GET к этому расположению; Подождите >30 секунд между чеками.</span><span class="sxs-lookup"><span data-stu-id="d8d92-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="d8d92-110">После успешного выполнения запроса состояние будет "выполнено успешно", а Таржетресаурцелокатион будет указывать на ресурс "создано/изменено".</span><span class="sxs-lookup"><span data-stu-id="d8d92-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d8d92-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8d92-111">Properties</span></span>

| <span data-ttu-id="d8d92-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8d92-112">Property</span></span> | <span data-ttu-id="d8d92-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d8d92-113">Type</span></span>   | <span data-ttu-id="d8d92-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d8d92-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d92-115">id</span><span class="sxs-lookup"><span data-stu-id="d8d92-115">id</span></span>|<span data-ttu-id="d8d92-116">string</span><span class="sxs-lookup"><span data-stu-id="d8d92-116">string</span></span> |<span data-ttu-id="d8d92-117">Уникальный идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-117">Unique operation id.</span></span>|
|<span data-ttu-id="d8d92-118">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="d8d92-118">operationType</span></span>|[<span data-ttu-id="d8d92-119">Объекта teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="d8d92-119">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="d8d92-120">Указывает, какие типы операций описаны.</span><span class="sxs-lookup"><span data-stu-id="d8d92-120">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="d8d92-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d92-121">createdDateTime</span></span>|<span data-ttu-id="d8d92-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d92-122">DateTimeOffset</span></span> |<span data-ttu-id="d8d92-123">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-123">Time when the operation was created.</span></span>|
|<span data-ttu-id="d8d92-124">status</span><span class="sxs-lookup"><span data-stu-id="d8d92-124">status</span></span>|[<span data-ttu-id="d8d92-125">теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="d8d92-125">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="d8d92-126">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-126">Operation status.</span></span>|
|<span data-ttu-id="d8d92-127">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d8d92-127">lastActionDateTime</span></span>|<span data-ttu-id="d8d92-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d92-128">DateTimeOffset</span></span> |<span data-ttu-id="d8d92-129">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-129">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="d8d92-130">аттемптскаунт</span><span class="sxs-lookup"><span data-stu-id="d8d92-130">attemptsCount</span></span>|<span data-ttu-id="d8d92-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d92-131">Int32</span></span>|<span data-ttu-id="d8d92-132">Сколько раз была предпринята попытка выполнения операции до ее пометки как успешной или неудачной.</span><span class="sxs-lookup"><span data-stu-id="d8d92-132">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="d8d92-133">таржетресаурцеид</span><span class="sxs-lookup"><span data-stu-id="d8d92-133">targetResourceId</span></span>|<span data-ttu-id="d8d92-134">кодом</span><span class="sxs-lookup"><span data-stu-id="d8d92-134">guid</span></span> |<span data-ttu-id="d8d92-135">Идентификатор объекта, созданного или измененного в результате асинхронной операции, как правило, [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d8d92-135">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="d8d92-136">таржетресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="d8d92-136">targetResourceLocation</span></span>|<span data-ttu-id="d8d92-137">string</span><span class="sxs-lookup"><span data-stu-id="d8d92-137">string</span></span>|<span data-ttu-id="d8d92-138">Расположение объекта, созданного или измененного в результате асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-138">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="d8d92-139">Этот URL-адрес должен считаться непрозрачным значением и не был проанализирован в пути к его компонентам.</span><span class="sxs-lookup"><span data-stu-id="d8d92-139">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="d8d92-140">error</span><span class="sxs-lookup"><span data-stu-id="d8d92-140">error</span></span>|[<span data-ttu-id="d8d92-141">оператионеррор</span><span class="sxs-lookup"><span data-stu-id="d8d92-141">operationError</span></span>](operationerror.md)|<span data-ttu-id="d8d92-142">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d8d92-142">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8d92-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8d92-143">JSON representation</span></span>

<span data-ttu-id="d8d92-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8d92-144">The following is a JSON representation of the resource.</span></span>

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
