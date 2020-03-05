---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ff4078938987c1d80462bd1bbdf8c17a90759edd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447313"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="928b2-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="928b2-103">onenoteOperation resource type</span></span>

<span data-ttu-id="928b2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="928b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="928b2-105">Состояние определенных длительно выполняемых операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="928b2-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="928b2-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="928b2-106">JSON representation</span></span>

<span data-ttu-id="928b2-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="928b2-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="928b2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="928b2-108">Properties</span></span>
| <span data-ttu-id="928b2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="928b2-109">Property</span></span>     | <span data-ttu-id="928b2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="928b2-110">Type</span></span>   |<span data-ttu-id="928b2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="928b2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="928b2-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="928b2-112">createdDateTime</span></span>| <span data-ttu-id="928b2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="928b2-113">DateTimeOffset</span></span> |<span data-ttu-id="928b2-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="928b2-114">The start time of the operation.</span></span>|
|<span data-ttu-id="928b2-115">error</span><span class="sxs-lookup"><span data-stu-id="928b2-115">error</span></span>|[<span data-ttu-id="928b2-116">оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="928b2-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="928b2-117">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="928b2-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="928b2-118">id</span><span class="sxs-lookup"><span data-stu-id="928b2-118">id</span></span>|<span data-ttu-id="928b2-119">строка</span><span class="sxs-lookup"><span data-stu-id="928b2-119">string</span></span>|<span data-ttu-id="928b2-120">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="928b2-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="928b2-121">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="928b2-121">lastActionDateTime</span></span>| <span data-ttu-id="928b2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="928b2-122">DateTimeOffset</span></span> |<span data-ttu-id="928b2-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="928b2-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="928b2-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="928b2-124">resourceId</span></span>|<span data-ttu-id="928b2-125">строка</span><span class="sxs-lookup"><span data-stu-id="928b2-125">string</span></span>|<span data-ttu-id="928b2-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="928b2-126">The resource id.</span></span>|
|<span data-ttu-id="928b2-127">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="928b2-127">resourceLocation</span></span>|<span data-ttu-id="928b2-128">строка</span><span class="sxs-lookup"><span data-stu-id="928b2-128">string</span></span>|<span data-ttu-id="928b2-129">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="928b2-129">The resource URI for the object.</span></span> <span data-ttu-id="928b2-130">Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="928b2-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="928b2-131">status</span><span class="sxs-lookup"><span data-stu-id="928b2-131">status</span></span>|<span data-ttu-id="928b2-132">string</span><span class="sxs-lookup"><span data-stu-id="928b2-132">string</span></span>|<span data-ttu-id="928b2-133">Текущее состояние операции: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="928b2-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="928b2-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="928b2-134">percentComplete</span></span>|<span data-ttu-id="928b2-135">строка</span><span class="sxs-lookup"><span data-stu-id="928b2-135">string</span></span>|<span data-ttu-id="928b2-136">Процент завершения операции, если операция все еще находится в `running` состоянии.</span><span class="sxs-lookup"><span data-stu-id="928b2-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="928b2-137">Связи</span><span class="sxs-lookup"><span data-stu-id="928b2-137">Relationships</span></span>
<span data-ttu-id="928b2-138">Нет</span><span class="sxs-lookup"><span data-stu-id="928b2-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="928b2-139">Методы</span><span class="sxs-lookup"><span data-stu-id="928b2-139">Methods</span></span>

| <span data-ttu-id="928b2-140">Метод</span><span class="sxs-lookup"><span data-stu-id="928b2-140">Method</span></span>           | <span data-ttu-id="928b2-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="928b2-141">Return Type</span></span>    |<span data-ttu-id="928b2-142">Описание</span><span class="sxs-lookup"><span data-stu-id="928b2-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="928b2-143">Получение операции</span><span class="sxs-lookup"><span data-stu-id="928b2-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="928b2-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="928b2-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="928b2-145">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="928b2-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
