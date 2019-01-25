---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512852"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="15193-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="15193-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15193-104">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="15193-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15193-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="15193-105">JSON representation</span></span>

<span data-ttu-id="15193-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15193-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
## <a name="properties"></a><span data-ttu-id="15193-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15193-107">Properties</span></span>
| <span data-ttu-id="15193-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15193-108">Property</span></span>     | <span data-ttu-id="15193-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15193-109">Type</span></span>   |<span data-ttu-id="15193-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15193-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15193-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15193-111">createdDateTime</span></span>| <span data-ttu-id="15193-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15193-112">DateTimeOffset</span></span> |<span data-ttu-id="15193-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="15193-113">The start time of the operation.</span></span>|
|<span data-ttu-id="15193-114">error</span><span class="sxs-lookup"><span data-stu-id="15193-114">error</span></span>|[<span data-ttu-id="15193-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="15193-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="15193-116">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="15193-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="15193-117">id</span><span class="sxs-lookup"><span data-stu-id="15193-117">id</span></span>|<span data-ttu-id="15193-118">string</span><span class="sxs-lookup"><span data-stu-id="15193-118">string</span></span>|<span data-ttu-id="15193-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15193-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="15193-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="15193-120">lastActionDateTime</span></span>| <span data-ttu-id="15193-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15193-121">DateTimeOffset</span></span> |<span data-ttu-id="15193-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="15193-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="15193-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="15193-123">resourceId</span></span>|<span data-ttu-id="15193-124">строка</span><span class="sxs-lookup"><span data-stu-id="15193-124">string</span></span>|<span data-ttu-id="15193-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="15193-125">The resource id.</span></span>|
|<span data-ttu-id="15193-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="15193-126">resourceLocation</span></span>|<span data-ttu-id="15193-127">string</span><span class="sxs-lookup"><span data-stu-id="15193-127">string</span></span>|<span data-ttu-id="15193-p101">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="15193-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="15193-130">status</span><span class="sxs-lookup"><span data-stu-id="15193-130">status</span></span>|<span data-ttu-id="15193-131">string</span><span class="sxs-lookup"><span data-stu-id="15193-131">string</span></span>|<span data-ttu-id="15193-132">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="15193-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="15193-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="15193-133">percentComplete</span></span>|<span data-ttu-id="15193-134">string</span><span class="sxs-lookup"><span data-stu-id="15193-134">string</span></span>|<span data-ttu-id="15193-135">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="15193-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="15193-136">Связи</span><span class="sxs-lookup"><span data-stu-id="15193-136">Relationships</span></span>
<span data-ttu-id="15193-137">Нет</span><span class="sxs-lookup"><span data-stu-id="15193-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="15193-138">Методы</span><span class="sxs-lookup"><span data-stu-id="15193-138">Methods</span></span>

| <span data-ttu-id="15193-139">Метод</span><span class="sxs-lookup"><span data-stu-id="15193-139">Method</span></span>           | <span data-ttu-id="15193-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15193-140">Return Type</span></span>    |<span data-ttu-id="15193-141">Описание</span><span class="sxs-lookup"><span data-stu-id="15193-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15193-142">Получение операции</span><span class="sxs-lookup"><span data-stu-id="15193-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="15193-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="15193-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="15193-144">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="15193-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
