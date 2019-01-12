---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977467"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="4ab00-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="4ab00-103">onenoteOperation resource type</span></span>

<span data-ttu-id="4ab00-104">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="4ab00-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ab00-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ab00-105">JSON representation</span></span>

<span data-ttu-id="4ab00-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ab00-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4ab00-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ab00-107">Properties</span></span>
| <span data-ttu-id="4ab00-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ab00-108">Property</span></span>     | <span data-ttu-id="4ab00-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ab00-109">Type</span></span>   |<span data-ttu-id="4ab00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ab00-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ab00-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab00-111">createdDateTime</span></span>| <span data-ttu-id="4ab00-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab00-112">DateTimeOffset</span></span> |<span data-ttu-id="4ab00-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="4ab00-113">The start time of the operation.</span></span>|
|<span data-ttu-id="4ab00-114">error</span><span class="sxs-lookup"><span data-stu-id="4ab00-114">error</span></span>|[<span data-ttu-id="4ab00-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="4ab00-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="4ab00-116">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="4ab00-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="4ab00-117">id</span><span class="sxs-lookup"><span data-stu-id="4ab00-117">id</span></span>|<span data-ttu-id="4ab00-118">строка</span><span class="sxs-lookup"><span data-stu-id="4ab00-118">string</span></span>|<span data-ttu-id="4ab00-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ab00-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="4ab00-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab00-120">lastActionDateTime</span></span>| <span data-ttu-id="4ab00-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab00-121">DateTimeOffset</span></span> |<span data-ttu-id="4ab00-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="4ab00-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="4ab00-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ab00-123">resourceId</span></span>|<span data-ttu-id="4ab00-124">строка</span><span class="sxs-lookup"><span data-stu-id="4ab00-124">string</span></span>|<span data-ttu-id="4ab00-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ab00-125">The resource id.</span></span>|
|<span data-ttu-id="4ab00-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="4ab00-126">resourceLocation</span></span>|<span data-ttu-id="4ab00-127">строка</span><span class="sxs-lookup"><span data-stu-id="4ab00-127">string</span></span>|<span data-ttu-id="4ab00-p101">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="4ab00-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="4ab00-130">status</span><span class="sxs-lookup"><span data-stu-id="4ab00-130">status</span></span>|<span data-ttu-id="4ab00-131">строка</span><span class="sxs-lookup"><span data-stu-id="4ab00-131">string</span></span>|<span data-ttu-id="4ab00-132">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4ab00-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="4ab00-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="4ab00-133">percentComplete</span></span>|<span data-ttu-id="4ab00-134">строка</span><span class="sxs-lookup"><span data-stu-id="4ab00-134">string</span></span>|<span data-ttu-id="4ab00-135">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="4ab00-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="4ab00-136">Связи</span><span class="sxs-lookup"><span data-stu-id="4ab00-136">Relationships</span></span>
<span data-ttu-id="4ab00-137">Нет</span><span class="sxs-lookup"><span data-stu-id="4ab00-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="4ab00-138">Методы</span><span class="sxs-lookup"><span data-stu-id="4ab00-138">Methods</span></span>

| <span data-ttu-id="4ab00-139">Метод</span><span class="sxs-lookup"><span data-stu-id="4ab00-139">Method</span></span>           | <span data-ttu-id="4ab00-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ab00-140">Return Type</span></span>    |<span data-ttu-id="4ab00-141">Описание</span><span class="sxs-lookup"><span data-stu-id="4ab00-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ab00-142">Получение операции</span><span class="sxs-lookup"><span data-stu-id="4ab00-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="4ab00-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="4ab00-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="4ab00-144">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="4ab00-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
