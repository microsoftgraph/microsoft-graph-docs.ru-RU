---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 3f6a8bdfc6cee8b71fb77fb7778171677acb5df9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966435"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="77718-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="77718-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77718-104">Состояние определенных длительно выполняемых операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="77718-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77718-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77718-105">JSON representation</span></span>

<span data-ttu-id="77718-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77718-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="77718-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="77718-107">Properties</span></span>
| <span data-ttu-id="77718-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="77718-108">Property</span></span>     | <span data-ttu-id="77718-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77718-109">Type</span></span>   |<span data-ttu-id="77718-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77718-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77718-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77718-111">createdDateTime</span></span>| <span data-ttu-id="77718-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77718-112">DateTimeOffset</span></span> |<span data-ttu-id="77718-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="77718-113">The start time of the operation.</span></span>|
|<span data-ttu-id="77718-114">error</span><span class="sxs-lookup"><span data-stu-id="77718-114">error</span></span>|[<span data-ttu-id="77718-115">Оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="77718-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="77718-116">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="77718-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="77718-117">id</span><span class="sxs-lookup"><span data-stu-id="77718-117">id</span></span>|<span data-ttu-id="77718-118">string</span><span class="sxs-lookup"><span data-stu-id="77718-118">string</span></span>|<span data-ttu-id="77718-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77718-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="77718-120">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="77718-120">lastActionDateTime</span></span>| <span data-ttu-id="77718-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77718-121">DateTimeOffset</span></span> |<span data-ttu-id="77718-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="77718-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="77718-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="77718-123">resourceId</span></span>|<span data-ttu-id="77718-124">string</span><span class="sxs-lookup"><span data-stu-id="77718-124">string</span></span>|<span data-ttu-id="77718-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="77718-125">The resource id.</span></span>|
|<span data-ttu-id="77718-126">Ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="77718-126">resourceLocation</span></span>|<span data-ttu-id="77718-127">string</span><span class="sxs-lookup"><span data-stu-id="77718-127">string</span></span>|<span data-ttu-id="77718-128">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="77718-128">The resource URI for the object.</span></span> <span data-ttu-id="77718-129">Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="77718-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="77718-130">status</span><span class="sxs-lookup"><span data-stu-id="77718-130">status</span></span>|<span data-ttu-id="77718-131">string</span><span class="sxs-lookup"><span data-stu-id="77718-131">string</span></span>|<span data-ttu-id="77718-132">Текущее состояние операции: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="77718-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="77718-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="77718-133">percentComplete</span></span>|<span data-ttu-id="77718-134">string</span><span class="sxs-lookup"><span data-stu-id="77718-134">string</span></span>|<span data-ttu-id="77718-135">Процент завершения операции, если операция все еще находится в `running` состоянии.</span><span class="sxs-lookup"><span data-stu-id="77718-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="77718-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="77718-136">Relationships</span></span>
<span data-ttu-id="77718-137">Нет</span><span class="sxs-lookup"><span data-stu-id="77718-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="77718-138">Методы</span><span class="sxs-lookup"><span data-stu-id="77718-138">Methods</span></span>

| <span data-ttu-id="77718-139">Метод</span><span class="sxs-lookup"><span data-stu-id="77718-139">Method</span></span>           | <span data-ttu-id="77718-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77718-140">Return Type</span></span>    |<span data-ttu-id="77718-141">Описание</span><span class="sxs-lookup"><span data-stu-id="77718-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77718-142">Получение операции</span><span class="sxs-lookup"><span data-stu-id="77718-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="77718-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="77718-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="77718-144">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="77718-144">Get the status of the operation.</span></span> |

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
