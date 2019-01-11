---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7632186c3e44afbfe0d6cbf3d079ad0758514b38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860265"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="42751-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="42751-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="42751-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42751-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42751-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42751-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42751-106">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="42751-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42751-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="42751-107">JSON representation</span></span>

<span data-ttu-id="42751-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42751-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="42751-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="42751-109">Properties</span></span>
| <span data-ttu-id="42751-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="42751-110">Property</span></span>     | <span data-ttu-id="42751-111">Тип</span><span class="sxs-lookup"><span data-stu-id="42751-111">Type</span></span>   |<span data-ttu-id="42751-112">Описание</span><span class="sxs-lookup"><span data-stu-id="42751-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42751-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42751-113">createdDateTime</span></span>| <span data-ttu-id="42751-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42751-114">DateTimeOffset</span></span> |<span data-ttu-id="42751-115">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="42751-115">The start time of the operation.</span></span>|
|<span data-ttu-id="42751-116">error</span><span class="sxs-lookup"><span data-stu-id="42751-116">error</span></span>|[<span data-ttu-id="42751-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="42751-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="42751-118">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="42751-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="42751-119">id</span><span class="sxs-lookup"><span data-stu-id="42751-119">id</span></span>|<span data-ttu-id="42751-120">строка</span><span class="sxs-lookup"><span data-stu-id="42751-120">string</span></span>|<span data-ttu-id="42751-121">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42751-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="42751-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="42751-122">lastActionDateTime</span></span>| <span data-ttu-id="42751-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42751-123">DateTimeOffset</span></span> |<span data-ttu-id="42751-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="42751-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="42751-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="42751-125">resourceId</span></span>|<span data-ttu-id="42751-126">строка</span><span class="sxs-lookup"><span data-stu-id="42751-126">string</span></span>|<span data-ttu-id="42751-127">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="42751-127">The resource id.</span></span>|
|<span data-ttu-id="42751-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="42751-128">resourceLocation</span></span>|<span data-ttu-id="42751-129">string</span><span class="sxs-lookup"><span data-stu-id="42751-129">string</span></span>|<span data-ttu-id="42751-p102">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="42751-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="42751-132">status</span><span class="sxs-lookup"><span data-stu-id="42751-132">status</span></span>|<span data-ttu-id="42751-133">string</span><span class="sxs-lookup"><span data-stu-id="42751-133">string</span></span>|<span data-ttu-id="42751-134">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="42751-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="42751-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="42751-135">percentComplete</span></span>|<span data-ttu-id="42751-136">string</span><span class="sxs-lookup"><span data-stu-id="42751-136">string</span></span>|<span data-ttu-id="42751-137">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="42751-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="42751-138">Связи</span><span class="sxs-lookup"><span data-stu-id="42751-138">Relationships</span></span>
<span data-ttu-id="42751-139">Нет</span><span class="sxs-lookup"><span data-stu-id="42751-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="42751-140">Методы</span><span class="sxs-lookup"><span data-stu-id="42751-140">Methods</span></span>

| <span data-ttu-id="42751-141">Метод</span><span class="sxs-lookup"><span data-stu-id="42751-141">Method</span></span>           | <span data-ttu-id="42751-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42751-142">Return Type</span></span>    |<span data-ttu-id="42751-143">Описание</span><span class="sxs-lookup"><span data-stu-id="42751-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42751-144">Получение операции</span><span class="sxs-lookup"><span data-stu-id="42751-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="42751-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="42751-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="42751-146">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="42751-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
