---
title: Тип ресурса Теамсасинкоператион
description: 'Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dea11ee20e09f1de7c058ef7704e6a824ba2f765
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462258"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="8d13c-103">Тип ресурса Теамсасинкоператион</span><span class="sxs-lookup"><span data-stu-id="8d13c-103">teamsAsyncOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d13c-104">Асинхронная операция Microsoft Teams — это операция, не истечение срока действия одного запроса API.</span><span class="sxs-lookup"><span data-stu-id="8d13c-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="8d13c-105">Эти операции долго выполняются или слишком дороги для завершения в течение периода действия исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="8d13c-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="8d13c-106">При запуске асинхронной операции метод возвращает код ответа, принятый в 202.</span><span class="sxs-lookup"><span data-stu-id="8d13c-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="8d13c-107">В ответе также будет содержаться заголовок Location, который содержит расположение Теамсасинкоператион.</span><span class="sxs-lookup"><span data-stu-id="8d13c-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="8d13c-108">Периодически проверяйте состояние операции, выполнив запрос GET к этому расположению; Дождитесь >30 секунд между проверками.</span><span class="sxs-lookup"><span data-stu-id="8d13c-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="8d13c-109">После успешного выполнения запроса состояние будет "выполнено успешно", а Таржетресаурцелокатион будет указывать на ресурс "создано/изменено".</span><span class="sxs-lookup"><span data-stu-id="8d13c-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="8d13c-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d13c-110">Properties</span></span>

| <span data-ttu-id="8d13c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d13c-111">Property</span></span> | <span data-ttu-id="8d13c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8d13c-112">Type</span></span>   | <span data-ttu-id="8d13c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8d13c-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d13c-114">id</span><span class="sxs-lookup"><span data-stu-id="8d13c-114">id</span></span>|<span data-ttu-id="8d13c-115">строка</span><span class="sxs-lookup"><span data-stu-id="8d13c-115">string</span></span> |<span data-ttu-id="8d13c-116">Уникальный идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-116">Unique operation id.</span></span>|
|<span data-ttu-id="8d13c-117">Оператионтипе</span><span class="sxs-lookup"><span data-stu-id="8d13c-117">operationType</span></span>|[<span data-ttu-id="8d13c-118">Объекта teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="8d13c-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="8d13c-119">Указывает, какие типы операций описаны.</span><span class="sxs-lookup"><span data-stu-id="8d13c-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="8d13c-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d13c-120">createdDateTime</span></span>|<span data-ttu-id="8d13c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d13c-121">DateTimeOffset</span></span> |<span data-ttu-id="8d13c-122">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="8d13c-123">status</span><span class="sxs-lookup"><span data-stu-id="8d13c-123">status</span></span>|[<span data-ttu-id="8d13c-124">Теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="8d13c-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="8d13c-125">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-125">Operation status.</span></span>|
|<span data-ttu-id="8d13c-126">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="8d13c-126">lastActionDateTime</span></span>|<span data-ttu-id="8d13c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d13c-127">DateTimeOffset</span></span> |<span data-ttu-id="8d13c-128">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="8d13c-129">Аттемптскаунт</span><span class="sxs-lookup"><span data-stu-id="8d13c-129">attemptsCount</span></span>|<span data-ttu-id="8d13c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8d13c-130">Int32</span></span>|<span data-ttu-id="8d13c-131">Сколько раз была предпринята попытка выполнения операции до ее пометки как успешной или неудачной.</span><span class="sxs-lookup"><span data-stu-id="8d13c-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="8d13c-132">Таржетресаурцеид</span><span class="sxs-lookup"><span data-stu-id="8d13c-132">targetResourceId</span></span>|<span data-ttu-id="8d13c-133">кодом</span><span class="sxs-lookup"><span data-stu-id="8d13c-133">guid</span></span> |<span data-ttu-id="8d13c-134">Идентификатор объекта, созданного или измененного в результате асинхронной операции, как правило, [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8d13c-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="8d13c-135">Таржетресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="8d13c-135">targetResourceLocation</span></span>|<span data-ttu-id="8d13c-136">строка</span><span class="sxs-lookup"><span data-stu-id="8d13c-136">string</span></span>|<span data-ttu-id="8d13c-137">Расположение объекта, созданного или измененного в результате асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="8d13c-138">Этот URL-адрес должен считаться непрозрачным значением и не был проанализирован в пути к его компонентам.</span><span class="sxs-lookup"><span data-stu-id="8d13c-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="8d13c-139">error</span><span class="sxs-lookup"><span data-stu-id="8d13c-139">error</span></span>|[<span data-ttu-id="8d13c-140">Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="8d13c-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="8d13c-141">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="8d13c-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d13c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d13c-142">JSON representation</span></span>

<span data-ttu-id="8d13c-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d13c-143">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
