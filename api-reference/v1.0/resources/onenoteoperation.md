---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
ms.openlocfilehash: 913562abf1d2f644bd621268c93768c7500f4399
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028384"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="1a6d0-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1a6d0-103">onenoteOperation resource type</span></span>

<span data-ttu-id="1a6d0-104">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a6d0-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a6d0-105">JSON representation</span></span>

<span data-ttu-id="1a6d0-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1a6d0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a6d0-107">Properties</span></span>
| <span data-ttu-id="1a6d0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a6d0-108">Property</span></span>     | <span data-ttu-id="1a6d0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a6d0-109">Type</span></span>   |<span data-ttu-id="1a6d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a6d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a6d0-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6d0-111">createdDateTime</span></span>| <span data-ttu-id="1a6d0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6d0-112">DateTimeOffset</span></span> |<span data-ttu-id="1a6d0-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-113">The start time of the operation.</span></span>|
|<span data-ttu-id="1a6d0-114">error</span><span class="sxs-lookup"><span data-stu-id="1a6d0-114">error</span></span>|[<span data-ttu-id="1a6d0-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="1a6d0-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="1a6d0-116">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="1a6d0-117">id</span><span class="sxs-lookup"><span data-stu-id="1a6d0-117">id</span></span>|<span data-ttu-id="1a6d0-118">строка</span><span class="sxs-lookup"><span data-stu-id="1a6d0-118">string</span></span>|<span data-ttu-id="1a6d0-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="1a6d0-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6d0-120">lastActionDateTime</span></span>| <span data-ttu-id="1a6d0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6d0-121">DateTimeOffset</span></span> |<span data-ttu-id="1a6d0-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="1a6d0-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="1a6d0-123">resourceId</span></span>|<span data-ttu-id="1a6d0-124">строка</span><span class="sxs-lookup"><span data-stu-id="1a6d0-124">string</span></span>|<span data-ttu-id="1a6d0-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-125">The resource id.</span></span>|
|<span data-ttu-id="1a6d0-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="1a6d0-126">resourceLocation</span></span>|<span data-ttu-id="1a6d0-127">string</span><span class="sxs-lookup"><span data-stu-id="1a6d0-127">string</span></span>|<span data-ttu-id="1a6d0-p101">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="1a6d0-130">status</span><span class="sxs-lookup"><span data-stu-id="1a6d0-130">status</span></span>|<span data-ttu-id="1a6d0-131">string</span><span class="sxs-lookup"><span data-stu-id="1a6d0-131">string</span></span>|<span data-ttu-id="1a6d0-132">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="1a6d0-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="1a6d0-133">percentComplete</span></span>|<span data-ttu-id="1a6d0-134">string</span><span class="sxs-lookup"><span data-stu-id="1a6d0-134">string</span></span>|<span data-ttu-id="1a6d0-135">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="1a6d0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="1a6d0-136">Relationships</span></span>
<span data-ttu-id="1a6d0-137">Нет</span><span class="sxs-lookup"><span data-stu-id="1a6d0-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="1a6d0-138">Методы</span><span class="sxs-lookup"><span data-stu-id="1a6d0-138">Methods</span></span>

| <span data-ttu-id="1a6d0-139">Метод</span><span class="sxs-lookup"><span data-stu-id="1a6d0-139">Method</span></span>           | <span data-ttu-id="1a6d0-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a6d0-140">Return Type</span></span>    |<span data-ttu-id="1a6d0-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1a6d0-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a6d0-142">Получение операции</span><span class="sxs-lookup"><span data-stu-id="1a6d0-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="1a6d0-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1a6d0-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="1a6d0-144">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
