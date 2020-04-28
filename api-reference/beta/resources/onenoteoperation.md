---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 500a4c20583f6af9cc8bacf98dd4de60354f0ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522346"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="5704b-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="5704b-103">onenoteOperation resource type</span></span>

<span data-ttu-id="5704b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5704b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5704b-105">Состояние определенных длительно выполняемых операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="5704b-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5704b-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5704b-106">JSON representation</span></span>

<span data-ttu-id="5704b-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5704b-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5704b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5704b-108">Properties</span></span>
| <span data-ttu-id="5704b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5704b-109">Property</span></span>     | <span data-ttu-id="5704b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5704b-110">Type</span></span>   |<span data-ttu-id="5704b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5704b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5704b-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5704b-112">createdDateTime</span></span>| <span data-ttu-id="5704b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5704b-113">DateTimeOffset</span></span> |<span data-ttu-id="5704b-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="5704b-114">The start time of the operation.</span></span>|
|<span data-ttu-id="5704b-115">error</span><span class="sxs-lookup"><span data-stu-id="5704b-115">error</span></span>|[<span data-ttu-id="5704b-116">оненотеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="5704b-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="5704b-117">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="5704b-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="5704b-118">id</span><span class="sxs-lookup"><span data-stu-id="5704b-118">id</span></span>|<span data-ttu-id="5704b-119">строка</span><span class="sxs-lookup"><span data-stu-id="5704b-119">string</span></span>|<span data-ttu-id="5704b-120">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5704b-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="5704b-121">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="5704b-121">lastActionDateTime</span></span>| <span data-ttu-id="5704b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5704b-122">DateTimeOffset</span></span> |<span data-ttu-id="5704b-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="5704b-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="5704b-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="5704b-124">resourceId</span></span>|<span data-ttu-id="5704b-125">string</span><span class="sxs-lookup"><span data-stu-id="5704b-125">string</span></span>|<span data-ttu-id="5704b-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="5704b-126">The resource id.</span></span>|
|<span data-ttu-id="5704b-127">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="5704b-127">resourceLocation</span></span>|<span data-ttu-id="5704b-128">string</span><span class="sxs-lookup"><span data-stu-id="5704b-128">string</span></span>|<span data-ttu-id="5704b-129">URI ресурса для объекта.</span><span class="sxs-lookup"><span data-stu-id="5704b-129">The resource URI for the object.</span></span> <span data-ttu-id="5704b-130">Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="5704b-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="5704b-131">status</span><span class="sxs-lookup"><span data-stu-id="5704b-131">status</span></span>|<span data-ttu-id="5704b-132">string</span><span class="sxs-lookup"><span data-stu-id="5704b-132">string</span></span>|<span data-ttu-id="5704b-133">Текущее состояние операции: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="5704b-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="5704b-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="5704b-134">percentComplete</span></span>|<span data-ttu-id="5704b-135">string</span><span class="sxs-lookup"><span data-stu-id="5704b-135">string</span></span>|<span data-ttu-id="5704b-136">Процент завершения операции, если операция все еще находится в `running` состоянии.</span><span class="sxs-lookup"><span data-stu-id="5704b-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="5704b-137">Связи</span><span class="sxs-lookup"><span data-stu-id="5704b-137">Relationships</span></span>
<span data-ttu-id="5704b-138">Нет</span><span class="sxs-lookup"><span data-stu-id="5704b-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="5704b-139">Методы</span><span class="sxs-lookup"><span data-stu-id="5704b-139">Methods</span></span>

| <span data-ttu-id="5704b-140">Метод</span><span class="sxs-lookup"><span data-stu-id="5704b-140">Method</span></span>           | <span data-ttu-id="5704b-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5704b-141">Return Type</span></span>    |<span data-ttu-id="5704b-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5704b-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5704b-143">Получение операции</span><span class="sxs-lookup"><span data-stu-id="5704b-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="5704b-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="5704b-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="5704b-145">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="5704b-145">Get the status of the operation.</span></span> |

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
