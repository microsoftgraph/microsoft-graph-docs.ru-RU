---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9e427776d1a001ad3be9badca2dd731c2b42a057
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039207"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="0eaf7-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="0eaf7-103">onenoteOperation resource type</span></span>

<span data-ttu-id="0eaf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eaf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eaf7-105">Состояние определенных длительно выполняемых операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eaf7-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0eaf7-106">JSON representation</span></span>

<span data-ttu-id="0eaf7-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0eaf7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0eaf7-108">Properties</span></span>
| <span data-ttu-id="0eaf7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eaf7-109">Property</span></span>     | <span data-ttu-id="0eaf7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0eaf7-110">Type</span></span>   |<span data-ttu-id="0eaf7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0eaf7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0eaf7-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0eaf7-112">createdDateTime</span></span>| <span data-ttu-id="0eaf7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eaf7-113">DateTimeOffset</span></span> |<span data-ttu-id="0eaf7-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-114">The start time of the operation.</span></span>|
|<span data-ttu-id="0eaf7-115">error</span><span class="sxs-lookup"><span data-stu-id="0eaf7-115">error</span></span>|[<span data-ttu-id="0eaf7-116">оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="0eaf7-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="0eaf7-117">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="0eaf7-118">id</span><span class="sxs-lookup"><span data-stu-id="0eaf7-118">id</span></span>|<span data-ttu-id="0eaf7-119">string</span><span class="sxs-lookup"><span data-stu-id="0eaf7-119">string</span></span>|<span data-ttu-id="0eaf7-120">Идентификатор операции. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="0eaf7-121">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="0eaf7-121">lastActionDateTime</span></span>| <span data-ttu-id="0eaf7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eaf7-122">DateTimeOffset</span></span> |<span data-ttu-id="0eaf7-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="0eaf7-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="0eaf7-124">resourceId</span></span>|<span data-ttu-id="0eaf7-125">string</span><span class="sxs-lookup"><span data-stu-id="0eaf7-125">string</span></span>|<span data-ttu-id="0eaf7-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-126">The resource id.</span></span>|
|<span data-ttu-id="0eaf7-127">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="0eaf7-127">resourceLocation</span></span>|<span data-ttu-id="0eaf7-128">string</span><span class="sxs-lookup"><span data-stu-id="0eaf7-128">string</span></span>|<span data-ttu-id="0eaf7-129">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-129">The resource URI for the object.</span></span> <span data-ttu-id="0eaf7-130">Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="0eaf7-131">status</span><span class="sxs-lookup"><span data-stu-id="0eaf7-131">status</span></span>|<span data-ttu-id="0eaf7-132">string</span><span class="sxs-lookup"><span data-stu-id="0eaf7-132">string</span></span>|<span data-ttu-id="0eaf7-133">Текущее состояние операции: `notstarted` ,, `running` `completed` , `failed`</span><span class="sxs-lookup"><span data-stu-id="0eaf7-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="0eaf7-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="0eaf7-134">percentComplete</span></span>|<span data-ttu-id="0eaf7-135">string</span><span class="sxs-lookup"><span data-stu-id="0eaf7-135">string</span></span>|<span data-ttu-id="0eaf7-136">Процент завершения операции, если операция все еще находится в `running` состоянии.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="0eaf7-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="0eaf7-137">Relationships</span></span>
<span data-ttu-id="0eaf7-138">Нет</span><span class="sxs-lookup"><span data-stu-id="0eaf7-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="0eaf7-139">Методы</span><span class="sxs-lookup"><span data-stu-id="0eaf7-139">Methods</span></span>

| <span data-ttu-id="0eaf7-140">Метод</span><span class="sxs-lookup"><span data-stu-id="0eaf7-140">Method</span></span>           | <span data-ttu-id="0eaf7-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0eaf7-141">Return Type</span></span>    |<span data-ttu-id="0eaf7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0eaf7-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0eaf7-143">Получение операции</span><span class="sxs-lookup"><span data-stu-id="0eaf7-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="0eaf7-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="0eaf7-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="0eaf7-145">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="0eaf7-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


