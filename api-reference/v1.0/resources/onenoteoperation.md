---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462664"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="ac6e2-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="ac6e2-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6e2-104">Состояние определенных длительно выполняемых операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6e2-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac6e2-105">JSON representation</span></span>

<span data-ttu-id="ac6e2-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ac6e2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac6e2-107">Properties</span></span>
| <span data-ttu-id="ac6e2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac6e2-108">Property</span></span>     | <span data-ttu-id="ac6e2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6e2-109">Type</span></span>   |<span data-ttu-id="ac6e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac6e2-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac6e2-111">createdDateTime</span></span>| <span data-ttu-id="ac6e2-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6e2-112">DateTimeOffset</span></span> |<span data-ttu-id="ac6e2-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-113">The start time of the operation.</span></span>|
|<span data-ttu-id="ac6e2-114">error</span><span class="sxs-lookup"><span data-stu-id="ac6e2-114">error</span></span>|[<span data-ttu-id="ac6e2-115">Оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="ac6e2-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="ac6e2-116">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="ac6e2-117">id</span><span class="sxs-lookup"><span data-stu-id="ac6e2-117">id</span></span>|<span data-ttu-id="ac6e2-118">строка</span><span class="sxs-lookup"><span data-stu-id="ac6e2-118">string</span></span>|<span data-ttu-id="ac6e2-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="ac6e2-120">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="ac6e2-120">lastActionDateTime</span></span>| <span data-ttu-id="ac6e2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6e2-121">DateTimeOffset</span></span> |<span data-ttu-id="ac6e2-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="ac6e2-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="ac6e2-123">resourceId</span></span>|<span data-ttu-id="ac6e2-124">строка</span><span class="sxs-lookup"><span data-stu-id="ac6e2-124">string</span></span>|<span data-ttu-id="ac6e2-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-125">The resource id.</span></span>|
|<span data-ttu-id="ac6e2-126">Ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="ac6e2-126">resourceLocation</span></span>|<span data-ttu-id="ac6e2-127">строка</span><span class="sxs-lookup"><span data-stu-id="ac6e2-127">string</span></span>|<span data-ttu-id="ac6e2-128">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-128">The resource URI for the object.</span></span> <span data-ttu-id="ac6e2-129">Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="ac6e2-130">status</span><span class="sxs-lookup"><span data-stu-id="ac6e2-130">status</span></span>|<span data-ttu-id="ac6e2-131">string</span><span class="sxs-lookup"><span data-stu-id="ac6e2-131">string</span></span>|<span data-ttu-id="ac6e2-132">Текущее состояние операции: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="ac6e2-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="ac6e2-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="ac6e2-133">percentComplete</span></span>|<span data-ttu-id="ac6e2-134">строка</span><span class="sxs-lookup"><span data-stu-id="ac6e2-134">string</span></span>|<span data-ttu-id="ac6e2-135">Процент завершения операции, если операция все еще находится в `running` состоянии.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="ac6e2-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac6e2-136">Relationships</span></span>
<span data-ttu-id="ac6e2-137">Нет</span><span class="sxs-lookup"><span data-stu-id="ac6e2-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="ac6e2-138">Методы</span><span class="sxs-lookup"><span data-stu-id="ac6e2-138">Methods</span></span>

| <span data-ttu-id="ac6e2-139">Метод</span><span class="sxs-lookup"><span data-stu-id="ac6e2-139">Method</span></span>           | <span data-ttu-id="ac6e2-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac6e2-140">Return Type</span></span>    |<span data-ttu-id="ac6e2-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6e2-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac6e2-142">Получение операции</span><span class="sxs-lookup"><span data-stu-id="ac6e2-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="ac6e2-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="ac6e2-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="ac6e2-144">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="ac6e2-144">Get the status of the operation.</span></span> |

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
