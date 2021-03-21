---
title: тип ресурса onenoteOperation
description: Состояние некоторых длительных операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 146cfec00c630fc0abde326a57374549d7b2d378
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961953"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f65b5-103">тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f65b5-103">onenoteOperation resource type</span></span>

<span data-ttu-id="f65b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f65b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f65b5-105">Состояние некоторых длительных операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="f65b5-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f65b5-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f65b5-106">JSON representation</span></span>

<span data-ttu-id="f65b5-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f65b5-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f65b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f65b5-108">Properties</span></span>
| <span data-ttu-id="f65b5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f65b5-109">Property</span></span>     | <span data-ttu-id="f65b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f65b5-110">Type</span></span>   |<span data-ttu-id="f65b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f65b5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f65b5-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f65b5-112">createdDateTime</span></span>| <span data-ttu-id="f65b5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f65b5-113">DateTimeOffset</span></span> |<span data-ttu-id="f65b5-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="f65b5-114">The start time of the operation.</span></span>|
|<span data-ttu-id="f65b5-115">error</span><span class="sxs-lookup"><span data-stu-id="f65b5-115">error</span></span>|[<span data-ttu-id="f65b5-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f65b5-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f65b5-117">Ошибка, возвращаемая операцией.</span><span class="sxs-lookup"><span data-stu-id="f65b5-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="f65b5-118">id</span><span class="sxs-lookup"><span data-stu-id="f65b5-118">id</span></span>|<span data-ttu-id="f65b5-119">string</span><span class="sxs-lookup"><span data-stu-id="f65b5-119">string</span></span>|<span data-ttu-id="f65b5-120">ID операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f65b5-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f65b5-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f65b5-121">lastActionDateTime</span></span>| <span data-ttu-id="f65b5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f65b5-122">DateTimeOffset</span></span> |<span data-ttu-id="f65b5-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="f65b5-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f65b5-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="f65b5-124">resourceId</span></span>|<span data-ttu-id="f65b5-125">string</span><span class="sxs-lookup"><span data-stu-id="f65b5-125">string</span></span>|<span data-ttu-id="f65b5-126">ID ресурса.</span><span class="sxs-lookup"><span data-stu-id="f65b5-126">The resource id.</span></span>|
|<span data-ttu-id="f65b5-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f65b5-127">resourceLocation</span></span>|<span data-ttu-id="f65b5-128">string</span><span class="sxs-lookup"><span data-stu-id="f65b5-128">string</span></span>|<span data-ttu-id="f65b5-129">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="f65b5-129">The resource URI for the object.</span></span> <span data-ttu-id="f65b5-130">Например, ресурс URI для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="f65b5-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f65b5-131">status</span><span class="sxs-lookup"><span data-stu-id="f65b5-131">status</span></span>|<span data-ttu-id="f65b5-132">operationStatus</span><span class="sxs-lookup"><span data-stu-id="f65b5-132">operationStatus</span></span>|<span data-ttu-id="f65b5-133">Текущий статус операции: `NotStarted` `Running` , , `Completed` `Failed` .</span><span class="sxs-lookup"><span data-stu-id="f65b5-133">The current status of the operation: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span> |
|<span data-ttu-id="f65b5-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f65b5-134">percentComplete</span></span>|<span data-ttu-id="f65b5-135">string</span><span class="sxs-lookup"><span data-stu-id="f65b5-135">string</span></span>|<span data-ttu-id="f65b5-136">Если операция по-прежнему находится в состоянии, операция будет `running` завершена в процентах.</span><span class="sxs-lookup"><span data-stu-id="f65b5-136">The operation percent complete if the operation is still in `running` status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f65b5-137">Связи</span><span class="sxs-lookup"><span data-stu-id="f65b5-137">Relationships</span></span>
<span data-ttu-id="f65b5-138">Нет</span><span class="sxs-lookup"><span data-stu-id="f65b5-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="f65b5-139">Методы</span><span class="sxs-lookup"><span data-stu-id="f65b5-139">Methods</span></span>

| <span data-ttu-id="f65b5-140">Метод</span><span class="sxs-lookup"><span data-stu-id="f65b5-140">Method</span></span>           | <span data-ttu-id="f65b5-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f65b5-141">Return Type</span></span>    |<span data-ttu-id="f65b5-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f65b5-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f65b5-143">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="f65b5-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f65b5-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f65b5-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f65b5-145">Получите состояние операции.</span><span class="sxs-lookup"><span data-stu-id="f65b5-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

